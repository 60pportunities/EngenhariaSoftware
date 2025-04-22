Na última década, assistimos a um crescimento exponencial do volume de dados, impulsionado por avanços na conectividade sem fio, nuvem, proliferação de dispositivos de Internet das Coisas (IoT) e Inteligência Artificial.

Os dados impulsionam partes significativas de nossas vidas, desde recomendações até sistemas de inteligência artificial que identificam tratamentos médicos mais eficazes. 

O mesmo se aplica aos negócios, que estão se tornando cada vez mais **orientados por dados** na busca do aprimoramento de serviços ou venda de produtos ou operações.

O foco principal reside na arquitetura de aplicações de Software como Serviço (SaaS) que lidam com grandes volumes de dados, explorando os benefícios e as considerações de plataformas de dados modernas, especialmente em ambientes de nuvem. 

Uma plataforma de dados robusta, escalável, segregada entre armazenamento e computação, suporte a diferentes tipos de dados (estruturados e semiestruturados), segurança em ambientes multilocatários e novas formas de compartilhamento de dados, deve ser  bem projetada garantirá que os desenvolvedores de aplicativos possam se concentrar no que fazem de melhor — **criar novas experiências de usuário** e **recursos de plataforma para ajudar seus clientes** — sem precisar despender esforços significativos na construção e manutenção de sistemas de dados.
## **Visão Acadêmica**
"Quem nunca ouviu uma área de negócio reclamar que precisa analisar alguma informação importante, mas que a devs/areas de desenvolvimento estão demorando muito pra entregar. Hoje, em uma conversa, disseram TCU."

- [ ] **Falta dos responsáveis pelos dados**: Quem são os responsáveis pelos dados?
- [ ] **Problemas de Qualidade dos dados**: O time de infraestrutura é responsável pela qualidade, mas não conhece os dados tão bem, pois não estão intimamente ligados com o time de negócio.
- [ ] **Escalabilidade Organizacional**: O time centralizado de ETL se torna o gargalo na democratização dos dados na empresa.
### A Explosão de Dados e o Crescimento de Aplicações de Dados
A quantidade de dados criados anualmente está crescendo exponencialmente, impulsionando o desenvolvimento de **"aplicações de dados"** que utilizam esses dados para gerar valor para os clientes.
Trabalhar com grandes volumes de dados requer plataformas especializadas para coleta, organização e exibição.
Aplicações de dados agregam valor ao aproveitar a incrível quantidade e variedade de dados disponíveis para impulsionar oportunidades de negócios novas e existentes.
### Importância de uma Plataforma de Dados Robusta
Uma plataforma de dados bem projetada permite que desenvolvedores de aplicativos se concentrem na criação de novas experiências de usuário e recursos.

Recursos importantes de uma plataforma de dados incluem suporte a diferentes tipos e estruturas de dados, interoperabilidade com ferramentas externas e fontes de dados, e escalabilidade eficiente.
### Ambientes de Nuvem e suas Vantagens
Ambientes de nuvem oferecem vantagens significativas em relação a soluções locais em termos de velocidade, escalabilidade, custo e manutenção.

- [ ] **Elasticidade da Nuvem**: Permite dimensionar recursos para atender à demanda por um custo menor do que expandir um data center, e reduzir recursos quando a carga diminui, oferecendo economia.
- [ ] **Modelos de Nuvem**
	- [ ] **Hospedado na Nuvem**: Executa software projetado para sistemas locais na nuvem. É preferível ao modelo local, mas ainda acarreta manutenção significativa e limita o aproveitamento dos recursos da nuvem.
	- [ ] **Priorizado na Nuvem**: Software desenvolvido especificamente para aproveitar os benefícios da nuvem, como escalabilidade e elasticidade. O provedor assume a responsabilidade pela operação da pilha e pelo dimensionamento automático de recursos. Este modelo é considerado superior.

Ambientes que priorizam a nuvem maximizam os benefícios da nuvem, como a redução de uma parcela significativa da carga de manutenção na criação e operação de aplicativos de dados.

A disponibilidade em múltiplas regiões geográficas pode ser construída de forma mais eficaz em ambientes priorizados na nuvem, com migração automática em caso de problemas em uma região.
### Suporte a Bancos de Dados Relacionais e NoSQL
Bancos de dados relacionais (com suporte a SQL e garantias ACID) continuam sendo componentes críticos para suportar ferramentas de BI embarcadas, visualização e usuários analíticos.

O SQL se beneficia de décadas de desenvolvimento, possui milhões de usuários e um ecossistema robusto.

Dados semiestruturados (como JSON ou Parquet), cuja prevalência cresceu exponencialmente, demandaram o surgimento de bancos de dados NoSQL, que se destacam em gravações rápidas e de alto volume.
No entanto, bancos de dados relacionais evoluíram para incluir suporte a dados semiestruturados e mantêm a vantagem na expressão de consultas analíticas através do SQL.
Bancos de dados NoSQL geralmente requerem o aprendizado de linguagens de programação ou linguagens específicas, o que pode limitar o uso por programadores.
### Separação de Armazenamento e Computação
Historicamente acoplados, a separação de armazenamento e computação em plataformas de dados modernas oferece maior confiabilidade, escalabilidade e redução de custos.
Permite escalar recursos independentemente de acordo com a demanda (mais poder computacional em picos, mais armazenamento com o crescimento dos dados).
Evita custos adicionais por recursos desnecessários que seriam provisionados juntos em sistemas acoplados.
Protege contra perda de dados em caso de falhas na instância de computação.
### Isolamento de Carga de Trabalho em Ambientes Multilocatários:
Em aplicações de dados com múltiplos clientes (locatários), é crucial isolar as cargas de trabalho de ingestão, analíticas e as cargas de trabalho de diferentes clientes uns dos outros para evitar a degradação do desempenho.
Existe uma disputa inerente por recursos em sistemas de dados, tornando o isolamento essencial.
### Extensibilidade da Plataforma de Dados
A capacidade de utilizar recursos de terceiros e código personalizado (User-Defined Functions - UDFs e Stored Procedures) é importante.
UDFs permitem encapsular código (em SQL, Python, Java) para reutilização em consultas SQL.
Stored Procedures são sub-rotinas SQL armazenadas em bancos de dados relacionais, úteis para gerar SQL dinamicamente ou executar operações CRUD.
A integração com sistemas externos para obter dados adicionais ou realizar análises é uma necessidade frequente.
### Escalabilidade em Aplicações de Dados
Escalabilidade é um requisito fundamental para o sucesso de aplicações de dados, permitindo integrar novos clientes rapidamente, executar novas cargas de trabalho sem impactar outros e aproveitar a elasticidade da nuvem para controlar custos.

- [ ] **Escalabilidade Vertical**: Fornecer recursos mais poderosos para executar uma tarefa.
- [ ] **Escalabilidade Horizontal**: Adicionar mais nós (instâncias) para lidar com o aumento da demanda. Plataformas priorizadas na nuvem geralmente gerenciam esse processo automaticamente.

Warehouses virtuais (como no Snowflake) e warehouses multicluster são mencionados como mecanismos para fornecer escalabilidade e isolamento de recursos computacionais para diferentes locatários e níveis de serviço.
### Padrões de Design para Armazenamento em Ambientes Multilocatários
Diferentes métodos para isolar dados entre locatários:
- [ ] **Tabelas Multilocatário**: Todos os locatários compartilham as mesmas tabelas, com segurança aplicada no nível da linha ou coluna. Requer consideração para garantir o desempenho.
- [ ] **Objeto por Locatário**: Locatários possuem seus próprios bancos de dados, esquemas e tabelas, agrupados em uma única instância de banco de dados, com controle de acesso baseado em função (RBAC). Pode se tornar difícil de gerenciar com muitos clientes.
- [ ] **Conta por Locatário**: Cada locatário possui uma instância de banco de dados dedicada associada à sua conta. Oferece maior isolamento, mas aumenta a sobrecarga administrativa e de manutenção.
### Padrões de Design para Segurança em Ambientes Multilocatários
A segurança dos dados é uma preocupação fundamental dos clientes.
Mecanismos de segurança devem incluir garantias para requisitos regulatórios e contratuais, bem como gerenciamento de acesso a dados e recursos computacionais.
- [ ] **Controle de Acesso Baseado em Função (RBAC)**: Agrupa privilégios em funções que são atribuídas aos usuários.
- [ ] **Controle de Acesso Discricionário (DAC)**: Proprietários de objetos podem conceder acesso a outros usuários a seu critério. O Snowflake combina esses modelos, com proprietários concedendo acesso por meio de funções atribuídas aos usuários.
É recomendável minimizar a distribuição de privilégios de um objeto entre várias funções e utilizar uma hierarquia de funções para criar combinações de privilégios.
A capacidade de auditar alterações nos controles de acesso é crucial.
Outras considerações de segurança incluem autenticação, gerenciamento de criptografia e design de rede segura.
### Processamento de Dados (ETL vs ELT):
- [ ] **Data Warehouses**: Armazenam apenas dados conformados (transformados em um esquema definido durante a ingestão).
- [ ] **Data Lakes**: Contêm dados em seu formato bruto, com a transformação ocorrendo sob demanda (esquema na leitura).
A decisão sobre o que conformar e o que deixar em estado bruto depende de como os dados serão usados.
- [ ] **ETL (Extract, Transform, Load)**: Dados são transformados antes de serem carregados no data warehouse.
- [ ] **ELT (Extract, Load, Transform)**: Dados brutos são carregados primeiro e a transformação ocorre quando necessário para análise (esquema na leitura). O ELT é facilitado por plataformas de nuvem com poder computacional elástico.
O esquema na leitura (ELT) é preferido por fornecedores de dados, pois reduz a carga de lidar com alterações na fonte de dados.

O tipo de dado VARIANT do Snowflake permite o esquema na leitura para dados semiestruturados.
- [ ] **Processamento em Lote (Batch Processing)**: Processa grandes volumes de dados em intervalos definidos.
- [ ] **Processamento de Streaming**: Opera continuamente em eventos individuais ou microlotes.
### Compartilhamento de Dados
A capacidade de compartilhar dados com segurança e em tempo real é essencial para aplicações de dados.
- [ ] **Compartilhamento por Cópia**: Abordagem legada que envolve a criação e transferência de cópias de dados, gerando custos de armazenamento, sobrecarga de manutenção e problemas de versionamento e atualização.
- [ ] **Compartilhamento por Referência**: Abordagem moderna onde os dados permanecem fixos e o acesso é concedido por meio de referências, eliminando a necessidade de cópia e permitindo o compartilhamento imediato e revogação de acesso.

O Snowflake Secure Data Sharing permite que consumidores e provedores acessem a mesma cópia dos dados, aproveitando a arquitetura de dados compartilhados e multicluster. O acesso é controlado pela camada de serviços e metadados, permitindo concessão e revogação instantâneas.
- [ ] **Snowflake Data Marketplace**: Permite que provedores de dados monetizem seus dados e que consumidores descubram e acessem dados de diversas fontes sem a complexidade da cópia.

O compartilhamento de dados por referência quebra silos de dados, facilita um ciclo de feedback entre provedores e consumidores e mantém custos e carga de manutenção sob controle.


### Principais Recursos de uma Plataforma de Dados Moderna (implícito)

- [ ] Separação de armazenamento e computação.
- [ ] Suporte nativo para dados semiestruturados.
- [ ] Suporte para SQL padrão.
- [ ] Isolamento de carga de trabalho em ambientes multilocatários.
- [ ] Escalabilidade elástica para corresponder à demanda.
- [ ] Recursos de compartilhamento de dados seguros e eficientes.
### **Conceituando**
Integridade de dados refere-se à garantia de que os dados permanecerão precisos, inalterados e consistentes durante todo o seu ciclo de vida.

| **Característica**     | **Data Warehouse**                                                     | **Data Lake**                                                           | **Data Mesh**                                                            |
| :--------------------- | :--------------------------------------------------------------------- | :---------------------------------------------------------------------- | :----------------------------------------------------------------------- |
| **Tipo de Dados**      | Dados estruturados                                                     | Dados estruturados e não estruturados                                   | Dados distribuídos, por domínio                                          |
| **Processamento**      | ETL (Extração, Transformação e Carga antes do armazenamento)           | ELT (Extração, Carga e Transformação após o armazenamento)              | Processamento descentralizado por cada domínio                           |
| **Objetivo Principal** | Análises de Business Intelligence (BI) e relatórios                    | Armazenamento de grandes volumes de dados brutos para análise posterior | Escalabilidade e autonomia na gestão de dados por domínio                |
| **Exemplo de Uso**     | Relatórios financeiros, dashboards e KPIs                              | Análises de dados não estruturados, machine learning, logs              | Grandes organizações com múltiplos departamentos e sistemas distribuídos |
| **Escalabilidade**     | Limitada, pois depende de uma estrutura centralizada                   | Alta, permite armazenamento de dados em grande escala                   | Muito alta, cada domínio pode escalar independentemente                  |
| **Governança**         | Centralizada, controlada por uma equipe de TI                          | Menos rigorosa, exige boas práticas de governança                       | Descentralizada, cada domínio gerencia seus próprios dados               |
| **Vantagens**          | Consultas rápidas, alta performance para BI                            | Flexibilidade no armazenamento de dados e baixo custo                   | Autonomia, escalabilidade e alinhamento com as necessidades de negócios  |
| **Desvantagens**       | Rigidez na estrutura de dados, dificuldades com dados não estruturados | Governança e consultas podem ser mais difíceis de gerenciar             | Complexidade de gestão e padronização entre os domínios                  |
| **Tecnologias Comuns** | Google BigQuery, Amazon Redshift, Snowflake, Microsoft SQL Server      | Hadoop, Apache Spark, AWS S3, Azure Data Lake, Google Cloud Storage     | Arquitetura distribuída, com ferramentas como Kubernetes, Kafka, etc.    |
###  **Arquitetura Integração de Dados**
As arquiteturas de integração de dados tornam-se canais para coletar e fornecer insights sobre processos e dados de negócios.
### **Arquitetura Integração de Dados**
A economia digital colocou mais demanda por serviços de dados dentro de uma organização, sobrecarregando a TI para fornecer esses serviços, acarretando uma proliferação de integrações não governadas na verdade piora na entrega e manutenção da mesma.

Arquiteturas de integração de dados consistem em múltiplas tecnologias que também podem ser alinhadas a outras áreas, como gerenciamento de dados ou governança de dados. 
As arquiteturas de integração de dados tornam-se canais para coletar e fornecer insights sobre processos e dados de negócios.
A integração de dados geralmente é uma tarefa dentro de um projeto maior, sendo um método que fornece dados que podem suportar algum conjunto de requisitos de negócios, objetivando uma melhorara na eficiência geral das organizações comerciais e técnicas, validando efetivamente seus pipelines e resultados de dados e análises.
Uma arquitetura de integração auxuliará a organizar as integrações em um ambiente coerente e estruturado.
Para podermos iniciar o trabalho, foi necessário efetuar um mapeamento dos dados mestres e referêmcia, propondo uma higienização durante o processo de implantação de um novo sistema de Gestão Empresarial. Nosso objetivo foi a promoção da higienização, designação do gestor, background check e seus metadados.
Foram identificados neste trabalho, ciclos viciosos de desenvolvimento em uma arquitetura acidental, que não garantiam a qualidade dos dados, aumentavam as dívida técnica e de processo.
Eventualmente, surgem perguntas sobre como os resultados foram derivados, a qualidade dos dados, a fonte dos dados e por que as mesmas métricas têm resultados diferentes em diferentes operações de negócios.

Uma arquitetura de integração de dados consiste nas tecnologias, dados e padrões, processos de negócios, necessidades de armazenamento e requisitos operacionais que permitem a entrega da integração de dados.

| Requisitos             | Tecnologia   | Design              | Implementação       | Monitoramento |
| ---------------------- | ------------ | ------------------- | ------------------- | ------------- |
| Dados Estruturados     | Mensageria   | Replicação          | Data Pipeline       | Custo         |
| Dados Não Estruturados | ETL/ELT/ETLT | Preparação          | Integração Metadata | Adminitração  |
| Processos de Negócio   | Orquestração | Transformação       | Armazenagem         | Suporte       |
| Metadata               | DatOps       | Orquestraçãp        |                     |               |
| Temporalidade          | Catalogação  | ETL/ELT/ETLT        |                     |               |
| Performance            |              | Pipeline Integração |                     |               |

## **Base de governança de dados e gerenciamento de informações**

Crie uma base de governança de dados e gerenciamento de informações para dar suporte ao gerenciamento de dados mestres e gerenciamento de metadados para dar suporte a casos de uso de governança de dados e análises; desenvolva novas habilidades e práticas recomendadas; e estabeleça segurança, privacidade e conformidade no gerenciamento de dados.

## **Arquitetura e modernização de gerenciamento de dados**
Implante uma infraestrutura de gerenciamento de dados escalável e confiável e arquitete a arquitetura de dados moderna mais adequada, incluindo gerenciamento de dados local, nativo da nuvem e híbrido para oferecer suporte a volume, velocidade e variedade de dados extremos.
## Princípios e implantações de gerenciamento de dados
Selecione, projete, implante e operacionalize sistemas de gerenciamento de dados usando tendências emergentes em armazenamentos de dados para fins especiais, como armazenamentos não relacionais, gráficos e de objetos, e migre bancos de dados para executar cargas de trabalho híbridas, multicloud e de borda.
## Integração de dados de última geração
Desenvolva as melhores práticas e arquitetura para integração de dados, aproveitando os princípios de engenharia de dados e as tecnologias de virtualização de dados para oferecer suporte a casos de uso de streaming em lote e em tempo real.
## Design de integrações usando métodos apropriados
O design de uma arquitetura de integração pega os processos de negócios definidos e os traduz em pipelines de integração. As fontes de dados e processos se tornam o pipeline de integração; o uso de dados e os tipos de dados se tornam os métodos de integração e transformações; e a usabilidade e o acesso aos dados se torna Insights sobre formatos de dados, uso dos dados, métodos de armazenamento, podem determinar o método de integração.
#### **Processos de negócios e regras de transformação**
As perguntas a serem respondidas pelos requisitos do processo incluem:

| Perguntas                                                | Perguntas                                              |
| -------------------------------------------------------- | ------------------------------------------------------ |
| Qual é a fonte dos dados ?                               | Existe algum Orgão regulador? Há contratos?            |
| Quem criará os dados?                                    | Quem poderá ler, consultar ou manter?                  |
| Dados históricos deverão ser mantidos, por quanto tempo? | Dados históricos precisarão ser modificados?           |
| Quais os tipos de validações, serão necessárias?         | Como os dados serão usados?                            |
| Que tipo de metadados devem ser capturados?              | Como os usuários consumirão/acessarão os dados finais? |

Os metadados contêm as informações necessárias para fornecer informações sobre definições de dados ou dicionários, linhagem de dados, pipelines de dados para usuários corporativos e desenvolvedores.

Esses tipos incluem metadados operacionais (relacionados a operações da arquitetura de integração, como tempos de execução de pipeline, número de falhas, transformações, agregações e junções executadas em dados) e metadados de negócios (como dicionários de dados e linhagem).
## Métodos de integração
Existem vários métodos de integração de dados, dependendo do formato, caso de uso e volume. Há plataformas de integração que fornecem recursos que vão além de apenas extrair, transformar e carregar (ETL/ELT/ETLT), como catálogos de dados, recursos de IA, governança de dados e suporte a DataOps, integração de fluxo ou virtualização.

| Técnica de Integração  | Descrição                                                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Replicação             | Pode ser considerada a forma mais básica de integração, pois envolve a cópia direta de dados de um sistema para outro.                                                                                          |
| Virtualização          | Executa consultas em várias fontes de dados para criar visualizações virtuais integradas de dados sob demanda.                                                                                                  |
| ETL/ELT                | Os dados de origem são extraídos e podem ser gravados como um arquivo em lote ou processados em trânsito, aproveitando uma ferramenta ou plataforma de integração de dados.                                     |
| ETLT                   | Mesmos conceitos fundamentais de ETL, porem, o processo de integração envolve várias etapas de extração, transformação e carga, e também pode incluir etapas adicionais de carregamento e transformação.        |
| Stream Data Processing | É um método para ingerir, integrar e processar dados em tempo real assim que são produzidos. A latência entre a criação e o processamento de dados é extremamente baixa em comparação ao processamento em lote. |
## Plataformas de integração
As plataformas de integração visam ser uma plataforma única para recursos de dados.
Com as permissões e acesso adequados, os usuários podem acessar dicionários de dados, entender a precisão e a qualidade dos dados, integrar dados mestres, visualizar a linhagem de dados e ver transformações, validações e quaisquer consolidações de dados até a fonte.
## Scheduler e Workflow Manager
O agendamento de pipeline de integração e o gerenciamento de fluxo de trabalho, como execução de frequência de trabalhos, alertas e automação são padrão, definidas nestas plataformas.
## Catálogos de dados
Os catálogos de dados armazenam metadados, tanto operacionais quanto comerciais, que complementam as transformações de dados ou análises para visualizar a jornada de dados.

- [ ] CI/CD, DataOps, Orquestração: Orquestração é o processo de criação de uma unidade lógica de pipelines de dados relacionados, fluxos de trabalho e componentes associados que produzem os conjuntos de dados desejados, incluindo seus artefatos (por exemplo, metadados, dicionário de dados, qualidade de dados e estatísticas de validação).
- [ ] HA, DR, Escalabilidade: O foco principal em alta disponibilidade (HA) e recuperação de desastres (DR) é manter o sistema operacional o tempo todo. No entanto, a principal diferença é que a HA aborda o problema enquanto o sistema é executado, enquanto a DR entra depois que ele falha.

Independentemente de quão altamente disponível um sistema seja, qualquer aplicativo de produção precisa ter planos de recuperação de desastres, pois alta disponibilidade e recuperação de desastres não são mutuamente exclusivas.
## Integração
A implementação dependerá das funções e recursos da ferramenta, que deveriam ter sido avaliados.
  
- [ ] Qual a melhor forma de implementar o CDC e onde?
- [ ] Como lidamos com dados atrasados/duplicados?
- [ ] Em caso de falha do pipeline, o processo deve ser executado novamente ou precisa continuar de onde falhou? Quais verificações de integridade de dados são necessárias?
- [ ] Como acompanhamos as métricas e monitoramos os pipelines de qualidade de dados (DQ)/SLAs?
- [ ] Como maximizamos o desempenho — taxa de transferência ou latência?
- [ ] Como orquestramos pipelines de dados de ponta a ponta?
- [ ] Como podemos depurar a lógica de transformação em um ambiente altamente distribuído?
- [ ] Como o sistema lida com a propagação de alterações upstream?
- [ ] Como gerenciamos a configuração e o estado do pipeline?
- [ ] Como a reutilização será gerenciada/integrada às equipes de desenvolvimento?
- [ ] Qual é o processo de implantação?
- [ ] O que é o ambiente de desenvolvimento?
- [ ] Como o aterro será realizado?
- [ ] Como implementamos pipelines de dados orientados por metadados?

| Tipo                 | Descricao                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Microlotes           | Divide o conjunto de dados resultante em lotes menores, agendando as extrações várias vezes ao longo do dia e da noite.                                                                                                                                                                                                                                                                                                                                            |
| Integração em lote   | Método tradicional, onde o processo começa assim que todos os dados a serem integrados são identificados, seja de um arquivo ou consultando o sistema de origem.                                                                                                                                                                                                                                                                                                   |
| Streaming de eventos | Fluxos de eventos de alta frequência que precisam ser processados dentro de SLAs muito rígidos – por exemplo, na detecção de fraudes, monitoramento de rede, consistência transacional ou monitoramento da cadeia de suprimentos – podem aproveitar o streaming de eventos. À medida que os eventos são processados no pipeline do fluxo de eventos, eles podem ser mesclados/atualizados/adicionados aos dados históricos armazenados para análise em tempo real. |
| Virtualização        | Método eficaz para combinar fontes de dados diferentes em uma única camada de acesso sem precisar mover dados fisicamente.                                                                                                                                                                                                                                                                                                                                         |
| Replicação           | Método que pega os dados da origem e os copia diretamente para o destino especificado.                                                                                                                                                                                                                                                                                                                                                                             |
## Armazenamentos de dados e modelos de dados
Do ponto de vista da integração de dados, os armazenamentos de dados podem servir a várias finalidades. Eles podem ser uma área central que armazena todos os dados de origem em vários formatos, armazenamentos intermediários para dados processados, armazenamentos temporários para integrações e agregações temporárias ou o produto de dados final em que os dados estão prontos para serem consumidos pelos usuários finais.
  
- [ ] Os dados residirão em uma tabela existente ou em uma nova tabela?
- [ ] Como os dados serão usados?
- [ ] Existem preocupações com a segurança dos dados/informações de identificação pessoal (LGPF, GPDR, HIPAA)?
- [ ] A quais dimensões os dados serão associados se empregar um esquema em estrela?

## Fluxo de trabalho de agendamento e integração
Os pipelines de integração precisarão de alguma forma de agendamento para serem executados em um agendamento ou janela designada. Alguns pipelines de integração também terão dependências de outros pipelines antes de serem executados.
O desenvolvimento da ingestão de dados é a base para a extração de dados de sistemas de dados de origem e orquestração de diferentes métodos de integração de gerenciamento de dados.
## Monitorar/Suporte
Métricas bem definidas podem ser aproveitadas para avaliar a qualidade dos dados. Métricas operacionais sobre tempo de atividade, tempo defuncionamento, tempo para resolver problemas e monitoramento proativo de possíveis problemas também podem ser coletadas.
Os aspectos de administração podem exigir a integração de novas administrações e suporte ao conhecimento de novas ferramentas de integração e metodologias de desenvolvimento, como implantação rápida. Existem duas áreas distintas de administração de suporte: a administração de infraestrutura, operações e aplicativos e a administração dos pipelines de integração e aplicativos relacionados.
  
```mermaid

flowchart LR

DS[(Data Source)] & newLines["`Data

Sources`"] --> |Pull/Push| id1(Ferramentas</br>Ingestão)

id1 --> id2(Processamento</br>de dados)

id2 --> id3(Armazenamento</br>de dados)

id3 --> id4(Consumo</br>de dados)

```

## Plataforma de Dados
Implantar a plataforma de dados significa abrir as válvulas para permitir a entrada dos dados (lote/streaming).
Essa deve ser a última etapa da implantação e deve ser feita no final do provisionamento da plataforma de processamento/ingestão.
  
- [ ] Verifique se o armazenamento de dados é provisionado com políticas de capacidade/acesso a dados.
- [ ] Verifique se um agente de streaming está provisionado e pronto.
- [ ] Verifique as qualidade dos dados são implantadas;
- [ ] Orquestração de dados seja provisionada;
- [ ] Ferramentas de gerenciamento e controle de versão do ciclo de vida dos dados estejam implantadas e prontas.
- [ ] Ferramentas de detecção de descompasso de dados estejam em vigor e ativas.
- [ ] Defina métricas a serem monitoradas em cada camada.
- [ ] Defina o intervalo normal de métricas.
- [ ] Armazene métricas em um repositório de configuração.
- [ ] Selecione ferramentas para monitoramento e observabilidade de dados — não há uma ferramenta única
- [ ] Obtenha respostas para estas perguntas no sistema de monitoramento:
- [ ] O processamento/ingestão de dados está ocorrendo na taxa/latência esperada?
- [ ] Existem problemas de qualidade de dados na ingestão, postagem, pré-processamento e pós-processamento?
- [ ] As variáveis de ambiente/sistema/aplicativo são otimizadas para o fluxo e o processamento de dados?
- [ ] Realize o monitoramento de esquema.
- [ ] Realize o monitoramento da qualidade dos dados.
- [ ] Taxas de transferência;
- [ ] Taxas de erro;
- [ ] Tempo de execução por estágio;
- [ ] Erros de estrutura;
- [ ] Detecção de informações de identificação pessoal (PII);
- [ ] Alertas de desvio de esquema;
- [ ] Alertas de desvio semântico;
- [ ] Métricas de execução de trabalho e metadados correspondentes;
- [ ] O tempo para iterar representa a capacidade de entender, monitorar e depurar pipelines existentes e criar novos
- [ ] Hora de implantar;
- [ ] Hora de resolver problemas;
- [ ] Frequência de implantação;
- [ ] Tempo médio de restauração (MTTR);
- [ ] Prazo de entrega para alterações;
- [ ] Hora de restaurar os serviços;
- [ ] Taxa de falha de alteração

## Automação  

## Avaliando as opções de arquitetura para bancos de dados multicloud
As arquiteturas centradas em dados multicloud são complexas.
### O que é multicloud?
No contexto de arquiteturas multicloud, é útil entender a distinção entre "híbrido" e "intercloud":

- [ ] Híbrido refere-se a componentes locais que são combinados com componentes baseados em nuvem.
- [ ] Intercloud refere-se a componentes de solução baseados em nuvem que estão sendo implantados em vários ambientes de nuvem.

![](../img/multicloud.png)

## Data Lake  
- [ ] **Transient/Staging**: Camada onde os dados são recebidos e armazenados em seu formato original.
- [ ] **Bronze/Raw**: Camada onde os dados são transformados para um formato padronizado e carregados no data lake.
- [ ] **Silver/Trusted**: Camada onde os dados são limpos, corrigidos e enriquecidos com metadados.
- [ ] **Gold/Refined**: Camada onde os dados são preparados para análise e visualização.
- [ ] **Sandbox**: Camada onde os dados são usados para desenvolvimento, testes e experimentação.

![](../img/post_camadaslake_img01.jpg)
### Existem três grupos principais em um ecossistema de dados moderno:
- [ ] **Produtores de dados**: Os especialistas de domínio que possuem os sistemas ou fontes de dados recebidos (pedidos, faturas, inventário e assim por diante).
- [ ] **Construtores de Plataforma de Dados**: Um segmento da equipe de TI com diversas habilidades de dados, dependendo da maturidade da empresa.
- [ ] **Consumidores de Dados**: Analistas e operadores que usam dados para otimizar os negócios, tomar decisões e definir estratégias.
## Data Mesh (Zhamak Dehghani)
<p align="justify">O gerenciamento é conduzido no nível da unidade, onde os indivíduos mais familiarizados com os dados em suas respectivas áreas determinam os métodos de processamento ideais. Sua proximidade com os dados e familiaridade com os requisitos permitem que eles garantam sua qualidade.</p>  
Responsabilidade das unidades individuais que produzem os dados.

<p align="justify">Capacitar equipes de domínio para assumir a responsabilidade por seus próprios produtos de dados e garantir que os princípios de governança, como qualidade e segurança de dados, sejam respeitados.</p>
  <p align="justify">A organização precisa dar suporte a uma mudança cultural em que as equipes de domínio sejam capacitadas para assumir a propriedade de seus pipelines de dados e entregar dados como um produto.</p><p align="justify">Uma infraestrutura robusta de ferramentas de dados de autoatendimento é essencial, permitindo que as unidades de negócios consumam, analisem e obtenham insights de dados de forma independente.</p>
<p align="justify">O Data Mesh oferece um novo paradigma para cumprir o valor prometido dos dados. Ela rejeita padrões de longa data arquiteturas de dados centralizadas, como o `data lake` e o `data warehouse` e seus associados equipes centralizadas. Em vez disso, ele descentraliza tanto a propriedade dos dados quanto os dados em si, transferindo-os para os domínios funcionais que criam e usam dados para administrar seus negócios.</p>
Seus quatro pilares:

- [ ] **Propriedade de domínio**: Uma equipe de domínio está próxima dos principais processos de negócios, conhece os dados que o domínio produz e as análises que seus stakeholders precisam para resolver problemas e capitalizar oportunidades.
- [ ] **Dados como um produto**: Os produtos de dados consistem em mais do que apenas dados. Eles incluem código para coletar e transformar dados e habilitar acesso gerenciado por meio de APIs. Eles incluem metadados que descrevem o produto, como esquema, semântica e métricas de qualidade.
- [ ] **Plataforma de dados self-service**: As equipes de domínio precisam de uma plataforma de autoatendimento para entregar e gerenciar dados produtos. Eles precisam provisionar infraestrutura de armazenamento e computação, construir, implantar e gerenciar versões de produtos de dados, limpar e transformar dados, fornecer acesso seguro a dados e cumprir políticas e regulamentações.
- [ ] **Governança computacional Federada**: Órgão federado composto por representantes de equipes de domínio e aqueles com responsabilidades globais de dados, como conformidade regulatória e gerenciamento de qualidade. Preocupações comuns, como o que constitui qualidade,classificações de dados e como lidar com diferentes níveis de sensibilidade, modelagem de dados que abrangem domínios e padrões para metadados de produtos de dados.

A malha de dados (Data Mesh) aborda essas dimensões, fundadas em quatro princípios:

- [ ] **Arquitetura de dados descentralizada orientada ao domínio**:
	- [ ] Os diferentes domínios de negocios (produtores de dados) sao responsaveis ​​por curar, validar, publicar, manter e gerenciar o ciclo de vida dos dados que possuem.
	- [ ] Data lakes que são gerenciados centralmente pela TI;
- [ ] **Dados disponibilizados como produto**:
	- [ ] Em um data lake típico, o data lake e os pipelines de dados são o produto. Em uma malha de dados, os dados e o domínio e a expertise do produtor que reúne e publica os dados são o produto.
	- [ ] Cada domínio deve ter um proprietário do produto de dados, responsável por garantir que os dados sejam entregues como um produto.
	- [ ] Qualidade de dados, menor tempo de espera de consumo de dados e, em geral, satisfação do usuário de dados.
	- [ ] Quem são os usuários dos dados;
- [ ] **Infraestrutura para disponibilizar os dados como self-service**: (Plataforma de dados self-service)
	- [ ] Armazenamento de dados escalável;
	- [ ] Esquema de produtos de dados;
	- [ ] Construção e orquestração de pipeline de dados;
	- [ ] Linhagem de dados;
- [ ] **Controle de acesso granular e escalável**
	- [ ] Os produtores especificam políticas de acesso, governança e retenção e quaisquer políticas de acesso personalizadas com base na granularidade dos dados.
	- [ ] Interoperabilidade por meio de padronização global,
	- [ ] Topologia dinâmica;
## Quais ferramentas:

- [ ] Dataflow:
- [ ] Google Cloud Dataflow
- [ ] AWS Data Pipeline/AWS Glue/Amazon Kinesis Data Streams
- [ ] Azure Data Factory/Azure Stream Analytics
- [ ] Oracle Cloud Data Flow
- [ ] Snowflake Data Cloud
- [ ] Apache Kafka
- [ ] Apache Nifi
- [ ] Apache Airflow e porque não Rundeck.
- [ ] Data Catalog:
- [ ] [Google Cloud Data Catalog](https://cloud.google.com/data-catalog/docs/concepts/overview?hl=pt-br)
- [ ] [Microsoft Azure Purview](https://learn.microsoft.com/pt-br/purview/purview)
- [ ] [DataHub](https://datahubproject.io/)
- [ ] [Metacat](https://github.com/Netflix/metacat)
- [ ] [Egeria](https://egeria-project.org/)
## Por onde começar?

- [ ] Mapeie os domínios da sua organização;
- [ ] Avalie os impulsionadores do negócio e comece pequeno;
- [ ] Defina padrões de produtos de dados;
- [ ] Atribuir proprietários de produtos de dados;
- [ ] Crie a plataforma de dados de autoatendimento;
## Definida onde queremos

- [ ] Defina uma estratégia de dados;
- [ ] Qual é a natureza dos dados?
- [ ] Diferenciar informações sensíveis (como dados de clientes ou funcionários) de informações não sensíveis (como informações de produtos).
- [ ] Quando os dados foram criados ou alterados?
- [ ] Quem realizou operações nos dados?
- [ ] Por que esses dados estão sendo armazenados? (Dados pessoais devem ser armazenados apenas para um propósito comercial legítimo.)
- [ ] Quanto tempo esses dados estão sendo armazenados?
- [ ] Como esses dados estão sendo usados?
- [ ] Descrever todos os aplicativos que têm dependência desses dados.
- [ ] Desenvolver um modelo de governança;
- [ ] Avalie a maturidade do Agile e do DevOps;
- [ ] Plataformas de design e padrões técnicos.
# Gerenciamento de Dados
<p align="justify">É uma estratégia usada por organizações para tornar os dados seguros, eficientes e disponíveis para quaisquer propósitos comerciais relevantes.</p>
<p align="justify">Gerenciamento de dados se refere tanto a processos quanto a tecnologia. Processos são geralmente definidos pela estrutura de governança de dados da organização, e cada um desses processos é implementado com as ferramentas de software relevantes.</p>

## Estratégia de Gerenciamento de Dados

### Definição

- [ ] Resumo da estratégia corporativa e de negócios;
- [ ] Níveis de maturidade atuais e desejados da análise de dados;
- [ ] Visão, missão e valores da análise de dados;
- [ ] Objetivos estratégicos e KPIs para atingir nossa visão;
- [ ] Equipe e orçamento;
- [ ] Princípios orientadores.
### Maturidade

- [ ] Gerenciamento e infraestrutura de dados;
- [ ] Qual/is as fontes e aquisição de dados?
- [ ] Como avalio a qualidade e limpeza de dados?
- [ ] Como são as soluções de armazenamento e processamento de dados?
- [ ] Como faço a Integração, Transformação e Disponibilização?
- [ ] Como faço a escalabilidade e desempenho da infraestrutura de dados?
- [ ] Quais são as Tecnologias em gestão e infraestrutura de dados?
- [ ] Como posso avaliar se a implementações foi/esta bem-sucedida?
- [ ] Governança e conformidade de dados
- [ ] Como a governança de dados permite que uma organização se torne orientada por dados?
- [ ] Como DIVIDIR, os dados e dividir a responsabilidade da governação de dados?
- [ ] Como tratar a questão da privacidade e segurança de dados?
- [ ] Como gerir a conformidade de dados?
- [ ] Como estabelecer a definição de ética de dados e seu uso responsável?
- [ ] Como implementar a governança e conformidade de dados?
- [ ] Ferramentas e técnicas de análise;
- [ ] Como padronizar e estabelecer o uso de ferramentas e técnicas de visualização de dados?
- [ ] Como padronizar e estabelecer o uso de modelos e técnicas de análise estatística?
- [ ] Como padronizar e estabelecer o uso de Ferramentas e técnicas de Machine learning?
- [ ] Como padronizar e estabelecer o uso de Ferramentas e técnicas de big data?
- [ ] Como padronizar e estabelecer o uso de Ferramentas e técnicas de preparação de dados?
- [ ] Como padronizar e estabelecer o uso de Matriz de seleção de ferramentas analíticas?
- [ ] Organização orientada a dados
- [ ] Como posso afirmar, que a organização ESTÁ orientada À dados?
- [ ] Como posso construindo uma cultura baseada em dados na organização?
- [ ] Como podemos criar uma infraestrutura de dados fácil de usar, consumir e distribuir?
- [ ] Como podemos fomentar a experimentação e a inovação, com os Dados?

| Dimensão                                | Emergente - Nível 1 | Pré-Adoção Nível 2 | Areas - Nível 3 | Corporativa- (Nível 4) | Maduro - (Nível 5) |
| --------------------------------------- | ------------------- | ------------------ | --------------- | ---------------------- | ------------------ |
| Governança e conformidade de dados      |                     |                    |                 |                        |                    |
| Gerenciamento e infraestrutura de dados |                     |                    |                 |                        |                    |
| Ferramentas e técnicas de análise       |                     |                    |                 |                        |                    |
| Organização orientada a dados           |                     |                    |                 |                        |                    |
#### Estratégia de Dados

| Estratégia   | Entenda                                                                                                                                                                                                                                                                                                                                                          |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ingestão     | Os dados devem ser adquiridos de fontes confiáveis, como bancos de dados de produção ou terceiros confiáveis.                                                                                                                                                                                                                                                    |
| Data Lineage | Linhagem de dados é o nome de um tipo específico de metadados que contém o histórico completo de seu assunto. Metadados de linhagem descrevem a origem dos dados aos quais se referem e fornecem detalhes de quaisquer operações desde o início. A linhagem de dados funciona como um tipo de changelog para esses dados, registrando cada operação que ocorreu. |
| Acesso       | Supervisionar a criação de funções de usuário e garantir que cada usuário receba acesso de leitura e gravação apropriados.                                                                                                                                                                                                                                       |
| Integração   | Processo de pegar dados de várias fontes diferentes e agrupá-los em um único local. Processos: ETL, ELT, ETLT.                                                                                                                                                                                                                                                   |
|              | Validação : verificar a precisão dos dados comparando-os a um esquema.                                                                                                                                                                                                                                                                                           |
|              | Consolidação : centralizar o armazenamento de dados para melhorar a eficiência ou armazenar big data de forma mais econômica.                                                                                                                                                                                                                                    |
|              | Habilitação de processo: novo processo que só é possível com uma fonte de dados integrada.                                                                                                                                                                                                                                                                       |
|              | Gerenciamento de dados mestres (MDM) : técnicas de integração para produzir dados mestres.                                                                                                                                                                                                                                                                       |
|              | Análise e inteligência empresarial (BI) : fonte de dados unificada para fins de análise, bem como outras aplicações de BI.                                                                                                                                                                                                                                       |
| Metadados    | Reunir e indexar metadados relevantes, e que esses metadados estejam disponíveis quando necessário.                                                                                                                                                                                                                                                              |
| Conformidade | Gerenciamento de dados deve refletir todos os requisitos regulatórios e garantir que a organização permaneça no lado certo da lei. (LGPD (Regulamento Geral de Proteção de Dados), PCI DSS (Padrão de Segurança de Dados do Setor de Cartões de Pagamento), HIPAA (Portabilidade e Responsabilidade de Seguro Saúde)) e SOX (Sarbanes-Oxley)                     |
| Análise      | análises para impulsionar suas tomadas de decisão. uporte aos esforços do tempo de análise e garantir que os dados disponíveis sejam oportunos, relevantes e completos.                                                                                                                                                                                          |
| Segurança    | Gerente de dados é responsável por trazer problemas de segurança à tona e também por organizar auditorias e testes regulares.                                                                                                                                                                                                                                    |
| Arquivamento | Recomendará soluções preferenciais para que a organização tenha uma abordagem unificada para armazenamento de dados de longo prazo.                                                                                                                                                                                                                              |
| Eficiência   | Revisar regularmente sua estratégia de gerenciamento de dados para perguntar se a abordagem atual é econômica e sustentável.                                                                                                                                                                                                                                     |
| Escala       | gerenciamento de dados deve planejar escalar facilmente quando necessário.(ex."IoT,Logs)                                                                                                                                                                                                                                                                         |
### BuzzWord - Organizacional e Estratégia de IA

<div class="mdx-columns2" markdown>

- [x] Resumo da estratégia corporativa e de negócios

- [x] Fundamentos da IA

- [x] Níveis de maturidade atuais e DESEJADOS da IA

- [x] Visão, missão e valores da IA

- [x] Objetivos estratégicos e KPIs para atingir nossa visão

- [x] Princípios orientadores

- [x] Centro de dados de IA

- [x] Machine Learning/Deep Learning

- [x] NLP(Natural Language Processing) & Prompt Engineering

- [x] Equipe e Orçamento

</div>

#### Delivery e Responsibility

<div class="mdx-columns2" markdown>

- [x] Estratégia de gerenciamento de mudanças

- [x] Planos de gerenciamento de mudanças

- [x] Avaliação pós-programa/projetos mudanças e como reuno(PDCA) lições aprendidas

- [x] Análise dos stakeholders

- [x] Estratégia de engajamento dos stakeholders

- [x] Plano detalhado de engajamento dos stakeholders

</div>

  
  

```mermaid

flowchart LR

A(Meus Dados</br>são...) -->|Dados| B{Regulamentados}

B --> |Sim| C(PCI DSS) & D(LGPD) & E(HIPAA) & F(SOX)

B --> |Não| G{Retível?}

G --> H{Necessita</br>Criptografia?}

H --> |Sim| H0(Criptografa)

H --> H1(Tag de</br>Retenção)

H0 --> H1 --> RETER[(Retenção)]

C --> H0 --> ARQUIVA[(Arquiva)]

D --> H0

E --> H0

F --> H0

```

  

## Data Mesh vs. Data Fabric

- [ ] Data Fabric é uma solução centralizada e orientada por tecnologia, que visa criar uma plataforma unificada para gerenciar e acessar dados onde quer que eles residam.
- [ ] Data Mesh, por outro lado, descentraliza os dados e sua propriedade.
- [ ] Em um data mesh equipes individuais ou unidades de negocios sao responsaveis ​​por seus próprios dados e sao encarregadas de criar produtos de dados, para seu proprio consumo e presumivelmente o consumo de outros na organizacao.

## Dados Links
### Linhagem de Dados

<div class="mdx-columns2" markdown>

- [x] [SAS](https://www.sas.com/)

- [x] [Informática](https://www.informatica.com/)

- [x] [Octopai](https://www.octopai.com/) Adquirida recentemente pela [Cloudera](https://www.cloudera.com/about/news-and-blogs/press-releases/2024-11-14-cloudera-to-acquire-octopais-platform.html)

- [x] [Datahub](http://datahub.io/)

</div>

### Dados Abertos

<div class="mdx-columns2" markdown>

- [x] [Microdados ENEM](http://portal.inep.gov.br/microdados)

- [x] [Portal Brasileiro de Dados Abertos](http://dados.gov.br/)

- [x] [NASA](http://data.nasa.gov/)

- [x] [The World Bank](http://data.worldbank.org/)

- [x] [United States Government](http://www.data.gov/)

</div>

  

![](../img/data-engenharia.png)

# Conceitos

## Fundamentais

- [ ] Modularidade: Deve ser construída com componentes independentes que se integram facilmente, promovendo flexibilidade e escalabilidade.
- [ ] Data as a Product: Cada conjunto de dados é tratado como um produto, com “donos” responsáveis, SLAs definidos e interfaces claras para consumo.
- [ ] Interoperabilidade: Capaz de suportar diferentes tecnologias e padrão para facilitar integração.
- [ ] Replicabilidade: Processos como ingestão de dados, transformação e monitoramento devem ser automatizados para reduzir erros e aumentar a eficiência.
- [ ] Segurança e Governança: Proteção de dados, rastreabilidade e conformidade regulatória são fundamentais e não podem ficar de fora.
## Componentes Importantes  

- [ ] Sources: Pontos de origem dos dados, como bancos de dados transacionais, APIs, logs.
- [ ] Ingestion: Ferramentas para capturar e transferir dados de fontes para ambiente de armazenamento.
- [ ] Storage: Foco em armazenamento de dados em formatos brutos e também estruturado e otimizado para análises.
- [ ] Processing: Processamento em lote (batch) e em tempo real (streaming).
- [ ] Transformation (ETL/ELT): Preparação e transformação e limpeza dos dados usando pipelines.
- [ ] Governance & Metadata Management: Controle de qualidade, catálogo de dados e gerenciamento de metadados.
- [ ] Orchestration: Coordenação de workflows de dados.
- [ ] Consumption: Interfaces e ferramentas para acessar dados em dashboards.
- [ ] Monitoring & Observability: Rastreamento de desempenho, latência e falhas.
- [ ] Security & Compliance: Criptografia, autenticação (IAM) e controle de acessos.


  # Lakehouse: A convergência de data warehousing, Ciência de Dados e Governança de Dados

Os formatos de arquivo abertos subjacentes, como Parquet e Avro , e as estratégias de otimização de dados em data lakehouses podem fornecer às organizações uma vantagem competitiva em governança de dados, análise de dados e ciência de dados.

  

- [ ] Data Warehouse é projetado para armazenar dados refinados, estruturados e relacionais com um esquema projetado no início. Onde os dados são armazenados em um formato estruturado.

- [ ] Data lake é projetada para armazenar dados não estruturados, não refinados e não relacionais com um esquema projetado no final. Usado principalmente para ciência de dados e análises avançadas para aprendizado de máquina e IA, pois permite a conexão de vários tipos de dados de diversas fontes.

  

![](img/data_lakehouse.png){width="650" height="950" style="display: block; margin: 0 auto"}

  

Arquiteturas de data lakehouse podem atingir a conformidade com ACID ( atômica, consistente, isolamento e durabilidade ) na presença de leitores e escritores simultâneos, aproveitando formatos de arquivo como [ORC , Parquet e Avro](https://www.astera.com/pt/type/blog/avro-vs-parquet-is-one-better-than-the-other/).

  

ORC e ​​Parquet usam um formato de armazenamento em colunas, permitindo acesso e modificação eficientes de colunas específicas, mantendo a integridade dos dados por meio de arquivos de metadados.

  

Avro é um formato popular de serialização de dados que pode ser usado para definir a estrutura de dados armazenada em um formato em colunas , como Parquet ou ORC , permitindo armazenamento e recuperação de dados mais eficientes.

  

Os data-frames oferecem uma abstração de tabela com vários operadores de transformação, muitos dos quais são mapeados para álgebra relacional.

  

Os data lakehouse é sua conformidade com o ACID , que complementa a governança de dados e os regulamentos de privacidade (por exemplo, gerenciamento de dados mestres (MDM), GDPR) ao fornecer uma maneira confiável e eficiente de atualizações e exclusões em nível de registro.

  

A arquitetura do data lakehouse difere dos sistemas tradicionais de data lake e warehouse porque inclui metadados, cache e camadas de indexação sobre o armazenamento de dados.

  

Da perspectiva comercial, Delta Lake, Iceberg e Hudi(Hadoop Upsert/Delete/Increment) são três tecnologias populares de data lakehouse que oferecem vários benefícios para armazenamento e processamento de dados.

  

O Hive LLAP ( Low Latency Analytical Processing ) também pode ser usado como um data lakehouse armazenando dados em um sistema de armazenamento baseado em nuvem ou Hadoop e criando tabelas no Hive que mapeiam os dados.

  

![](img/datalakehouse.png)

  

## Data Warehouse x Data Lake x Data Lakehouse: Visão Geral

  

| Tipo de solução                           | Data warehouse                                                     | Data lake                                                      | Data lakehouse                                                        |
| ----------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------------- | --------------------------------------------------------------------- |
| Tipo de dados                             | Dados estruturados                                                 | Estruturado, semiestruturado, não estruturado                  | Estruturado, semiestruturado, não estruturado                         |
| Qualidade dos dados                       | Dados altamente selecionados e confiáveis, segurança de alto nível | Dados brutos, baixa qualidade                                  | Dados brutos e estruturados, alta qualidade e alto nível de segurança |
| Em processamento                          | ETL — extrair, carregar, transformar                               | ELT – extrair, transformar, carregar                           | Tanto ETL quanto ELT                                                  |
| Política de preços                        | O armazenamento é caro                                             | O armazenamento é econômico e facilmente escalonável           | O armazenamento é econômico e facilmente escalonável                  |
| Conformidade com ACID Compatível com ACID | Não compatível com ACID                                            | Compatível com ACID                                            |                                                                       |
| Análise                                   | BI, relatórios                                                     | Análise avançada – aprendizado de máquina, análise de big data | Análise avançada, BI e outros tipos de fluxos de trabalho analíticos  |
| Usuários                                  | Equipes de BI, relatórios e dados                                  | Cientistas de dados e engenheiros de dados                     | Cientistas de dados e engenheiros de dados                            |

  

# Change Data Capture (CDC)

Para tirar vantagem, as organizações de TI precisam primeiro reinventar a forma como movem, armazenam, processam e analisam dados.

E os desafios são reais.
Os trabalhos de replicação em lote e os procedimentos manuais de script de extração, transformação e carregamento (ETL) são lentos e ineficientes.

  

https://debezium.io/

As alterações feitas em um registro específico em um banco de dados e permitem que os consumidores de eventos tomem medidas com base nessas informações, permitindo uma ampla gama de casos de uso , como ETL em tempo real (propagando os dados atualizados em armazenamentos de dados downstream, como data warehouses, bancos de dados analíticos ou índices de pesquisa de texto completo), troca de dados de microsserviços ou registro de auditoria.

  

| Evento                   | Entenda                                                                                                                                                 |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Completos                | Sempre que algo muda em um registro em um armazenamento de dados de origem, esse evento de alteração conterá o estado completo desse registro.          |
| Delta                    | Eles não contêm o estado completo do registro representado, mas apenas aquelas colunas ou campos cujo valor realmente mudou, bem como o id do registro. |
| Somente de identificação | Eles apenas descrevem qual registro no banco de dados de origem foi afetado por uma alteração.                                                          |

Observação: as ferramentas CDC emitem eventos de alteração de forma assíncrona, o que significa que, no momento em que você executa uma consulta para obter o estado completo da linha, essa linha pode já ter sido mutada novamente.
  
![](img/cdc_por_tipo.png)

  ## Metadados do Evento
* O tipo de uma alteração (inserir, atualizar, excluir)
* Carimbo de data e hora em que o evento ocorreu
* Nome do banco de dados, esquema e tabela de origem
* ID da transação
* Posição do evento no log de transações do banco de dados de origem
* A consulta que desencadeia uma alteração

  

# Testes de Migração de Dados

É um esforço que garante uma transição perfeita de um sistema legado para um novo com interrupção mínima e sem perda ou corrupção de dados. Ele verifica se os dados atuais, bem como os novos dados, serão manipulados corretamente pelos aspectos funcionais e não funcionais do seu aplicativo. Portanto, você deve garantir que:

  

* Os dados existentes chegam à nova estrutura sem perda ou corrupção;

* Os aplicativos legados e novos estão funcionando corretamente em relação à "nova" estrutura do banco de dados (assumindo que os aplicativos legados estarão em uso na produção após a migração, o que é provável);

* Cumpra as leis aplicáveis ​​sobre privacidade e proteção de dados (GPDR/LGPD): Consulte seu gerente de produto ou stakeholders e, se necessário, a equipe DPO da organização para determinar se a migração de dados envolve quaisquer dados de usuário regulamentados e se etapas adicionais precisam ser tomadas.

* Os usuários devem conseguir acessar todos os recursos do software sem problemas após a conclusão da migração.

* Você quer evitar qualquer inconveniência para os usuários do sistema, sejam eles clientes B2C ou funcionários de organizações que usam o sistema.

  

## Desafios da migração de dados

  

* Manipulando grandes conjuntos de dados

* Garantindo a consistência dos dados

* Abordando possíveis bugs que surgem durante a migração do sistema

* Dados em mais de um conjunto de caracteres

* Migrando dados e introduzindo novos recursos ao mesmo tempo

* Ofuscação adequada de dados de identificação pessoal do usuário

* "Mobilidade" de um conjunto de dados que contém dados de usuário e IDs de usuário ofuscados

  

## Estratégia de teste de migração de dados

  

* Auditoria Pré-migração: **Examine** os dados em sistemas legados e tabelas de banco de dados para identificar problemas como inconsistências, duplicatas, corrupção ou incompletude. Isso pode evitar complicações durante a migração real na produção e ajuda a preparar dados de teste realistas.

* Teste de compatibilidade : **Garanta** a compatibilidade com dados e recursos existentes;

* Teste de reversão : **Valide** a capacidade de reverter para o banco de dados legado, se necessário;

* Validação de dados pós-migração : **Confirme** se todos os dados foram migrados, estão no formato esperado e funcionam conforme o esperado no novo ambiente;

* Verifique se os recursos e sistemas funcionam com os dados migrados conforme o esperado.

* Teste as interfaces entre os dados migrados em aplicativos e outros serviços com os quais eles interagem.

* Teste o desempenho para garantir que ele esteja no mesmo nível (ou seja, mais rápido que) o do sistema legad

* **Execute** testes estáticos e funcionais em cada ambiente de teste;

* **Verifique** se os dados parecem bons, se tudo funciona e se não há travamentos em cada preparação separadamente.
