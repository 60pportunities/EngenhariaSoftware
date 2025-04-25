“Modernizando dados com propósito estratégico” é um relatório do MIT Technology Review Insights patrocinado pela Thoughtworks.

Os dados se tornaram um componente cada vez mais crítico para o sucesso dos negócios.

Com todos esses elementos implementados, as organizações podem garantir que serão sempre capazes de gerar valor a partir dos dados com velocidade e escala, independentemente da evolução dos seus requisitos de governança e demandas de dados.
## Diversos benefícios para o negócio

- [ ] Prover dados relevantes e confiáveis para o negócio;
- [ ] Construir uma Base única de verdade;
- [ ] Melhorar o COMPLIANCE da Organização;
- [ ] Apoiar o desenvolvimento de modelos de IA está entre os principais motivos pelos quais as organizações incluídas na nossa investigação procuram modernizar as suas capacidades de dados.
## Problemas Diversos

- [ ] Chamados negados e sem transparencia para o Cliente (Ocorre principalmente no início de cada mes);

```
Problema na identificacao da Instancia do Bem do CONTRATO: XXXXX.XXXX e AGENCIA/SAG: 9999.XX. NAO localizado instancia válida com parametros:
Favor, cadastrar/corrigir a instancia no modulo XXX do XXXXXXXXXXXXX.
```

- [ ] Notas Fiscais Denegadas;

```
A Inscrição Estadual do XXXXX foi desativada pela SEFAZ (XXXX atuando para regularização), não podemos emitir NFe do XXXX e contra o XXX, são todas denegadas.
```

- [ ] Consultoria exige a PDM (Padronização da Descrição do Material)

```
Necessidade em se Padronizar a Descrição de Material
Necessidade em se adotar critérios para o cadastramento de NCM
```

- [ ] Erros logísticos e/ou financeiros (pesos indevidos, endereços desatualizados);
- [ ] Autuação Fiscal;
- [ ] Calculo Incorreto de Impostos.
### Classificação dos Dados

- [ ] **Dados Mestres (Master Data)**: Descrevem locais (estabelecimentos), entidades (pessoas (funcionários, parentescos, prestadores de serviço, temporários), clientes, fornecedores, instituição) e coisas que fazem parte de um contexto empresarial.

| Tipo         | Exemplo                                                     |
| ------------ | ----------------------------------------------------------- |
| Cliente      | Dados do Cliente                                            |
| Financeiro   | Grupos contábeis, Ativos, Hierarquias de contas             |
| Governança   | Dados que dão suporte à privacidade, Regulamentações        |
| Instituição  | Dados da Instituição, estruturação                          |
| Funcionários | Dados sobre o funcionário , salários, funções e hierarquia. |
| Produto      | Descrições de produtos, Part-Number e etc.                  |

- [ ] **Dados de Referência (Reference Data)**: São um conjunto de valores ou esquemas de classificação que servem de apoio a um dado mestre.
- [ ] **Dados de referência externos**: APIs conectam os dados de referência a autoridades regulatórias externas, como agências governamentais ou conversores de moeda. Os dados recebidos são classificados e selecionados para se alinharem com os dados mestres estabelecidos.
- [ ] **Dados de referência interna**: As definições e categorias permanecem relevantes para os processos de negócios atuais e atendem às necessidades de todas as disciplinas de negócios. Garanta que os administradores de dados permaneçam consistentes na criação e no gerenciamento de dados de referência.
- [ ] **Dados transacionais**: São as informações operacionais cotidianas em seus bancos de dados de CRM, ERP e HCM. Como por exemplo: Notas Fiscais, Ordens de Compra, Lançamentos Financeiros e etc.
- [ ] **Dados não estruturados**: São dados de postagens em mídias sociais, e-mails, white papers ou chats de ajuda que são difíceis de categorizar.
## Estilos de implementação do Master Data Management (MDM)

| Estilo           | Entenda                                                                                                           |
| ---------------- | ----------------------------------------------------------------------------------------------------------------- |
| **Centralizado** | Em um estilo centralizado, os ERPs/CRMs criam os dados mestres e os dissemina para outros sistemas ou aplicações. |
| **Consolidação** | Criação de um **golden records**, os sistemas de origem alimentam dados em um hub central para golden records.    |
| **Coexistência** | Cria um hub de dados consolidado que então alimenta registros atualizados de volta para as fontes.                |
### Por que achamos de suma importância?
Tem que ser um espécie de protocolo de comunicação que traz diversos benefícios e oportunidades, como seguem:

- [ ] Precisão na identificação do Gestor do Dado;
- [ ] Organizar as informações cadastrais, documentação e contratos (formato, tipo e etc);
- [ ] Minimizar erros operacionais e não conformidades;
- [ ] Conter custos operacionais;
- [ ] Viabilizar sistemas de resposta rápida;
- [ ] Melhorar a acurácia das informações;
- [ ] Unificar as empresas, sistemas e catálogos;
- [ ] Auxiliar nas incorporações e consolidações de estoques;

Quando avaliamos a qualidade de nossos cadastros precisamos construir métricas, que permitam entender o atual cenário dos nossos dados.

- [ ] **VALIDADE E CONFORMIDADE** : A validade determina se o valor preenchido corresponde ao padrão do campo. Isto é, por exemplo, teremos, apenas, valores monetários no campo “Renda”.
- [ ] **DUPLICIDADE**: Acontece quando dois ou mais registros apontam para a mesma entidade real.
- [ ] **COMPLETUDE**: É um indicador, que pode ser expresso em percentual, e indica o quão nosso cadastro está completo para as nossas necessidades.
- [ ] **PRECISÃO E ACURÁCIA**: Usamos acurácia, na avaliação de qualidade de dados, para determinar se aquele dado corresponde a uma entidade real
## Algumas definições

| Definição             | Entenda                                                                                                                                                                                                                                                    |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Elemento de Dados** | É uma unidade de dados, que possui significado preciso ou semântica precisa. Por definição, um elemento de dados é indivisível. Número de conta, um nome, data de nascimento e etc.                                                                        |
| **Domínio de Dados**  | Definido pelo usuário que representa o significado funcional de uma coluna com base nos dados da coluna ou no nome da coluna. Exemplos: número de Previdência Social, número do cartão de crédito e ID de e-mail. (Atributos, Relacionamento e Hirarquia). |
| **Metadados**         | São dados que fornecem informações sobre outros dados.                                                                                                                                                                                                     |
## Pontos Chaves

- [ ] Modelo de Dados
- [ ] Qualidade dos Dados
- [ ] Integração
- [ ] Escalabilidade
- [ ] Auditoria
- [ ] Controle de Metadados
- [ ] Workflow

## Padronização da Descrição do Materia;l
### Código de Materiais
Definir as políticas e regras relacionadas à manutenção do cadastro de materiais.
Centralização do cadastramento, abrangência, incorporações, homologação, saneamento dos estoques, gerenciamento de requisitos, processos para controle e auditoria, bem como responsabilidades funcionais.
Em termos da identificação, o princípio mais importante que costumamos destacar no manual PDM é que “a finalidade do código é identificar, e não catalogar”, pois temos constatado que o equivoco mais usual é codificar os materiais por aplicação, no entanto aprendemos que “diferentes aplicações não determinam diferentes códigos”.
Enfim, para identificar corretamente, o código deve possuir os seguintes atributos:

- [ ] **Unicidade**: Apenas um código para cada SKU (Stock Keeping Units, ou unidades distintas mantidas em estoque);
- [ ] **Simplicidade**: Deve ser fácil de compreender e utilizar;
- [ ] **Formato**: Deve ser estruturado, de preferência com uma numeração sequencial automatizada;
- [ ] **Conciso**: Deve ser sucinto e objetivo;
- [ ] **Expansividade**: Deve suportar o crescimento da empresa;
- [ ] **Operacionalidade**: Deve ser prático e robusto;
- [ ] **Versatilidade**: Deve prever suas diversas aplicações;
- [ ] **Estabilidade**: Deve ser perene;
- [ ] **Confiabilidade**: Deve assegurar a identificação esperada.
- [ ] **Classificação UNSPSC (Universal Standard Products and Services Classification)**: Classifica os itens dentro de ramificações, seguindo uma hierarquia de importância numa árvore baseada na natureza dos materiais.
- [ ] Classificação NCM (Nomenclatura Comum do Mercosul): Baseada no "Sistema Harmonizado de Designação e Codificação de Mercadorias" para facilitar as transações entre Brasil, Argentina, Paraguai e Uruguai, estabelecendo tarifas comuns. No Brasil a NCM está conjugada com a tabela de incidência de impostos sobre produtos industrializados (IPI).
