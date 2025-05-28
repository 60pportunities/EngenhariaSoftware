## Moderador
Sejam bem-vindos à reunião de início do projeto para a utilização do Azure-DevOps no desenvolvimento do Sistema hipotético . Hoje, temos uma equipe multidisciplinar reunida para discutir as etapas iniciais e a abordagem geral do projeto. Então vamos comecar?
## Designer de Negócios
Como designer de negócios, estou aqui para garantir que as necessidades dos usuários e dos stakeholders sejam atendidas de forma eficaz. Precisamos entender bem os requisitos e expectativas de todos os envolvidos no sistema. Meu foco será realizar uma série de entrevistas com os usuários finais e stakeholders para entender suas necessidades e expectativas em relação ao sistema. Vou documentar todos os requisitos funcionais e não funcionais para garantir que sejam considerados durante todo o processo de desenvolvimento.
## Scrum Master
Como Scrum Master vou coordenar as atividades e garantir que os entregáveis sejam definidos e cumpridos.Com base nos requisitos que você vai levantar junto ao PO/PM/Stakeholder, eu vou trabalhar na criação do backlog do projeto, que serão priorizadas, estimadas, dividindo-as em sprints para que possamos acompanhar o progresso de forma mais eficiente.
## Arquiteto de Integração
Como arquiteta de integração, meu foco será garantir que todos os componentes do sistema se comuniquem de maneira adequada. Enquanto o backlog estiver sendo criado, vou realizar uma análise detalhada das integrações necessárias para o sistema. Isso inclui integração com sistemas externos e também entre os módulos internos do sistema. Vou garantir que tenhamos uma visão clara das dependências e interfaces, vou utilizar o C4-Model.
## Arquiteto de Dados
Como arquiteto de dados, meu papel é garantir que o sistema tenha uma estrutura sólida para o armazenamento e processamento dos dados. Enquanto a equipe trabalha no backlog e nas integrações, vou começar a projetar a estrutura do banco de dados do sistema. Preciso entender os tipos de dados, a modelagem e definir as regras de negócio relacionadas ao armazenamento e acesso dos dados.
## Arquiteto de Nuvem
Como arquiteta de nuvem, minha responsabilidade é projetar a infraestrutura do sistema na nuvem, garantindo escalabilidade, disponibilidade e segurança. Enquanto o banco de dados está sendo projetado, vou começar a mapear a arquitetura de nuvem necessária para o sistema. Isso inclui a seleção dos serviços de nuvem mais adequados, definição de grupos de recursos e estratégias de escalabilidade.

## Arquiteto de Segurança
Como arquiteto de segurança será garantir que o sistema seja robusto e protegido contra ameaças. Vou trabalhar em conjunto com todos para implementar práticas seguras no processo de desenvolvimento. Como a segurança é uma consideração importante desde o início, vou revisar as definições de segurança para o ambiente de desenvolvimento, garantindo que estejam alinhadas às melhores práticas.

## Arquiteto de Infraestrutura
Como arquiteto de infraestrutura, minha preocupação é criar a base sólida para o sistema operar, cuidando de servidores, redes e outros recursos. Enquanto a arquitetura de nuvem está sendo definida, vou começar a configurar o ambiente de desenvolvimento. Isso inclui a criação de containers/contêiner, redes, entre outros.
## Desenvolvedor
No contexto do projeto as atividades de um desenvolvedor podem incluir:

- [ ] **Análise de requisitos**: O desenvolvedor participa das reuniões iniciais para entender os requisitos funcionais e técnicos do sistema de viagem e deslocamento de trabalho.
- [ ] **Desenvolvimento de funcionalidades**: Com base nos requisitos levantados, o desenvolvedor é responsável por desenvolver as funcionalidades do sistema utilizando a linguagem e frameworks relacionados/definidos.
- [ ] **Integração com o banco de dados**: O desenvolvedor trabalha em conjunto com o arquiteto de dados para integrar as funcionalidades desenvolvidas ao banco de dados, garantindo o correto armazenamento e acesso às informações.
- [ ] **Integração com serviços externos**: O desenvolvedor é comum a integração com serviços externos, como APIs. O desenvolvedor é responsável por realizar essa integração de forma eficiente.
- [ ] **Implementação de segurança**: Em parceria com o arquiteto de segurança, o desenvolvedor deve garantir a implementação das práticas de segurança no código, como validação de entrada de dados, prevenção de ataques de injeção SQL e proteção contra vulnerabilidades conhecidas.
- [ ]  **Testes unitários e de integração**: O desenvolvedor deve escrever testes para garantir a qualidade e integridade das funcionalidades desenvolvidas, assegurando que tudo funcione conforme o esperado.
- [ ] **Manutenção e correção de bugs**: Além do desenvolvimento de novas funcionalidades, o desenvolvedor também é responsável pela manutenção do sistema, corrigindo eventuais bugs que possam surgir.
- [ ] **Colaboração com a equipe**: O desenvolvedor trabalha em estreita colaboração com os demais membros da equipe, como os arquitetos, designers e o orquestrador dos trabalhos, para garantir a integração adequada das funcionalidades e a entrega do projeto conforme o planejado.
- [ ] **Documentação do código**: O desenvolvedor deve manter a documentação do código sempre atualizada, tornando-o compreensível para outros membros da equipe e facilitando futuras manutenções.
- [ ] **Integração com o Azure-DevOps**: O desenvolvedor utiliza o Azure-DevOps para gerenciar o versionamento do código, acompanhar as tarefas e sprints, e colaborar com a equipe no desenvolvimento do projeto.
## Alguns Requisitos

- [ ] **Deverão ser utilizados SDKs para o Desenvolvimento (Software Development Kit)**;
- [ ] **Deverá ser utilizada a estratégia de Trunk Based Development**;
- [ ] **Deverá ser utilizada a Estratégias de Deployment - Versioned Deployment**;
- [ ] **Diagramas MER/DER deverão ser realizados em ferramenta SQL DataModeler**;

## Requisitos de Arquitetura


[![](https://mermaid.ink/img/pako:eNp1U8tuGzEM_BVhTwkQIEDRk1E0MNYueogRxBs0F1_oFS2zWYkbPdI6QT6m6KGnnoJ-wf5YGNv7gJ3eRM4MOaSkp6xkjdkos-S0hXrhlPLM8eRk6iI6jf7T-dJ_ZuXQNC8l8enpG0WpLxDZY1D3CbeMnCtYsge7g5W6ZGfUmoLQNm2uQBdY5WxTRxuLSINBq75yJWwqoYW-UWh-c0eMFJNGlfvmb8-6TkBBQRB_JYZAGjSGVjKVcha8SiE1vzxxB2x1LnK4OMhIoejBBWj-NP_wAK4Uq4i25u3AYkXmrzlEuDhsWMqETjxKlX4ApeZYQWxexMmgcDErBtHtGmIY1_UgdYNgWydtgxssHVdsqFvW-DF57EUTfOB6MG_OMhw59GLCyJr7O7kkuWg_8MPOgb9Oy67aLS4L9A9U4qDg1XxStNFVkqUNsAlEuGTQfcbeaS4HjDZjofQc6ioZcseoqcis45J_viNEb4H0h_9J_fbthh9gDPpj0h7YsY7VezhRBPNOb3K02hwWreg-0RICDgX9WYR3fasin3WQodid5eFYio_ohqjl77SLJwRGvli_69l0fj6Zztsw_6hm8p2rDt5tSWxkZ9l-ZfLXn97wRRbXaHGRjeSocQWpiots4Z6FCilysXFlNoo-4VmWag0R992z0QqqgM-vXmNQaA?type=png)](https://mermaid.live/edit#pako:eNp1U8tuGzEM_BVhTwkQIEDRk1E0MNYueogRxBs0F1_oFS2zWYkbPdI6QT6m6KGnnoJ-wf5YGNv7gJ3eRM4MOaSkp6xkjdkos-S0hXrhlPLM8eRk6iI6jf7T-dJ_ZuXQNC8l8enpG0WpLxDZY1D3CbeMnCtYsge7g5W6ZGfUmoLQNm2uQBdY5WxTRxuLSINBq75yJWwqoYW-UWh-c0eMFJNGlfvmb8-6TkBBQRB_JYZAGjSGVjKVcha8SiE1vzxxB2x1LnK4OMhIoejBBWj-NP_wAK4Uq4i25u3AYkXmrzlEuDhsWMqETjxKlX4ApeZYQWxexMmgcDErBtHtGmIY1_UgdYNgWydtgxssHVdsqFvW-DF57EUTfOB6MG_OMhw59GLCyJr7O7kkuWg_8MPOgb9Oy67aLS4L9A9U4qDg1XxStNFVkqUNsAlEuGTQfcbeaS4HjDZjofQc6ioZcseoqcis45J_viNEb4H0h_9J_fbthh9gDPpj0h7YsY7VezhRBPNOb3K02hwWreg-0RICDgX9WYR3fasin3WQodid5eFYio_ohqjl77SLJwRGvli_69l0fj6Zztsw_6hm8p2rDt5tSWxkZ9l-ZfLXn97wRRbXaHGRjeSocQWpiots4Z6FCilysXFlNoo-4VmWag0R992z0QqqgM-vXmNQaA){width="1200" height="300" style="display: block; margin: 0 auto"}
