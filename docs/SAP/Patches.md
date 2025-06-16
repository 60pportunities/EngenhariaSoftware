https://www.leanix.net/en/wiki/tech-transformation/sap-s4hana-deployment-options?utm_term=&utm_source=google-ads&utm_medium=ppc&utm_campaign=AMERICAS-LAC_SAP-S4HANA_PCE_DSA_ENG&hsa_ver=3&hsa_cam=22643262919&hsa_grp=178370563617&hsa_acc=2468165327&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_src=g&hsa_tgt=aud-1531737551023:dsa-2279613690184&hsa_ad=756348201022&gad_source=1&gad_campaignid=22643262919&gbraid=0AAAAACe0l9wOVHqMkJ23TltcdO1qBJvBr&gclid=CjwKCAjw9anCBhAWEiwAqBJ-c_Q0fHk-fVPshSbKI869umNUiDUPaVHaWiXa2npKILgjs9q_UZeLfRoCn1IQAvD_BwE

## Versionamento Semantivo ()

Dado um número de versão MAJOR.MINOR.PATCH, incremente a:

- [ ]  versão Maior(MAJOR): quando fizer mudanças incompatíveis na API,
- [ ] versão Menor(MINOR): quando adicionar funcionalidades mantendo compatibilidade, e
- [ ] versão de Correção(PATCH): quando corrigir falhas mantendo compatibilidade.

- [ ] Versão Maior X (X.y.z | X > 0) DEVE ser incrementada se forem introduzidas mudanças incompatíveis na API pública. PODE incluir alterações a nível de versão Menor e de versão de Correção. Versão de Correção e Versão Menor DEVEM ser redefinidas para 0(zero) quando a versão Maior for incrementada.
- [ ] Versão Menor Y (x.Y.z | x > 0) DEVE ser incrementada se uma funcionalidade nova e compatível for introduzida na API pública. DEVE ser incrementada se qualquer funcionalidade da API pública for definida como descontinuada.
- [ ] Versão de Correção Z (x.y.Z | x > 0) DEVE ser incrementado apenas se mantiver compatibilidade e introduzir correção de bugs.

        1996 ──────────────────────────────────────────────► 2025

Oracle EBS:
        │
        ├─ 1996 → Oracle Financials 10.7
        ├─ 1998 → Oracle EBS 11.0
        ├─ 2000 → Oracle EBS 11i (11.5.0)
        ├─ 2004 → Oracle EBS 11.5.10.2
        ├─ 2007 → Oracle EBS R12.0
        ├─ 2009 → Oracle EBS R12.1
        ├─ 2013 → Oracle EBS R12.2 (Online Patching)
        ├─ 2013-2022 → R12.2.3 ~ R12.2.12 (Continuous Innovation)
        ├─ 2023 → Oracle EBS 12.2.13 (Atual)
        └─ 2030+ → Suporte Premier garantido

SAP S/4HANA (On-Premise & RISE Private Edition):
        │
        ├─ 2015 → 1503 (Finance release)
        ├─ 2015 → 1511 (Primeiro release completo)
        ├─ 2016 → 1610
        ├─ 2017 → 1709
        ├─ 2018 → 1809
        ├─ 2019 → 1909
        ├─ 2020 → 2020
        ├─ 2021 → 2021
        ├─ 2022 → 2022
        ├─ 2023 → 2023 (LTS atual, base Private Edition)
        └─ 2025 → 2025 (Nova LTS)

SAP S/4HANA Cloud Public Edition (RISE Public & GROW with SAP):
        │
        ├─ 2016-2022 → 1603~2208 (primeiros releases Cloud)
        ├─ 2023 → 2302 (nova nomenclatura YYMM)
        ├─ 2023 → 2305, 2308, 2311
        ├─ 2024 → 2402, 2405 (atual)
        └─ 2024 → 2408 (previsto para agosto)

GROW with SAP:
        │
        ├─ 2023 → Lançamento oficial
        └─ 2024 → Expansão forte na adoção global (rodando sempre na versão Public Edition)


## Histórico de Versões do Oracle E-Business Suite

| **Versão**           | **Ano de Lançamento** | **Notas / Evolução**                                      |
| -------------------- | --------------------- | --------------------------------------------------------- |
| EBS 10.7             | 1996                  | Primeira versão cliente-servidor.                         |
| EBS 11.0 (11.0.3)    | 1998                  | Chamada de "Oracle Applications 11".                      |
| EBS 11i (11.5.x)     | 2000–2006             | Interface web baseada em navegador; grande evolução.      |
| EBS 12.0             | 2007                  | Nova arquitetura de contabilidade (Subledger Accounting). |
| EBS 12.1             | 2009                  | Melhorias em gerenciamento de ciclo de vida e segurança.  |
| EBS 12.2.0           | 2013                  | Introdução da tecnologia **Online Patching** (ADOP).      |
| EBS 12.2.4 a 12.2.13 | 2014–2023             | Atualizações contínuas com novos recursos.                |
| EBS 12.2.14          | 2024 (previsto)       | Última versão com suporte a longo prazo.                  |
**Oracle EBS 12.2** é a única versão com **Premier Support** até **2031** (com possibilidade de extensão).

### **Tipos de Patches**

| **Tipo de Patch**            | **Descrição**                                                                 |
| ---------------------------- | ----------------------------------------------------------------------------- |
| **One-Off Patch**            | Corrige um problema específico (bug fix). Nomeado por número único.           |
| **Mini-Pack**                | Conjunto de patches relacionados a um módulo.                                 |
| **Family Pack**              | Atualização para uma família de produtos, ex: `HR_PF.F`.                      |
| **Maintenance Pack**         | Atualização cumulativa para vários módulos, ex: `11i.ATG_PF.H`                |
| **Rollup Patch (RUP)**       | Conjunto de correções aplicadas cumulativamente. Ex: `R12.HR_PF.B.DELTA.6`.   |
| **Consolidated Update (CU)** | Atualizações cumulativas que consolidam vários patches menores. Ex: `12.2.10` |
| **Technology Stack Patch**   | Atualizações no WebLogic, Forms, Java, etc.                                   |
## Estrutura de Nomeação de Patch

Patch 34600055: R12.HR_PF.C.DELTA.12

- **R12**: Release 12.
- **HR_PF**: Human Resources Product Family.
- **C**: Versão base da família.
- **DELTA.12**: Atualização incremental (Delta Patch número 12).

## **Histórico de Versões do SAP ERP**

O SAP evoluiu significativamente ao longo das décadas, acompanhando a transformação digital e mudanças tecnológicas. Veja:

| **Produto / Versão**                   | **Ano de Lançamento** | **Descrição**                                                             |
| -------------------------------------- | --------------------- | ------------------------------------------------------------------------- |
| **SAP R/2**                            | 1979                  | Sistema mainframe para grandes empresas.                                  |
| **SAP R/3 1.0**                        | 1992                  | Primeira versão cliente-servidor; revolucionou o mercado ERP.             |
| **SAP R/3 4.6C**                       | 2000                  | Muito utilizado por empresas no início dos anos 2000.                     |
| **SAP ERP 5.0**                        | 2004                  | Evolução do R/3 com integração maior.                                     |
| **SAP ERP 6.0**                        | 2006                  | Base de versões posteriores até o ECC.                                    |
| **SAP ECC 6.0 EHPx**                   | 2006–2020             | Enhancement Packages (EHP1 a EHP8); melhorias sem grandes upgrades.       |
| **SAP S/4HANA 1511**                   | 2015                  | Primeiro release do novo ERP otimizado para HANA (simplificação massiva). |
| **SAP S/4HANA 1610 – 2023**            | 2016–2023             | Releases anuais com novas funcionalidades.                                |
| **SAP S/4HANA 2023**                   | 2023                  | Última versão on-premise (até o momento).                                 |
| **SAP S/4HANA Cloud (Public/Private)** | Contínuo              | Versão com ciclos de atualização trimestrais ou semestrais.               |

## **Nomeação de Patches no SAP**

### **Tipos de Atualizações (Patches)**

| **Tipo**                        | **Descrição**                                                   |
| ------------------------------- | --------------------------------------------------------------- |
| **SAP Notes (OSS Notes)**       | Correções pontuais. Podem ser manuais ou automáticas via SNOTE. |
| **Support Package (SP)**        | Conjunto de correções de bugs e melhorias. Ex: SAP_BASIS SP17   |
| **Support Package Stack (SPS)** | Pacote coordenado de SPs para múltiplos componentes.            |
| **Enhancement Package (EHP)**   | Pacotes de funcionalidades novas. Ex: EHP8 para ECC 6.0         |
| **Feature Pack (FP)**           | Introduz novas funcionalidades em S/4HANA.                      |
| **Correction Instructions**     | Pequenos ajustes liberados via SAP Notes.                       |
| **Kernel Patches**              | Atualizações no núcleo do sistema (sapkernel).                  |

### Ferramentas úteis:

- **Maintenance Planner**
- **Download Basket**
- **SPAM/SAINT Transaction** (para aplicação de SPs)
- **SNOTE** (para SAP Notes)


# Pontos de Atenção
Em nosso contrato da solução RISE 0
**Short Distance (intra-região)** quanto **Long Distance (inter-região)** — e os impactos disso nos **objetivos de recuperação: RTO (Recovery Time Objective)** e **RPO (Recovery Point Objective)**.

| **Termo**             | **Significado**                                                                           |
| --------------------- | ----------------------------------------------------------------------------------------- |
| **RTO**               | Tempo máximo aceitável para restaurar o serviço após uma falha.                           |
| **RPO**               | Tempo máximo aceitável de perda de dados (tempo entre último backup e falha).             |
| **Short Distance DR** | Failover para um data center na mesma região metropolitana (menor latência).              |
| **Long Distance DR**  | Failover para uma região geograficamente distante (maior resiliência, mas mais latência). |

- [ ] **Se o foco é RTO/RPO baixos (<10 min)** → opte por **Short Distance** com **replicação síncrona**, com **AWS ou Azure** no Brasil (ambos oferecem múltiplas zonas).
- [ ] **Se a prioridade é máxima resiliência (desastre regional)** → **Long Distance DR** com replicação assíncrona é o ideal, mas o **custo e latência são maiores**.


## **Resumo: Avaliação Comparativa para RISE no Brasil**

|**Critério**|**Short Distance**|**Long Distance**|
|---|---|---|
|**Alta disponibilidade**|Multi-AZ (na mesma região)|Replicação entre regiões (cross-region)|
|**RTO esperado**|5 a 30 minutos|1 a 4 horas|
|**RPO esperado**|0 a 5 minutos (sync)|15 min a 1 hora (async)|
|**Impacto no custo**|Médio|Alto (link dedicado, duplicação de recursos)|
|**Provedores recomendados**|AWS, Azure, GCP (com múltiplas zonas no Brasil)|AWS, Azure, GCP (com regiões fora do Brasil)|

Objetivando efetuar um resumo dos entendimentos  para as soluções oferecidas pela SAP na solução RISE para a BB Tecnologia e Serviços, tendo como base o SBOM proposto acordado, solicito que seja respondido os seguintes questionamentos:

- [ ] A solução ofertada para a BB Tecnologia e Serviços possui os Cloud Provider - Azure, AWS e GCP, com  failover para um data center na mesma região metropolitana (Short Distance) ou para região geograficamente distante (Long Distance).
	- [ ] Pedimos que referencia as zonas de disponibilidade(SD) ou regiões geograficamente separadas (LD)?
	- [ ] Indicar a RPO para os provedores?
	- [ ] Como se dará a orquestração automática de failover.
	- [ ] Quais os relatórios de conformidade de RTO/RPO, que serão disponibilizados?
- [ ] Ciclo de atualizações intermediárias e de versões:
	- [ ] Como esta subdividida o ciclo de atualizações ( Support Package Stacks,Feature Pack Stacks e  SAP Notes), informar temporalidade e responsabilidade;
	- [ ] Qual o período minimo e máximo para mantermos a defasagem de release/versão dos ambientes contratados? (SAP S4/Hana, SAP Ariba, SAP Concur e etc)
- [ ]
No ciclo de atualizações de quem é a responsabilidade contratual pela manutenção da integração RISE with SAP (S/4HANA Cloud + Ariba/Concur), em caso de evolução das integrações dos produtos.
### **Cenário RISE with SAP (S/4HANA Cloud + Ariba/Concur)**

Se você está no **RISE with SAP**, a SAP gerencia a compatibilidade, mas é importante:
✔️ **Manter ambas as soluções (Ariba/Concur) na versão mais recente**.
✔️ **Usar SAP BTP (Integration Suite)** para evitar problemas com PI/PO legado.
✔️ **Monitorar o SAP Product Availability Matrix (PAM)** para atualizações:
🔗 [SAP PAM - Ariba](https://support.sap.com/pam)
🔗 [SAP PAM - Concur](https://www.concur.com/support)
