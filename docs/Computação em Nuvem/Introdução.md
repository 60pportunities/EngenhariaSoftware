Computação em Nuvem é um modelo de entrega de serviços de TI sob demanda via internet, onde recursos como servidores, armazenamento, bancos de dados, redes, softwares, inteligência artificial e análises são disponibilizados de forma escalável, flexível e paga conforme o uso.
### **Origem do Conceito**
A ideia central da computação em nuvem remonta à **década de 1960**, com visões de compartilhamento de recursos computacionais:

- [ ] **J.C.R. Licklider** (1960s): Cientista da ARPA que idealizou uma rede interconectada ("Intergalactic Computer Network"), base do que viria a ser a internet.
- [ ] **Termo "Cloud"**: Surgiu nos anos 1990 como metáfora para a internet (representada por uma nuvem em diagramas de rede).
- [ ] **John McCarthy** (1927–2011) foi um cientista da computação pioneiro, conhecido por:
   - [ ] **Visão da Computação como Utility** (1961): Em um discurso no MIT, ele propôs que a computação poderia ser organizada como um **serviço público**, semelhante à eletricidade ou água, onde usuários pagariam apenas pelo que consumissem.
### **CAPEX vs OPEX**

- [ ] CapEx é a abreviação de Capital Expenditures ou "Despesas de Capital". Essas despesas consistem nos fundos que as empresas usam para comprar os principais bens físicos ou serviços que a empresa usará (geralmente) por mais de um ano.
	- [ ] Uma vez que o ativo está sendo usado, ele é depreciado ao longo do tempo para distribuir o custo do ativo ao longo de sua vida útil. Em outras palavras, a cada ano, uma parte do ativo fixo está sendo "consumida" ou "depreciada".
	- [ ] A depreciação representa o grau de desgaste de um ativo. As empresas podem deduzir o valor da depreciação em sua declaração anual de impostos.
	- [ ] Em alguns casos, pode ser conhecido como custos "Up-Front". Ou seja, a empresa precisa pagar ou adquirir um equipamento antes de usá-lo.
- [ ] OpEx é a abreviação de Operational Expenditures ou "Despesas Operacionais". Refere-se às despesas que uma empresa incorre em suas operações diárias.
	- [ ] Como as despesas operacionais constituem a maior parte dos custos contínuos de uma empresa, a administração normalmente procura maneiras de reduzir seu OPEX sem causar uma queda crítica na qualidade ou na produção.
	- [ ] As despesas operacionais são deduzidas integralmente na declaração anual de impostos, no período em que foram incorridas.

| **Aspecto**            | **CAPEX (Despesas de Capital)**                                                                         | **OPEX (Despesas Operacionais)**                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Definição**          | Gastos com aquisição de ativos físicos ou investimentos de longo prazo.                                 | Gastos recorrentes com operações diárias, serviços ou recursos consumidos durante o uso.                                    |
| **Exemplos**           | Compra de servidores físicos <br>Aquisição de licenças de software perpétuas  <br>Data centers próprios | Pagamento mensal por serviços de nuvem (OCI, GCP, AWS, Azure)  <br>Modelo "pay-as-you-go"  <br>Custos de manutenção de SaaS |
| **Impacto Financeiro** | Alto custo inicial  <br>Ativo registrado no balanço patrimonial  <br>Depreciação ao longo do tempo      | Custo variável conforme o uso  <br>Despesa operacional (dedutível imediatamente)  <br>Sem depreciação                       |
| **Flexibilidade**      | Menos flexível (investimento fixo)  <br>Risco de obsolescência tecnológica                              | Alta flexibilidade (escala conforme demanda)  <br>Atualizações automáticas e sem custo adicional                            |
| **Escalabilidade**     | Requer planejamento prévio para expansão  <br>Limitações físicas (espaço, energia, hardware)            | Escalabilidade elástica (aumento/redução de recursos em minutos)                                                            |
| **Responsabilidade**   | Empresa responsável por manutenção, upgrades e segurança física                                         | Provedor de nuvem gerencia infraestrutura, segurança e atualizações                                                         |
| **Benefício Fiscal**   | Depreciação do ativo ao longo de anos (redução gradual do impacto fiscal)                               | Dedução fiscal imediata (100% do custo como despesa operacional no ano)                                                     |
| **Cenários de Uso**    | Cargas de trabalho previsíveis e estáveis  <br>Requisitos regulatórios de infraestrutura local          | Demanda variável  <br>Startups ou empresas que buscam redução de custos iniciais  <br>- Inovação ágil                       |

### **Comparação Direta na Nuvem**

| **Característica**       | **CAPEX (Modelo Tradicional)**                                      | **OPEX (Cloud Computing)**                                    |
| ------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------- |
| **Custo Inicial**        | Alto investimento em hardware, licenças e infraestrutura.           | Baixo ou nenhum custo inicial (pago conforme o uso).          |
| **Alocação de Recursos** | Recursos fixos (subutilização ou falta de capacidade comum).        | Recursos sob demanda (evita desperdício).                     |
| **Inovação**             | Lentidão para adotar novas tecnologias (ciclos longos).             | Acesso imediato a tecnologias emergentes (ex.: IA, Big Data). |
| **Risco Financeiro**     | Alto risco de investimento em ativos que podem se tornar obsoletos. | Risco reduzido (custos alinhados ao crescimento do negócio).  |

### **Modelos de Cloud**
##### **Public Cloud**
A **nuvem pública** é um modelo de computação em nuvem onde os recursos (servidores, armazenamento, redes, etc.) são disponibilizados por um **provedor terceirizado** via internet, sendo compartilhados entre múltiplos clientes ("multi-tenancy"). 

Os usuários **pagam apenas pelo que configuram**, sem necessidade de investir em infraestrutura física.

- [ ] A nuvem pública é **100% operacional** (OPEX), pois os custos são recorrentes e baseados no uso (ex.: pagamento mensal por horas de servidor ou GB armazenados).
- [ ] 
##### **Vantagens Financeiras e Operacionais**

| **Característica** | **Descrição**                                                           |
| ------------------ | ----------------------------------------------------------------------- |
| **Flexível**       | Adaptação rápida a necessidades variáveis sem custos fixos.             |
| **Escalável**      | Expansão ou redução automática de recursos conforme a demanda.          |
| **Resiliente**     | Alta disponibilidade e recuperação de desastres sem intervenção manual. |
- [ ] **Redução de CAPEX**: Elimina investimentos em hardware, licenças perpétuas e data centers próprios.
- [ ] **Custo variável**: Pague apenas pelo uso real (ideal para empresas com demanda flutuante).
- [ ] **Foco no core business**: A empresa não precisa gerenciar infraestrutura, apenas consumir serviços

##### **Hybrid Cloud**
A **Nuvem Híbrida** é um ambiente de computação em nuvem que combina infraestrutura **local (on-premises)**, **nuvem privada** (geralmente dedicada a um único cliente) e **nuvem pública**, permitindo que dados e aplicações sejam compartilhados entre elas. 
O objetivo é equilibrar controle, segurança, custos e flexibilidade, usando cada ambiente para cargas de trabalho específicas.
##### **Vantagens Financeiras e Operacionais**

| **Característica** | **Descrição**                                                                  |
| ------------------ | ------------------------------------------------------------------------------ |
| **Flexível**       | Movimentação dinâmica de cargas entre ambientes conforme necessidades.         |
| **Escalável**      | Expansão temporária de recursos na nuvem pública sem investimento local.       |
| **Resiliente**     | Alta disponibilidade através de redundância entre ambientes locais e na nuvem. |

- [ ] **Controle e conformidade**: Dados sensíveis permanecem on-premises ou em nuvem privada, atendendo a regulamentações (ex.: LGPD, GDPR).
- [ ] **Otimização de custos**: Uso da nuvem pública apenas para demandas variáveis, reduzindo CAPEX em hardware.
- [ ] **Inovação gradual**: Migração de aplicações legadas para a nuvem pública sem abandonar investimentos locais.
- [ ] **Setores regulamentados**: Saúde, finanças ou governo (exige controle de dados).
- [ ] **Cargas de trabalho mistas**: Algumas aplicações exigem baixa latência (local), enquanto outras precisam de escalabilidade (nuvem pública).
- [ ] **Transição para a nuvem**: Empresas em processo de migração que não podem abandonar infraestrutura legada rapidamente.
- [ ] **Pode ser vista**, como uma ponte entre o **controle tradicional** e a **agilidade da nuvem pública**, ideal para organizações que buscam equilibrar segurança, custos e inovação.

###  **Private Cloud**
A **Nuvem Privada** é um ambiente de computação em nuvem dedicado exclusivamente a uma única organização. Pode ser hospedado **on-premises** (no data center local) ou por um provedor terceirizado, mas os recursos não são compartilhados com outros usuários ("single-tenancy"). Oferece maior controle, segurança e personalização em comparação com a nuvem pública.

##### **Vantagens Financeiras e Operacionais**
A Private Cloud **prioriza CAPEX**, mas pode incluir OPEX dependendo do modelo:

- [ ] **CAPEX**: Investimento em hardware, licenças de software e infraestrutura física (ex.: servidores locais).
- [ ] **OPEX**: Custos recorrentes se a nuvem privada for hospedada por um provedor terceirizado (ex.: manutenção, atualizações).

| **Característica** | **Descrição**                                                          |
| ------------------ | ---------------------------------------------------------------------- |
| **Flexível**       | Adaptação completa a requisitos técnicos e regulatórios.               |
| **Escalável**      | Expansão limitada pela infraestrutura física ou contrato com provedor. |
| **Resiliente**     | Disponibilidade garantida por redundância controlada internamente.     |

- [ ] **Segurança avançada**: Dados sensíveis não são compartilhados com terceiros.
- [ ] **Conformidade**: Adequação a leis locais (ex.: GDPR, LGPD) e setores regulados (saúde, governo).
- [ ] **Desempenho previsível**: Latência controlada e recursos dedicados para aplicações críticas.
- [ ] **Dados altamente confidenciais**: Setores como defesa, saúde ou finanças.
- [ ] **Aplicações legadas**: Sistemas que dependem de arquiteturas não compatíveis com nuvem pública.
- [ ] **Controle total**: Organizações que não podem delegar gestão de infraestrutura a terceiros.