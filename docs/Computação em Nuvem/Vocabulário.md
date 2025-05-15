- [ ] LAN (Local Area Network): Uma **rede local** que conecta dispositivos em uma área geográfica restrita, como uma casa, escritório, escola ou prédio. Alta (até 10 Gbps)
- [ ] WAN (Wide Area Network): **rede de longa distância** que conecta múltiplas LANs espalhadas geograficamente — entre cidades, estados ou até países. Variável (Mbps a Gbps)
- [ ] Espaço público reservado

|Conceito / Escopo|**AWS**|**Azure**|**Google Cloud (GCP)**|**Oracle Cloud (OCI)**|**Alibaba Cloud**|
|---|---|---|---|---|---|
|**Região geográfica (Region)**|`Region` (ex: us-east-1)|`Region` (ex: East US)|`Region` (ex: us-central1)|`Region` (ex: us-ashburn-1)|`Region` (ex: cn-hangzhou)|
|**Zona de disponibilidade**|`Availability Zone (AZ)`|`Availability Zone`|`Zone`|`Availability Domain`|`Zone`|
|**Tenant / Espaço isolado**|`Account` ou `Organization`|`Tenant` (dentro do AAD)|`Project`|`Tenancy`|`Account`|
|**Unidade de cobrança**|`Account` / `Billing Entity`|`Subscription`|`Billing Account` + `Project`|`Compartment` + `Tenancy`|`Resource Group` / `Account`|
|**Ambiente lógico de recursos**|`VPC`|`Resource Group`|`Project`|`Compartment`|`Resource Group`|
|**Catálogo público de serviços**|`Public Cloud`|`Azure Public Cloud`|`Google Public Cloud`|`Oracle Public Cloud`|`Alibaba Public Cloud`|
- [ ] Plataformas de Gerenciamento de Nuvem (Cloud Management Platforms – CMPs)

| **Provedor**      | **Plataforma de Gerenciamento de Nuvem**           | **Principais Recursos / Funções**                                                              |
| ----------------- | -------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **AWS**           | **AWS Systems Manager**                            | Automação, inventário, gerenciamento de patch, monitoramento de conformidade, execução remota. |
|                   | **AWS Control Tower**                              | Governança multi-conta, landing zones, políticas e conformidade.                               |
|                   | **AWS CloudFormation / OpsWorks**                  | Provisionamento e gerenciamento de infraestrutura como código (IaC).                           |
| **Azure**         | **Azure Arc**                                      | Gerenciamento de recursos locais, multi-cloud, Kubernetes, políticas e identidade.             |
|                   | **Azure Monitor / Azure Automation**               | Observabilidade, alertas, autoscaling, runbooks e scripts automáticos.                         |
|                   | **Azure Lighthouse**                               | Gerenciamento centralizado e seguro de múltiplos tenants para MSPs.                            |
| **GCP**           | **Google Cloud Operations Suite (ex Stackdriver)** | Monitoramento, logging, rastreamento, dashboards, alertas.                                     |
|                   | **Cloud Deployment Manager**                       | Gerenciamento de infraestrutura como código.                                                   |
|                   | **Anthos**                                         | Gerenciamento multi-cloud e Kubernetes, com controle de políticas.                             |
| **Oracle Cloud**  | **OCI Resource Manager**                           | Gerenciamento IaC com Terraform.                                                               |
|                   | **OCI Operations Insights / Monitoring**           | Monitoramento de desempenho e capacidade, alertas, machine learning para otimização.           |
|                   | **OCI Cloud Guard / Security Zones**               | Governança e segurança automatizada de recursos em nuvem.                                      |
| **Alibaba Cloud** | **Alibaba Cloud Resource Management**              | Organização de contas, tags, acesso e permissões.                                              |
|                   | **Cloud Config / ActionTrail / Operation Audit**   | Conformidade, auditoria e rastreamento de mudanças.                                            |
|                   | **Resource Orchestration Service (ROS)**           | Infraestrutura como código semelhante ao AWS CloudFormation.                                   |
- [ ] **Multilocação** é a capacidade de um sistema de atender a múltiplos clientes com a mesma instância de software ou infraestrutura, garantindo isolamento, segurança e personalização entre eles.
- [ ] RTO/RPO

| **Provedor/Plataforma no Brasil** | **Presença Local**                           | **Short-Distance (mesma região)** | **Long-Distance (entre regiões/países)** | **RPO (estimado)**                    | **RTO (estimado)**                         |
| --------------------------------- | -------------------------------------------- | --------------------------------- | ---------------------------------------- | ------------------------------------- | ------------------------------------------ |
| **AWS (Amazon Web Services)**     | São Paulo (Region)                           | Zonas de disponibilidade em SP    | Cross-region (ex: SP ↔ Virgínia, USA)    | RPO: ~0-15 min (multi-AZ)             | RTO: ~<1 hora (short), até horas (long)    |
| **Microsoft Azure**               | SP e RJ (Availability Zones)                 | Zonas na mesma região             | Azure Geo-Replicated (ex: Brasil ↔ EUA)  | RPO: ~15 min (Geo-Red.)               | RTO: 1h+ (manual), <15 min (com automação) |
| **Google Cloud Platform (GCP)**   | São Paulo (Region)                           | Zonas de SP                       | Multi-region (ex: SP ↔ EUA, EU)          | RPO: ~<1 min (Cloud SQL HA)           | RTO: ~1h (com scripts)                     |
| **Oracle Cloud (OCI)**            | Vinhedo-SP (Region)                          | Zonas internas (1 region apenas)  | Vinhedo ↔ Ashburn, EUA                   | RPO: 0 (Data Guard)                   | RTO: ~<1h (manual switchover)              |
| **Alibaba Cloud**                 | Sem região própria no Brasil (via parceiros) | N/A                               | Long-distance via Hong Kong / EUA        | RPO: >15 min (dependendo do parceiro) | RTO: 2h+                                   |
| **LocalWeb Cloud**                | SP e outros datacenters                      | SP ↔ RJ ou DCs próximos           | SP ↔ EUA (Cloud2b, etc.)                 | RPO: ~15–60 min                       | RTO: 1–2 horas                             |
| **UOL Diveo / Compasso Cloud**    | SP, Campinas, etc.                           | DCs redundantes locais            | SP ↔ Miami / Santiago                    | RPO: ~30 min                          | RTO: 2–4 horas (dependendo da arquitetura) |
| **Tivit Cloud**                   | SP, RJ, Chile                                | DCs em SP e RJ                    | SP ↔ Chile / EUA                         | RPO: 0–30 min (com replicação)        | RTO: ~1–2h (varia por serviço)             |
