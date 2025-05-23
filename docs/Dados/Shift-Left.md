Os dados são a alma das empresas , especialmente quando usados em tempo real.  Em muitas empresas, os dados são isolados, fragmentados e armazenados em vários formatos em diversos sistemas legados e baseados em nuvem.

Para tornar os dados mais acessíveis, a maioria das organizações de TI centraliza o máximo de informações possível.

Por que os pipelines de dados tradicionais não são escaláveis?

- [ ] **Processamento em Lote**:  Movem dados em lotes periódicos;
- [ ] **Equipes de dados centralizadas**:  Única equipe centralizada de engenharia de dados, que precisa aprovar solicitações individuais de dados ou dedicar tempo à construção de novos pipelines e à manutenção dos existentes;
- [ ] **Governança Imatura e Observabilidade**: Linhagem de dados e gerenciamento de erros de dados e esquemas também são desafios;
- [ ] **Processamento de dados com uso intensivo de recursos**: Pipelines tradicionais exigem grande capacidade de computação e armazenamento, e os requisitos estão aumentando à medida que os volumes de dados aumentam;
- [ ] **Design monolítico**:x


Historicamente existe uma grande divisão entre o **Lado Operacional e o Analítico do negócio**, já que cada equipe acaba trabalhando sozinha para obter, limpar, estruturar e usar os dados.

- [ ] Quanto mais longe da fonte você move, copia e transforma os dados, maior a frequência de quebras, maior a latência, mais complexas as dependências.
- [ ] O objetivo de configurar um pipeline de ETL é obter dados do seu **sistema de origem** para o plano **analítico**, para que você possa realizar análises.
- [ ] As equipes de dados ficam isoladas em sua própria área da empresa — com sua própria liderança, seus próprios objetivos de negócios e seus próprios centros de custo.
	- [ ] Da mesma forma, as equipes operacionais também têm sua própria liderança, objetivos e centros de custo, o que pode tornar a cooperação entre as  equipes um pouco lenta.

## Arquiteturas de dados single-hop
Os dados são copiados apenas uma vez, por exemplo, de um sistema de origem para um data lake/warehouse onde os cientistas de dados podem acessá-los.

```mermaid
graph TB
subgraph grp01 [Tabelas de Origem]
direction TB
id01[(e-Business)]
id02[(Fiscal)]
id03[(Pessoal)]
id04[(Gateway)]
end
subgraph grp02 [E.T.L.]
  grp0202@{ shape: dbl-circ, label: "Transformação" }
end
grp01 -->|Extração| grp02 --> |Carga| DWETLELT@{ shape: lin-cyl, label: "Data Warehouse"}
dsp01@{ shape: curv-trap, label: "PowerBI" }
dsp02@{ shape: curv-trap, label: "Tableau" }
DWETLELT <--> dsp01 & dsp02
```

- [ ] Lado Operacional, caracterizado por aplicativos e serviços otimizados para transações de baixa latência.
- [ ] Lado Analítico, caracterizado por consultas grandes e de alta latência ocorrem regularmente, mas dependem de técnicas de otimização inovadas especialmente para análise.

Historicamente, os data warehouses eram o local onde você carregava todos os seus dados limpos e estruturados para fins analíticos — segmentando os dados para responder a consultas.

- [ ] **Star Schema**(Tabelas de fatos no centro conectadas diretamente às tabelas de dimensão);
- [ ] **Snowflake Schema** (Dimensões divididas em tabelas adicionais - normalizadas);
## Arquiteturas de dados multi-hop
Utilizado para arquiteturas em que os dados são processados e copiados diversas vezes antes de finalmente atingirem um nível de qualidade e organização que possa impulsionar um caso de uso comercial específico.

```mermaid
flowchart LR
    subgraph Source["Database Externo"]
direction LR
id01[(e-Business)]
id02[(Fiscal)]
id03[(Pessoal)]
id04[(Gateway)]

    end

    subgraph Processamento
        B[ETL]
    end

    subgraph Estagio
        C1[Raw Data</br>Landing]
        C2[Cleaned Data]
        C3[Business</br>Specific Data]
    end

    subgraph Consumo
        D1[Dashboard]
        D2[Reports]
        D3[AI/ML]
    end

    Source --> B
    B --> C1
    C1 --> C2
    C2 --> C3
    C3 --> D1
    C3 --> D2
    C3 --> D3
```

- [ ] _Zona de pouso ou preparação_:  _Esses dados normalmente vêm de um sistema externo como parte de um_ ETL, uma cópia direta de arquivo ou outro mecanismo de ingestão.
- [ ] Dados básicos limpos: Aplicar filtragem, remodelação e aplicação da qualidade dos dados para converter os dados do estágio 1 para o estágio 2.
- [ ] Dados empresariais selecionados: consistem em conjuntos de dados empresariais específicos criados a partir de dados obtidos no estágio 2.
## Arquitetura Medallion
A arquitetura medalhão é um padrão de design usado por profissionais de dados para organizar e delinear conjuntos de dados. Ela é dividida em três classificações ou camadas de medalhão diferentes, de acordo com o padrão da Medalha Olímpica: bronze, prata e ouro.

Cada uma das três camadas representa qualidade, confiabilidade e garantias progressivamente maiores sendo o bronze o mais fraco e o ouro o mais forte.

Medallion é a adaptação mais recente e popular, e por um bom motivo: faz muito sentido da perspectiva de um profissional de dados que recebe pouca ou nenhuma ajuda das equipes que criam e mantêm os modelos de dados de origem.


```mermaid
flowchart LR
    subgraph Fontes
        A1[Sistemas OLTP]
        A2[APIs]
        A3[Arquivos CSV/JSON]
        A4[Streams Kafka]
    end
    A1 --> B[Ingestão]
    A2 --> B
    A3 --> B
    A4 --> B
    B --> C[Zona Bruta</br>Aterrissagem]
    C --> D[Camada Bronze</br>Dados Brutos]
    D --> E[Camada Prata</br> Dados Limpos e Modelados]
    E --> F[Camada Ouro</br> Dado Curado</br>Agregado]
    F --> G1[BI & Dashboards]
    F --> G2[Data Science & ML]
    F --> G3[APIs de Dados / Exposição]
    G2 -->|Treinamento| H[Loja de recursos]
    H --> E
```

- [ ] A desvantagem da arquitetura Medallion é que todo o trabalho que você faz para deixar os dados limpos, confiáveis e bem formatados (a camada prateada) fica bloqueado no data lake ou no data warehouse.
- [ ] Mover esses dados de prata para a esquerda  significa que podemos publicá-los como um **produto de dados** de primeira classe e fornecê-los a todos os consumidores, operacionais, analíticos ou intermediários;
- [ ] Arquitetura Medallion é cara.
	- [ ] Cada etapa incorre em custos — carregamento de dados;
	- [ ] Encontrar conjuntos de dados semelhantes para reutilização pode ser difícil, pois a abordagem ad hoc para acessar dados tende a gerar silos e descobertas fragmentadas;
	- [ ] ETL falha, todos os trabalhos subsequentes devem ser pausados até que o ETL seja corrigido;
	- [ ] Transfere os dados do seu sistema para o seu data lake por meio de ETL/ELT, você precisa desnormalizá-los, reestruturá-los, padronizá-los, remodelá-los e dar sentido a eles — sem cometer erros;
	- [ ] Dados incorretos farão com que seus clientes percam a confiança;

OU


```mermaid
flowchart TD
    subgraph Fontes de Dados
        DB1[e-Business Suite]
        DB2[PeopleSoft]
        DB3[Supravizio]
        DB4[Contratos]
        DB5[Outras]
    end
    subgraph Bronze["Camada Bronze (Raw Data)"]
        Bronze1[Bruto e-Business Suite]
        Bronze2[Bruto PeopleSoft]
        Bronze3[Bruto Supravizio]
        Bronze4[Bruto Contratos]
        Bronze5[Bruto Outras]
    end
    subgraph Silver["Camada Silver (Cleaned & Structured)"]
        Silver1[Silver Table 1]
        Silver2[Silver Table 2]
        Silver3[Silver Table 3]
    end
    subgraph Gold["Camada Gold (Business-Ready)"]
        Gold1[Gold Table 1]
        Gold2[Gold Table 2]
    end
    DB1 -->|Extração</br>CDC</br>API</br>Queue| Bronze1
    DB2 -->|Extração</br>CDC</br>API| Bronze2
    DB3 -->|Extração</br>CDC</br>API| Bronze3
    DB4 -->|Extração</br>CDC</br>API| Bronze4
    DB5 -->|Extração</br>CDC</br>API| Bronze5

    dsp01@{ shape: curv-trap, label: "PowerBI" }
    dsp02@{ shape: curv-trap, label: "Tableau" }

    Bronze1 -->|Limpeza| Silver1
    Bronze2 -->|Limpeza| Silver1
    Bronze3 -->|Estruturação| Silver2
    Bronze4 -->|Join/Map| Silver2
    Bronze5 -->|Validação| Silver3
    Silver1 --> Gold1 --> dsp01
    Silver2 --> Gold1
    Silver3 --> Gold2 --> dsp02
```




- [ ] **Ingestão**: O processo de coletar dados de diferentes fontes e trazê-los para o ambiente de dados;
- [ ] **Zona de Bruta**: A primeira área de armazenamento após a ingestão, onde os dados são armazenados **exatamente como recebidos**, sem tratamento;
- [ ] **Camada Bronze**: Camada onde os dados são **organizados minimamente** para uso posterior, mantendo ainda sua forma bruta;
- [ ] **Camada Prata**: Camada intermediária com dados **limpos, estruturados, normalizados** e integrados (Correção de dados, tratamento de nulos, deduplicação, Envolve **joins**, **regras de negócio** e **validações** );
- [ ] **Camada final**: com dados **prontos para consumo analítico** ou operacional;
- [ ] **Loja de Recursos**: Promove a **reutilização e padronização** entre equipes.


## A "mentalidade de "cada um por si" predominante nas responsabilidades de acesso a dados
Pegue o código de limpeza SQL que você está executando no seu data lake e deslocá-lo para a esquerda, em direção ao sistema de origem que criou os dados originalmente.

Mover a limpeza, a estruturação e a transformação de dados o mais próximo possível da criação dos dados para que todos possam se beneficiar do resultado.

A migração para a esquerda reduz a complexidade e os custos, eliminando pipelines de dados, processamento e armazenamento de dados duplicados. Elimina a necessidade de
manutenção paralela, elimina o trabalho de correção de falhas no pipeline de dados e libera seus engenheiros para trabalhar em tarefas mais valiosas.

## Levando dados do plano operacional para o plano analítico
A mudança para a esquerda — uma seleção e mudança incremental dos conjuntos de dados importantes que sustentam o seu negócio — funciona na prática para que todos possam se beneficiar de um acesso limpo, simples e confiável aos dados.

Sistemas transacionais fazem parte do plano operacional (preenchido por sistemas de processamento de transações on-line ou OLTP) e são extremamente eficientes no atendimento a seus casos de uso comercial específicos. _Mas os requisitos de negócios vão muito além da gestão de transações_? Responder a essas perguntas exige coletar dados de toda a organização e analisá-los em data warehouses, data lakes ou data lakehouses.

Para piorar a situação, o plano analítico não é o único que precisa de acesso a dados corporativos de alta qualidade.


Nesta era de computação em nuvem desacoplada, microsserviços, mecanismos SQL gerenciados e aplicativos de software como serviço (SaaS), a necessidade de dados corporativos de alta qualidade é maior do que nunca em toda a sua empresa, incluindo a camada operacional.

IA generativa (GenAI), impulsionaram um aumento na demanda por acesso a dados em todos os negócios.

![[Pasted image 20250505204631.png]]

##  Arquitetura de dados Headless
Uma arquitetura de dados headless é o produto de dados, com o qual você já deve estar familiarizado com a abordagem de malha de dados .

Na arquitetura de dados headless, um produto de dados é composto por um fluxo com tecnologia Apache Kafka e sua tabela relacionada com tecnologia Apache Iceberg.

Os dados gravados no fluxo são automaticamente anexados à tabela, permitindo que você os acesse como um tópico do Kafka ou como uma tabela Iceberg.

![[Pasted image 20250505204652.png]]


Os microsserviços são projetados como aplicativos pequenos, autocontidos e independentes.

Eles seguem a filosofia UNIX de fazer uma única coisa e fazê-la bem. Aplicativos mais complexos são criados conectando vários microsserviços entre
si, que se comunicam apenas por meio de interfaces padronizadas, como conexões HTTP RESTful.


```mermaid
flowchart TD
 subgraph id00 ["Eventos"]
    E01@{ shape: tag-rect, label: "Eventos"  }
    E02@{ shape: tag-rect, label: "Resposta" }
 end
 subgraph id01 ["Aplicações"]
   A01@{ shape: brace-r, label: "Comment" }
   A02@{ shape: tag-rect, label: "CRM" }
   A03@{ shape: tag-rect, label: "ERP" }
   A04@{ shape: tag-rect, label: "WEB-APP" }
end
subgraph id02 ["Armazenamento"]
  AR01@{ shape: lin-cyl, label: "ERP" }
  AR02@{ shape: lin-cyl, label: "CRM" }
  AR03@{ shape: lin-cyl, label: "FSC" }
  AR04@{ shape: lin-cyl, label: "PSF" }
end
id00 L1@<==> id01
id01 L2@<==> id02
L1@{ animate: true }
L2@{ animate: true }
```


```mermaid
flowchart TD
 subgraph id01 ["Serviço 01"]
    SVA01@{ shape: tag-rect, label: "CRM" }
    DBA01@{ shape: lin-cyl, label: "CRM" }
    SVA01  Lid01@<==>  DBA01
    Lid01@{ animate: true }
 end
 subgraph id02 ["Serviço 02"]
    SVA02@{ shape: tag-rect, label: "ERP" }
    DBA02@{ shape: lin-cyl, label: "ERP" }
    SVA02  Lid02@<==>  DBA02
    Lid02@{ animate: true }
end
subgraph id03 ["Serviço 03"]
    SVA03@{ shape: tag-rect, label: "PSF" }
    DBA03@{ shape: lin-cyl, label: "PSF" }
    SVA03  Lid03@<==>  DBA03
    Lid03@{ animate: true }
end
subgraph id04 ["Aplicação"]
 APP01@{ shape: tag-rect, label: "Aplicação" }
end
id04 Lid05@<==> id01
id04 Lid06@<==> id02
id04 Lid07@<==> id03
Lid05@{ animate: true }
Lid06@{ animate: true }
Lid07@{ animate: true }
```

## Apache Flink
É um processador de fluxo robusto e robusto, amplamente utilizado em aplicações exigentes como essas.

Seu desempenho e robustez são o resultado de alguns princípios básicos de design, incluindo uma arquitetura "share-nothing" com estado local, processamento em tempo de evento e snapshots de estado (para recuperação).
### Arquitetura Share-Nothing
Em sistemas distribuídos, esta é uma arquitetura onde cada nó é completamente independente de outros nós no sistema. A estrutura de processamento do Hadoop usa o armazenamento HDFS distribuído.

```mermaid
graph TD
    subgraph Nó 1
        DB1[(Banco de Dados 1)]
        App1[Aplicação 1]
        App1 --> DB1
    end

    subgraph Nó 2
        DB2[(Banco de Dados 2)]
        App2[Aplicação 2]
        App2 --> DB2
    end

    subgraph Nó 3
        DB3[(Banco de Dados 3)]
        App3[Aplicação 3]
        App3 --> DB3
    end

    Client[Cliente]
    Client --> App1
    Client --> App2
    Client --> App3
```
Essas arquiteturas também são tolerantes a falhas: cada nó é independente, portanto não há pontos únicos de falha, e o sistema pode se recuperar rapidamente de uma falha de um nó individual.
## Pipelines de Dados de Streaming
Pipelines de dados de streaming são uma abordagem moderna para a entrega de dados como um produto de autoatendimento.

Conectar
Crie e gerencie fluxos de dados com uma interface de usuário visual fácil de usar e conectores pré-criados.

Governça
Gerencie, marque, audite e aplique políticas centralmente para fluxos de dados confiáveis e de alta qualidade.

Enriqueça
Use SQL para combinar, agregar, limpar, processar e moldar dados em tempo real, aumentando a segurança, a eficiência e a usabilidade dos seus fluxos de dados para potencializar casos de uso operacionais, analíticos e de inteligência empresarial.

Construir
Prepare produtos de dados confiáveis e bem formatados para sistemas e aplicativos downstream

Compartilhar
Colabore com segurança em transmissões ao vivo com descoberta e compartilhamento de dados de autoatendimento.

![[Pasted image 20250507202922.png]]
https://developer.confluent.io/courses/apache-flink/intro/?utm_medium=sem&utm_source=google&utm_campaign=ch.sem_br.nonbrand_tp.prs_tgt.dsa_mt.dsa_rgn.latam_lng.eng_dv.all_con.confluent-developer&utm_term=&creative=&device=c&placement=&gad_source=1&gad_campaignid=19560855033&gbraid=0AAAAADRv2c1F6WeDshAB6j7kzQXq_JvjC&gclid=CjwKCAjwiezABhBZEiwAEbTPGPfcLKmQhtdyl11-F9S5lj2lHzPE7tpF8f4tOe3JpApTSQ5S2f5pTRoCyz8QAvD_BwE

# DevSecOps
### Capacite a codificação segura
 Capacitar os desenvolvedores a lidar com vulnerabilidades de segurança logo no início do processo de desenvolvimento — ou a evitar introduzi-las completamente. Uma abordagem de "shift left", em que as considerações de segurança são transferidas para mais perto do início do ciclo de vida de desenvolvimento do software, é significativamente mais econômica e menos disruptiva do que lidar com problemas após a implantação.
 A varredura de segurança baseada em IDE é uma primeira linha de defesa essencial contra vulnerabilidades e ajuda a minimizar uma potencial enxurrada de artefatos inseguros transmitidos às equipes de segurança enquanto os assistentes de codificação produzem o código.

###  Integrar e automatizar os testes de segurança
Os testes integrados garantem que as vulnerabilidades de segurança sejam identificadas o mais rápido possível ao entrarem no projeto e priorizadas para correção antes de serem implantadas em produção. Automação desempenha um papel vital nesse processo, reduzindo o esforço manual, garantindo a consistência nos procedimentos de teste e a tolerância a riscos, além de acelerar o ciclo de feedback para os desenvolvedores.

- [ ] Testes de segurança de aplicativos estáticos (SAST)
- [ ] Análise de composição de software (SCA)
- [ ] Shift Left Security Scan;
- [ ] Testes de segurança de aplicativos dinâmicos (DAST)

### Promova uma mentalidade de “Segurança em Primeiro Lugar”
Cultive um forte senso de responsabilidade pela segurança entre os desenvolvedores é essencial para a construção segura de aplicações em uma cultura de desenvolvimento.
Desenvolvedores com amplo conhecimento dos princípios de segurança e vulnerabilidades comuns estão mais bem equipados para escrever código seguro desde o início, bem como para identificar problemas introduzidos por assistentes de codificação de IA. Isso ajuda a tornar o processo de desenvolvimento mais eficiente e mais preciso.
### Testes de segurança orientados por políticas
Isso envolve o estabelecimento de políticas de segurança centralizadas que possam ser aplicadas de forma consistente em diferentes equipes e projetos, garantindo um nível básico de segurança para todos os aplicativos e habilitando os mecanismos automatizados.
Desenvolver uma plataforma unificada que agregue as descobertas de segurança de todos os testes de segurança (por exemplo, SAST, SCA, IAST, DAST) fornece uma visão abrangente da postura de segurança da organização, exigindo o mínimo de ferramentas de segurança ou variação no fluxo de trabalho para as equipes de AppSec que supervisionam as iniciativas de DevSecOps.

Em resumo:

- [ ] Utilize as melhores práticas do setor da [Open Source Security Foundation (OPSSF)](https://openssf.org/)
- [ ] [Diretrizes existentes para desenvolvimento e distribuição de software seguro](https://github.com/ossf/wg-best-practices-os-developers/blob/main/docs/Existing%20Guidelines%20for%20Developing%20and%20Distributing%20Secure%20Software.md)
- [ ]
