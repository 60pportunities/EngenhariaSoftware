## SaaS, On-Premise
Mapear as aplicações em um ambiente **SaaS (Software as a Service)** para validar o **consumo de dados** é uma prática crítica, tanto do ponto de vista **estratégico quanto operacional**.

- [ ] Transparência sobre onde e como os dados são usados;
	- [ ] Que dados estão sendo consumidos por cada aplicação?
	- [ ] De onde esses dados vêm (fontes)? Com que frequência e volume?
- [ ] Evitar redundância e desperdício tecnológico
	- [ ] Conectores e integrações que **sobrecarregam APIs** ou bancos de dados.
	- [ ] Soluções "shadow IT" usando dados críticos **sem controle da TI**.
- [ ] Segurança e conformidade (GPDR, PCI DSS, LGPD e HIPAA)
- [ ] Controle de custos e otimização de licenças/API
	- [ ] Volume de chamadas API
	- [ ] Quantidade de dados processados
	- [ ] Licenças de usuários e conectores
- [ ] Facilita projetos de migração, integração ou modernização
	- [ ] Sem mapear os pontos de consumo de dados, qualquer mudança se torna um risco.

## Exemplo Mapeamento das Aplicações

| Nome da Aplicação     | Sigla | Descrição                                                               | Área Gestora (Negócio) | ANS Satisfação | Disponibilidade de Serviço | Níveis de Funcionamento do Serviço  | Datas de Importância                  | Tipo de Arquitetura | Linguagem  | Banco de Dados | Crescimento Anual do Banco (GB) | Tamanho Inicial do Banco (GB) |
| --------------------- | ----- | ----------------------------------------------------------------------- | ---------------------- | -------------- | -------------------------- | ----------------------------------- | ------------------------------------- | ------------------- | ---------- | -------------- | ------------------------------- | ----------------------------- |
| Gestão Corporativa    | GCORP | Aplicação monolítica para controle de processos administrativos         | Administrativo         | >= 85%         | 99,5%                      | Alta prioridade, operação 24x7      | Janeiro, Segunda-feira, 1-5           | Monolítica          | PHP e Java | Oracle         | 10                              | 10                            |
| Serviço de Pagamentos | SPAG  | Microserviços para processamento de pagamentos e conciliação financeira | Financeiro             | >= 90%         | 99,9%                      | Critico, operação 24x7 com failover | Dezembro, Sexta-feira, 10,15,20,25,30 | Microserviços       | Java       | MongoDB        | 10                              | 10                            |

## Exemplo Provisionamento de Aplicações
O provisionamento das aplicações em modelo **SaaS (Software as a Service)** está sendo realizado de forma controlada e supervisionada pela **equipe de TI**, garantindo que o consumo esteja alinhado com os requisitos técnicos, de segurança e de governança definidos pela organização. Esse monitoramento segue os princípios da **especificação FOCUS (FinOps Open Cost and Usage Specification)**, promovendo **transparência, padronização e rastreabilidade dos custos e métricas de uso** das aplicações em nuvem. Através da coleta e análise contínua de dados de consumo, a TI assegura que as decisões de escalabilidade, licenciamento e descontinuidade de serviços estejam embasadas em dados precisos e comparáveis entre provedores.
Buscando o equilíbrio **velocidade, controle e custo** no consumo de SaaS, com foco em **responsabilidade financeira compartilhada** entre áreas técnicas e de negócios.
### Exemplo: PHP

| **Componente**          | **Serviço AWS** | **Configuração**                                   | **Custo Mensal (USD)** | **Custo Anual (USD)** | **Observações**                     |
| ----------------------- | --------------- | -------------------------------------------------- | ---------------------- | --------------------- | ----------------------------------- |
| **Servidor Web (PHP)**  | EC2             | `t3.large` (4 vCPU, 8 GiB RAM) + EBS `gp3` (50 GB) |                        |                       | Auto Scaling para picos de demanda  |
| **Servidor Java (App)** | EC2             | `t3.large` (4 vCPU, 8 GiB RAM)                     |                        |                       | Cluster com 2 instâncias            |
| **Banco de Dados**      | RDS (Oracle)    | `db.t3.medium` (10 GB inicial) + 10 GB/ano         |                        |                       | Backup diário (7 dias retenção)     |
| **Armazenamento**       | S3              | 100 GB (Standard)                                  |                        |                       | Dados estáticos e logs              |
| **Balanceamento**       | ALB             | Application Load Balancer                          |                        |                       | Redirecionamento HTTP/HTTPS         |
| **Monitoramento**       | CloudWatch      | Métricas customizadas + Logs                       |                        |                       | Alertas para latência > 500ms       |
| **Segurança**           | WAF + Shield    | Proteção contra DDoS e vulnerabilidades            |                        |                       | Regras personalizadas para PHP/Java |
| **Total Monolítico**    |                 |                                                    |                        |                       |                                     |

### Exemplo: Java

| **Componente**          | **Serviço AWS**    | **Configuração**                        | **Custo Mensal (USD)** | **Custo Anual (USD)** | **Observações**                     |
| ----------------------- | ------------------ | --------------------------------------- | ---------------------- | --------------------- | ----------------------------------- |
| **Contêineres Java**    | ECS Fargate        | 4 tarefas (2 vCPU, 4 GB RAM cada)       |                        |                       | Escalável horizontalmente           |
| **Banco de Dados**      | MongoDB Atlas      | M10 Cluster (10 GB inicial) + 10 GB/ano |                        |                       | Replicação automática               |
| **API Gateway**         | API Gateway        | 1M requisições/mês                      |                        |                       | Rate limiting e cache               |
| **Monitoramento**       | CloudWatch + X-Ray | Rastreamento de microsserviços          |                        |                       | Análise de desempenho em tempo real |
| **Armazenamento**       | S3                 | 50 GB (Intelligent-Tiering)             |                        |                       | Dados de configuração               |
| **Total Microserviços** |                    |                                         |                        |                       |                                     |

### **Projeção de Crescimento**

| **Ano** | **Tamanho Oracle (GB)** | **Custo Oracle (USD/ano)** | **Tamanho MongoDB (GB)** | **Custo MongoDB (USD/ano)** |
| ------- | ----------------------- | -------------------------- | ------------------------ | --------------------------- |
| 1       | 10                      |                            | 10                       |                             |
| 2       | 20                      |                            | 20                       |                             |
| 3       | 30                      |                            | 30                       |                             |

**Observação**: Previsão de uma taxa de crescimento de 10 GBytes Anuais
