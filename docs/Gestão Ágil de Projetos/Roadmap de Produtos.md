Um roadmap de produto é um instrumento estratégico que alinha visão, planejamento e execução, garantindo que todas as partes interessadas (stakeholders) compreendam o direcionamento do produto. Sua elaboração é essencial por vários motivos:

- [ ] Alinhamento Estratégico e de Prioridades
- [ ] Comunicação Transparente com Stakeholders
- [ ] Adaptação a Mudanças e Riscos
- [ ] Otimização de Recursos e Tempo
- [ ] Mensuração de Resultados

Um roadmap de produto não é apenas um cronograma, mas uma ferramenta dinâmica que:

- [ ] Alinha times em torno de objetivos comuns.
- [ ] Comunica o plano de forma visual e acessível.
- [ ] Adapta-se a mudanças sem perder o foco estratégico.

Sem ele, a gestão do produto fica **reativa, fragmentada e sujeita a falhas** de execução.

Portanto, sua elaboração é não apenas necessária, mas crítica para o sucesso sustentável.

### Definir Formato (Tático vs. Estratégico)

| Roadmap Estratégico (Longo Prazo)                           | Roadmap Tático (Curto Prazo)                              |
| ----------------------------------------------------------- | --------------------------------------------------------- |
| Foco em objetivos macro (ex: expansão para novos mercados). | Foco em entregas imediatas (ex: lançamento de feature X). |
| Escopo flexível, sem prazos rígidos.                        | Cronograma detalhado (sprints, milestones).               |
| Público-alvo: liderança e investidores.                     | Público-alvo: equipes de desenvolvimento e operação.      |
#### Matriz de Priorização

| Iniciativa     | Impacto (1-5) | Esforço (1-5) | Alinhamento Estratégico | Pontuação  |
| -------------- | ------------: | ------------: | ----------------------: | :--------: |
| Integrar API   |             5 |             3 |                       4 | 12 (5+3+4) |
| Redesign da UI |             4 |             5 |                       3 | 12 (4+5+3) |

#### **Exemplo Estratégico 202X**

##### Objetivo Principal: [Ex: Liderança de mercado em X]


| Trimestre | Iniciativa                  | Métrica de Sucesso       | Dados de Apoio            |
| --------- | --------------------------- | ------------------------ | ------------------------- |
| Q1        | Lançamento do Módulo A      | +15% de retenção         | Pesquisa com 200 clientes |
| Q2        | Integração com Plataforma B | 20 parceiros onboardados | Benchmarking competitivo  |
##### **Roadmap Tático - Q1 202X**

| Sprint | Tarefa                 | Responsável | Status       |
| ------ | ---------------------- | ----------- | ------------ |
| 1      | Protótipo da Feature X | Time Dev    | Em andamento |
| 2      | Testes de Usabilidade  | UX          | Planejado    |
**Observação**: Este modelo garante clareza, adaptabilidade e decisões baseadas em dados, essenciais para um produto competitivo.

##### **Fato Projeto Atualização do e-Business Suite**

```mermaid

gantt

dateFormat YYYY-MM-DD

title Clonagem

excludes weekends

%% (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)

  

section Desenvolvimento

Q_01/2025 :done, DEV20241,2024-12-27,2025-03-28

DBA_01/2025 :DBA1,2024-12-27, 5d

Q_02/2025 :done, DEV20252,2025-04-02,2025-07-04

DBA_02/2025 :DBA2,2025-04-02, 5d

Q_03/2025 :done, DEV20253,2025-07-09,2025-10-10

DBA_03/2025 :DBA3,2025-07-09, 5d

Q_04/2026 :done, DEV20254,2025-10-15,2026-01-16

DBA_04/2026 :DBA4,2025-10-15, 5d

Q_01/2026 :done, DEV20261,2026-01-21,2026-04-24

DBA_01/2026 :DBA5,2026-01-21, 5d

Q_02/2026 :done, DEV20262,2026-04-29,2026-07-31

DBA_02/2026 :DBA6,2026-04-29, 5d

Q_03/2026 :done, DEV20263,2026-08-05,2026-11-06

DBA_03/2026 :DBA7,2026-08-05, 5d

Q_01/2027 :done, DEV20261,2026-11-11,2027-02-12

DBA_01/2027 :DBA8,2026-11-11, 5d

Q_02/2027 :done, DEV20272,2027-02-17,2027-05-21

DBA_02/2027 :DBA9,2027-02-17, 5d

section Projeto

SET/2025 :P1, 2025-09-08, 20d

FUNC_01/2025 :FUNC1,2025-09-28, 30d

SET/2026 :P2, 2026-09-07, 20d

FUNC_02/2026 :FUNC2,2026-09-27, 5d

section Homologação

H_01/2025 :done, HML20251,2025-04-02,2025-05-02

HBA_01/2025 :HBA1,2025-04-02, 5d

H_02/2025 :done, HML20252,2025-05-07,2025-06-06

HBA_02/2025 :HBA2,2025-05-07, 5d

H_03/2025 :done, HML20253,2025-06-11,2025-07-11

HBA_03/2025 :HBA3,2025-06-11, 5d

H_04/2025 :done, HML20254,2025-07-16,2025-08-15

HBA_04/2025 :HBA4,2025-07-16, 5d

H_05/2025 :done, HML20255,2025-08-20,2025-09-19

HBA_05/2025 :HBA5,2025-08-20, 5d

H_06/2025 :done, HML20256,2025-09-24,2025-10-24

HBA_06/2025 :HBA6,2025-09-24, 5d

H_07/2025 :done, HML20257,2025-10-29,2025-11-28

HBA_07/2025 :HBA7,2025-10-29, 5d

H_08/2026 :done, HML20258,2025-12-03,2026-01-02

HBA_08/2026 :HBA8,2025-12-03, 5d

H_09/2026 :done, HML20269,2026-01-07,2026-02-06

HBA_09/2026 :HBA9,2026-01-07, 5d

H_10/2026 :done, HML202610,2026-02-11,2026-03-13

HBA_10/2026 :HBA10,2026-02-11, 5d

H_11/2026 :done, HML202611,2026-03-18,2026-04-17

HBA_11/2026 :HBA11,2026-03-18, 5d

H_12/2026 :done, HML202612,2026-04-22,2026-05-22

HBA_12/2026 :HBA12,2026-04-22, 5d

H_13/2026 :done, HML202613,2026-05-27,2026-06-26

HBA_13/2026 :HBA13,2026-05-27, 5d

```



### Segurança de Código
### Testes
O teste automatizado é um componente central da Integração Contínua, pois permite que os desenvolvedores validem novas alterações de código em relação à base de código existente de forma rápida e eficiente.
#### Por que o teste automatizado é crucial para CI
Os testes automatizados desempenham um papel crítico no processo de CI por vários motivos:

- [x] **Feedback mais rápido**: executar testes automaticamente como parte do seu pipeline de CI fornece feedback imediato sobre o impacto de novas alterações de código, permitindo que os desenvolvedores resolvam problemas antes que se tornem problemas mais significativos.
- [x] **Esforço manual reduzido**: automatizar testes elimina a necessidade de testes manuais, liberando tempo dos desenvolvedores para se concentrarem na implementação de novos recursos e na correção de bugs.
- [x] **Ambiente de teste consistente**: testes automatizados são executados em um ambiente consistente, reduzindo a probabilidade de discrepâncias entre execuções de teste e garantindo um processo de validação confiável.
- [x] **Colaboração aprimorada**: com testes automatizados em vigor, os membros da equipe podem ter mais confiança na estabilidade da base de código, facilitando a colaboração em novos recursos e correções de bugs.

  

Existem vários tipos de testes que você pode incorporar em seus fluxos de trabalho de CI, dependendo dos requisitos do seu projeto e do nível de validação necessário:

- [x] **Testes de unidade**: Os testes de unidade focam em pequenos pedaços isolados de código, como funções ou classes individuais. Esses testes garantem que cada componente funcione conforme o esperado isoladamente.
- [x] **Testes de integração**: Os testes de integração examinam as interações entre diferentes componentes do seu aplicativo para garantir que eles funcionem juntos corretamente.
- [x] **Testes Funcionais**: Os testes funcionais validam a funcionalidade geral do seu aplicativo da perspectiva do usuário, geralmente por meio de interações de IU automatizadas ou chamadas de API.
- [x] **Testes de Desempenho**: Os testes de desempenho avaliam a capacidade de resposta, a escalabilidade e a estabilidade do seu aplicativo sob várias condições de carga.

### Cobertura e Relatórios de código
A cobertura de código é uma métrica importante que mede a porcentagem do seu código que é executada durante o teste.

Ela ajuda os desenvolvedores a identificar áreas do código que podem não ser testadas adequadamente e exigem testes adicionais para garantir a correção e a confiabilidade.
  
### Introdução à Cobertura de Código
A cobertura de código é uma métrica que quantifica o grau em que o código-fonte de um programa é testado por um conjunto de testes específico.

Geralmente é expressa como uma porcentagem e representa a proporção de linhas de código, ramificações, funções ou outras unidades lógicas que foram executadas durante o processo de teste.

  

A cobertura de código fornece insights valiosos sobre a eficácia do seu conjunto de testes, destacando áreas do código que podem não ser testadas adequadamente e potencialmente abrigando bugs ou problemas não descobertos.

  

Ao medir a cobertura de código, os desenvolvedores podem identificar lacunas em sua cobertura de teste e priorizar a criação de novos testes para garantir que a funcionalidade crítica seja completamente testada.

  

É importante observar, no entanto, **que uma alta porcentagem de cobertura de código não garante a ausência de bugs ou a qualidade geral do software**. É apenas um indicador da extensão em que o código foi exercido pelo conjunto de testes.

  

Outros fatores, como a minúcia dos próprios testes, também desempenham um papel crucial na confiabilidade e na manutenibilidade da base de código.

  

No contexto da Integração Contínua, a cobertura de código serve como uma métrica útil para monitorar a eficácia contínua do seu conjunto de testes e orientar melhorias na sua estratégia de testes.

  

#### Importância da cobertura de código em CI

A cobertura de código desempenha um papel crucial na Integração Contínua (CI) por vários motivos:
- [ ] **Detecção precoce de código não Testado**: Ao medir regularmente a cobertura de código como parte do seu pipeline de CI, você pode identificar rapidamente áreas do código que não foram suficientemente testadas. Isso permite que os desenvolvedores abordem problemas potenciais antes que se tornem problemas mais significativos e ajuda a manter uma base de código robusta e confiável.

- [ ] **Monitoramento da eficácia do conjunto de Testes**: As métricas de cobertura de código fornecem insights sobre a eficácia geral do seu conjunto de testes, garantindo que ele continue a fornecer cobertura adequada conforme a base de código evolui. Isso permite que os desenvolvedores tomem decisões informadas sobre onde concentrar seus esforços de teste, garantindo que as partes mais críticas do código sejam completamente testadas.

- [ ] **Qualidade de código Aprimorada**: Um conjunto de testes abrangente, combinado com análise regular de cobertura de código, incentiva os desenvolvedores a escrever código mais limpo e modular, mais fácil de testar e manter. Isso resulta em uma base de código de maior qualidade com menos bugs e problemas.

- [ ] **Maior confiança nas alterações de Código**: Ao manter um alto nível de cobertura de código, os desenvolvedores podem ter maior confiança de que suas alterações não introduzirão novos bugs ou regressões. Isso pode levar a ciclos de desenvolvimento mais rápidos e melhor colaboração entre os membros da equipe, pois há menos risco associado a fazer alterações no código.

- [ ] **Responsabilidade e Visibilidade**: Integrar métricas de cobertura de código em seu pipeline de CI fornece uma medida transparente e objetiva da eficácia do conjunto de testes. Isso pode ajudar a estabelecer expectativas claras e responsabilidade para a equipe, garantindo que os testes permaneçam uma prioridade durante todo o processo de desenvolvimento.

  

Em resumo, a cobertura de código é um aspecto essencial da implementação da Integração Contínua, pois ajuda a garantir uma base de código confiável e de alta qualidade.

  

Ao medir e monitorar regularmente a cobertura de código como parte de seu pipeline de CI, você pode identificar lacunas em sua cobertura de teste, priorizar os esforços de teste e manter um conjunto de testes abrangente que minimiza o risco de bugs e regressões.

  

### Container

##### Escanear Dockerfile

##### Assinar contêiner

### Monitoramento

### Segurança

#### Tratamento de Segredos

#### Dados Confidenciais

### Implantação em várias plataformas

#### Implantando em servidores locais

A implantação local se refere à hospedagem de seu aplicativo em seus próprios servidores físicos ou virtuais, em vez de utilizar plataformas de nuvem.

Embora a implantação em servidores locais possa exigir mais gerenciamento de infraestrutura em comparação às plataformas de nuvem, ela pode oferecer maior controle sobre sua infraestrutura, segurança aprimorada e possíveis economias de custos.

Certifique-se de criar um ambiente dedicado para cada estágio do seu pipeline de implantação (desenvolvimento, preparação e produção).

| **Aspecto**                | **Continuous Integration (CI)**                                        | **Continuous Delivery (CD)**                                                | **Continuous Deployment (CD)**                                                     |
| -------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Objetivo**               | Integrar e testar código frequentemente para detectar erros cedo       | Garantir que o código esteja sempre pronto para ser liberado                | Automatizar a liberação do código diretamente para produção                        |
| **Frequência de Deploy**   | Nenhum deploy automático; apenas integração e testes contínuos         | Deploy manual para produção, mas o código está sempre pronto                | Deploy automático em produção após testes e validações automáticas                 |
| **Ação Manual**            | Não envolve deploy ou release manual                                   | A liberação para produção é manual ou por aprovação                         | Nenhuma ação manual; o deploy ocorre automaticamente para produção                 |
| **Ponto de Feedback**      | Feedback imediato após integração e testes unitários                   | Feedback contínuo com a garantia de que o código está pronto para produção  | Feedback rápido com liberação contínua após aprovação de testes                    |
| **Exemplo de Ferramentas** | Jenkins, Travis CI, CircleCI, GitLab CI                                | Jenkins, Spinnaker, GitLab CI, Bamboo                                       | Jenkins, CircleCI, GitLab CI, AWS CodePipeline                                     |
| **Benefício Principal**    | Identificação precoce de problemas de integração e qualidade do código | Liberação mais rápida e controlada para produção, com menos risco de falhas | Entrega contínua, com mudanças sendo rapidamente disponibilizadas para os usuários |
| **Foco**                   | Automatizar testes e integração de código                              | Garantir que o código esteja pronto para produção a qualquer momento        | Automatizar todo o processo, incluindo o deploy em produção                        |
| **Exemplo de Workflow**    | Desenvolvedor envia código → Testes e integração contínuos             | Código aprovado → Pré-produção → Aprovação manual → Deploy em produção      | Código aprovado → Deploy automático em produção                                    |
  

```mermaid

sequenceDiagram

participant Delivery as Delivery Team

participant VersionControl as Version Control

participant BuildTest as Build & Unit Test

participant AutoAcceptTest as Automated Acceptance Test

participant UserAcceptTest as User Acceptance Test

participant Release as Release

  

%% Continuous Integration (CI)

Delivery->>VersionControl: Check-in de código

VersionControl->>BuildTest: Trigger de Build & Unit Test

BuildTest->>VersionControl: Feedback de Build & Unit Test (sucesso ou falha)

alt Sucesso no Build

BuildTest->>AutoAcceptTest: Trigger para Automated Acceptance Test

AutoAcceptTest->>BuildTest: Feedback de Automated Acceptance Test (sucesso ou falha)

alt Sucesso nos Testes Automatizados

%% Continuous Delivery (CD)

AutoAcceptTest->>UserAcceptTest: Trigger para User Acceptance Test

UserAcceptTest->>AutoAcceptTest: Feedback de User Acceptance Test (sucesso ou falha)

alt Sucesso nos Testes de Aceitação do Usuário

%% Continuous Deployment (CD)

UserAcceptTest->>Release: Trigger para Release

Release->>UserAcceptTest: Feedback de Release (sucesso ou falha)

else Falha nos Testes de Aceitação do Usuário

UserAcceptTest->>Delivery: Feedback de falha

end

else Falha nos Testes Automatizados

AutoAcceptTest->>Delivery: Feedback de falha

end

else Falha no Build

BuildTest->>Delivery: Feedback de falha

end

```

  
# Termos


- [ ] Nightly Builds (ou compilações noturnas) são processos automatizados de construção, teste e deploy de um software que são executados todas as noites, geralmente em um horário programado (ex.: 2h da manhã). Eles são uma prática essencial no desenvolvimento contínuo (Continuous Integration/Delivery - CI/CD) para garantir a estabilidade do código.