É uma abordagem leve, iterativa e integrada ao desenvolvimento ágil, que visa **identificar, analisar e mitigar ameaças de segurança** de forma contínua, ao longo do ciclo de vida do software — e não como uma etapa isolada ou final.
**Na abordagem ágil**, ela é adaptada para funcionar **em ciclos curtos** (sprints), focando no que realmente está sendo desenvolvido naquele momento, para:

- Reduzir retrabalho
- Detectar riscos cedo
- Automatizar quando possível
- Integrar segurança como uma atividade contínua

## Como funciona (visão geral)

1. **Identifique o que será desenvolvido nesta sprint**
    - Feature, módulo, API, etc.
2. **Modele possíveis ameaças sobre esse escopo**
    - Usando modelos como STRIDE, LINDDUN, CIA (Mudei para CAIA), etc.
3. **Documente e priorize os riscos**
    - Baseado no impacto e na probabilidade
4. **Crie histórias de segurança**
    - Para tratar ou mitigar as ameaças
5. **Repita em cada sprint**
    - Modelagem incremental

### **STRIDE** (Microsoft)
- Modelo mais popular, cobre 6 categorias de ameaças:
    - **S**poofing (Falsificação de identidade)
    - **T**ampering (Violação de integridade)
    - **R**epudiation (Repúdio sem rastreabilidade)
    - **I**nformation Disclosure (Vazamento)
    - **D**enial of Service (Negação de serviço)
    - **E**levation of Privilege (Elevação de privilégio)
### **CAIA** (Confidencialidade,Autenticidade,  Integridade e Disponibilidade)

- Avalia os riscos com base nos 4 pilares da segurança da informação:
    - **Confidencialidade** (ex. dados sensíveis expostos?)
    - **Autenticidade**
    - **Integridade** (ex. dados podem ser modificados?)
    - **Disponibilidade** (ex. sistema pode ser derrubado?)
### **LINDDUN** (Privacidade)
- Modelo voltado à **privacidade de dados pessoais**, cobre:
    - **L**inkability (Vinculo)
    - **I**dentifiability(Identificabilidade)
    - **N**on-repudiation(Não repúdio)
    - **D**etectability(Detecibilidade)
    - **D**isclosure of information(Divulgação de Informações)
    - **U**nauthorized actions (Ações Não autorizadas)
    - **N**on-compliance (Não conformidade)
### **PASTA** (Process for Attack Simulation and Threat Analysis)
- Definition of the Objectives: Compreender os ativos críticos da aplicação e como ela apoia os objetivos de negócio.
	- Identificação de ativos críticos, Priorização de risco de negócio e Avaliação do impacto à missão da organização.
- Definição do Escopo Técnico (Definition of the Technical Scope): Definir quais sistemas, componentes, interfaces e tecnologias estão dentro do escopo da análise.
	- Diagrama de arquitetura, Inventário de tecnologia e Identificação de interfaces e fluxos de dados.
- Decomposição da Aplicação (Application Decomposition): Compreender os fluxos de dados, atores, pontos de entrada e componentes da aplicação.
	- Diagrama de fluxo de dados, Identificação de trust boundaries (_fronteiras de confiança_), Perfis de usuário e permissões;
- Análise de Ameaças (Threat Analysis): Identificar ameaças potenciais contra os ativos e componentes da aplicação.
	- Catálogo de ameaças (baseado em STRIDE, OWASP, etc.), Mapeamento de ameaças para componentes e Avaliação de motivação de atacantes (ameaças baseadas em perfil do adversário);
- Análise de Vulnerabilidades (Vulnerability and Weakness Analysis): Identificar vulnerabilidades conhecidas e potenciais nas tecnologias e implementações.
	- Lista de vulnerabilidades (CVEs, CWE), Resultados de testes de segurança (estáticos, dinâmicos) e Correlação de vulnerabilidades com ameaças
- Simulação de Ataques (Attack Simulation): Simular como um atacante poderia explorar vulnerabilidades para atingir os ativos críticos.
	- Modelos de ataque (ex: Attack Trees, Kill Chain), Cenarios de exploração e Cadeias de ataque (TTPs – Táticas, Técnicas e Procedimentos)
- Análise de Riscos e Impacto (Risk and Impact Analysis):
### **Attack Trees / Kill Chains**
- Visão hierárquica de como um ataque pode ocorrer
- Útil para sistemas críticos e ameaças avançadas

## Exemplos práticos na abordagem ágil:

|Sprint|Feature|Ameaça STRIDE|Ação|
|---|---|---|---|
|1|Login|Spoofing|Autenticação multifator|
|2|API de pagamento|Tampering|Assinatura digital das requisições|
|3|Logs|Repudiation|Logs imutáveis com auditoria|
