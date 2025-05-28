SAP FIori não era da SAP e passou a ser do SAP FIori - Ele é, na verdade, **uma abordagem de design de interface e uma coleção de aplicações SAP com foco na experiência do usuário**.

- O **SAP Fiori Launchpad** é a **plataforma de acesso central** onde os usuários veem e acessam suas Fiori Apps.
- Parece uma tela inicial com **ícones (tiles)** para cada aplicativo que o usuário tem permissão para usar.
- Personalizável por perfil, cargo e preferência do usuário.

|Termo|O que é?|Exemplo|
|---|---|---|
|**SAP Fiori**|Conjunto de apps com design moderno|App para aprovar pedidos de compra|
|**Fiori Launchpad**|Portal web com acesso aos apps|Tela inicial com todos os tiles (ícones) de apps disponíveis|

Transações Fiori nativas e transações Fiorizadas (fioriappslibrary.hana.ondemand.com/sap/fix/externalViewer/)


O SAP HANA é um banco de dados em memória, com armazenamento em colunas, projetado para alto desempenho.  _Todos os dados são compactados e mantidos na memória, o que permite_ a execução de operações em grandes volumes de dados sem acessar o disco, evitando gargalos de entrada/saída.

O dimensionamento do hardware é complexo e muitos fatores precisam ser considerados. O fator de crescimento é especialmente difícil de mensurar e é fácil cometer erros.
_Se for superestimado, recursos caros não serão_ utilizados, resultando em um custo total de propriedade (TCO) excessivo.

_O RISE with SAP inclui diferentes componentes do SAP BTP e SAP Business Network para


| Característica       | **RISE with SAP**             | **GROW with SAP**                 |
| -------------------- | ----------------------------- | --------------------------------- |
| Público-alvo         | Grandes empresas / legadas    | Empresas médias / em crescimento  |
| Tipo de nuvem        | Privada ou pública            | Nuvem pública (public cloud)      |
| ERP incluído         | SAP S/4HANA (qualquer edição) | SAP S/4HANA Cloud, public edition |
| Abordagem            | Transformação / migração      | Adoção rápida / Greenfield        |
| Customização         | Alta                          | Limitada (pré-configurado)        |
| Tempo de implantação | Médio a longo                 | Curto (mais rápido)               |
| Custo                | Mais elevado                  | Mais acessível                    |

A assinatura RISE with SAP inclui não apenas o SAP S/4HANA Cloud, edição privada, mas também a infraestrutura do hyperscaler e uma gama de serviços de gerenciamento técnico que a SAP fornece mediante um acordo de nível de serviço (SLA) previamente acordado. Inclui também os tickets de consumo para SAP BTP, o pacote inicial do SAP Business Network para SAP S/4HANA, o SAP Signavio Process Insights e o SAP Process Intelligence. Aqui está uma breve descrição desses diferentes componentes:

|Processo|Nome em inglês|Função principal|Área principal|
|---|---|---|---|
|Projeto para Operação|Project to Operate|Planejar e executar projetos|PM, PS, CO|
|Registro para Relatório|Record to Report|Contabilidade e relatórios financeiros|FI, CO|
|Lead-to-Cash|Lead to Cash|Vendas até recebimento|SD, FI|
|Fonte para Pagamento|Source to Pay|Compras até pagamento|MM, FI|
|Recrutar para Aposentar|Recruit to Retire|Ciclo de vida do funcionário|HCM, SuccessFactors|
|Solicitação de Serviço|Request to Service|Gerenciar e executar solicitações de serviço|CS, ITSM|
PMW -


| Fase SAP Activate         | Mês | % Esforço Planejado (acumulado) |     |
| ------------------------- | --- | ------------------------------- | --- |
| Discover (Descoberta)     | 1   | 5%                              | 5   |
| Prepare (Preparação)      | 2   | 15%                             | 10  |
| Explore (Exploração)      | 3   | 35%                             | 20  |
| Realize (Realização)      | 4   | 70%                             |     |
| Deploy (Implantação)      | 5   | 90%                             |     |
| Run (Suporte pós go-live) | 6   | 100%                            |     |


| Característica                         | Oracle E-Business Suite (EBS) | Oracle Fusion Applications        | SAP (S/4HANA)                     |
| -------------------------------------- | ----------------------------- | --------------------------------- | --------------------------------- |
| **Modelo de Dados Organizacionais**    | Multi-Org                     | Enterprise Structures             | Enterprise Structure / Org Units  |
| **Separação Legal/Fiscal**             | Legal Entity                  | Legal Entity                      | Company Code                      |
| **Unidade Operacional Principal**      | Operating Unit                | Business Unit                     | Plant / Company Code / Org Units  |
| **Controle Contábil**                  | Set of Books / Ledger         | Primary Ledger / Secondary Ledger | Ledger / Chart of Accounts        |
| **Centro de Lucro ou Custo**           | Cost Center / OU              | Cost Center / Business Unit       | Cost Center / Profit Center       |
| **Hierarquia Flexível (multiempresa)** | Limitada (via Multi-Org)      | Sim (com estrutura unificada)     | Sim (com Company Codes + Orgs)    |
| **Modelo Cloud-Ready**                 | Não (on-premise)              | Sim (nativamente Cloud)           | Sim (S/4HANA Cloud ou on-premise) |

|Função / Conceito|Oracle EBS|Oracle Fusion ERP|SAP S/4HANA|
|---|---|---|---|
|Entidade legal|Legal Entity|Legal Entity|Company Code|
|Unidade de operação|Operating Unit|Business Unit|Plant, Sales Org|
|Unidade contábil|Ledger|Ledger|Ledger / Chart of Accts|
|Controle de custo/lucro|OU / Cost Center|BU / Cost Center|Cost Center / Profit Ctr|
|Unidade de estoque|Inventory Org|Inventory Org|Plant|
|Gerenciamento centralizado|Limitado|Sim|Sim|


Ledger (Set of Books)
└── Legal Entity
    └── Operating Unit (OU)
        └── Inventory Organization(s)


Client
└── Company Code
    └── Plant
        └── Storage Locations


| Função / Conceito        | Oracle EBS / Fusion    | SAP S/4HANA        |
| ------------------------ | ---------------------- | ------------------ |
| Entidade de estoque      | Inventory Organization | Plant              |
| Local interno de estoque | Subinventory / Locator | Storage Location   |
| Transações de estoque    | Sim                    | Sim                |
| Integração com produção  | Sim (WIP / MFG)        | Sim (PP / MRP)     |
| Contabilidade de estoque | Por Org. de Inventário | Por Valuation Area |



| **Company Code** | Valor do material é igual em todas as plantas da empresa. |
| ---------------- | --------------------------------------------------------- |
| **Plant**        | Valor do material pode variar de planta para planta.      |
|                  |                                                           |
Na maioria das implementações modernas (especialmente no **S/4HANA**), a **Valuation Area por Plant** é **obrigatória**, pois permite maior controle.

## Clean Core
Clean Core é um conceito, gestão do ciclo de vida da aplicação.

- [ ] Política de controle de modificações: **Evitar modificações no código-fonte do SAP S/4HANA**.
- [ ] Remoção de código obsoleto: **Eliminar código não utilizado ou redundante**.
- [ ] Uso de APIs: **Dar prioridade no uso de APIs para extensões e integrações**.

### PAAS (Plataform as a Service)

**Extensibilidade de Usuário-chave (In-App Key-user Extensibility)**: Possibilita fazer extensões e customizações dentro do SAP S/4HANA, usando aplicações Fiori. Apesar do nome ser Key-User Extensibility, essa é uma opção de extensibilidade mais direcionada a consultores funcionais e desenvolvedores, podendo ser feita por usuários-chave que tenham mais domínio técnico do SAP. Possibilidades dessa extensibilidade:

- [ ] Adaptar telas do SAP Fiori.
- [ ] Adicionar lógica e campos customizados.
- [ ] Criar análises personalizadas.
- [ ] Criar formulários e modelos de e-mail.
- [ ] Criar objetos de negócios customizados.

**Extensibilidade do Desenvolvedor SAP BTP (Side-by-Side Developer Extensibility)**: Possibilita a criação de extensões e customizações maiores e mais complexas, para isso são utilizados serviços disponíveis no SAP Business Tecnology Plataform, os desenvolvimentos feitos aqui estão desacoplados do S/4HANA, portanto, mantendo o core do sistema limpo. Possibilidades dessa extensibilidade:

- [ ] Criar aplicações personalizadas.
- [ ] Desenvolver aplicativos móveis.
- [ ] Implementar soluções de IoT e Big Data.
- [ ] Implementar soluções de inteligência artificial.

**Extensibilidade do Desenvolvedor - In-App (On-Stack Developer Extensibility)**: Possibilita a criação de extensões e customizações maiores e mais complexas, neste caso usando ABAP Cloud - On-Stack, desenvolvendo dentro do próprio S/4HANA, desta maneira não é necessário o SAP BTP. Mesmo desenvolvendo dentro do S/4HANA, existem regras e validações que garantem a cumprimento dos princípios do Clean Core. Possibilidades dessa extensibilidade:

As possibilidades são quase as mesmas da Extensibilidade do Desenvolvedor - SAP BTP (Side-by-Side Extensibility), entretanto algumas delas são mais seguras e performáticas se criadas no SAP BTP.
- [ ] Criar aplicações personalizadas.
- [ ] Desenvolver aplicativos móveis (recomendado no SAP BTP).
- [ ] Implementar soluções de IoT e Big Data (recomendado no SAP BTP).
- [ ] Implementar soluções de inteligência artificial (recomendado no SAP BTP).

## Business Technology Platform - PAAS (Plataform as a Service)

| Model   | Descricao |
| ----    | ---- |
| App Dev | Foco total em desenvolvimento de aplicações, aqui estão serviços como: SAP Build Apps, SAP Build Workzone, SAP Build Code, entre outros. |
| Automation | Foco total em automatização e workflows, aqui estão serviços como: SAP Build Process Automation, SAP Task Center, entre outros. |
| Integration | Foco total em integração entre sistemas e aplicações, aqui estão serviços como: SAP Integration Suite, SAP Business Accelerator Hub, entre outros. |
| Data and Analytics | Foco total em extração, tratamento e análises de dados e indicadores, aqui estão serviços como: SAP Datasphere, SAP Analytics Cloud, entre outros. |
| Artificial Intelligence | Foco total em desenvolvimento de aplicações com uso de inteligência artificial, aqui estão serviços como: SAP AI Core, SAP AI Launchpad, entre outros. |

## Core Data Services (CDS)
Os CDSs são usados para criar estruturas de dados complexas, views e interfaces de serviço que podem ser consumidas por aplicativos Fiori e outros componentes do S/4HANA.

### Code Pushdown
Mover a lógica de processamento de dados para o nível do banco de dados.
Os CDSs facilitam isso ao permitir que operações complexas sejam definidas e executadas diretamente no banco de dados, reduzindo a quantidade de dados transferidos e melhorando significativamente o desempenho das aplicações.

#### CDSs em comparação com as views ABAP tradicionais
Melhor desempenho devido ao processamento no nível do banco de dados
Reutilização mais fácil em diferentes contextos (analítico, transacional)
Capacidade de incluir anotações para metadados e comportamentos
Integração mais simples com ferramentas de desenvolvimento SAP modernas
Suporte nativo para criação de serviços OData
