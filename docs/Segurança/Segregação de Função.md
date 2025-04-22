A **Segregação de Funções** (Segregation of Duties - SoD), é um princípio de controle interno que visa **minimizar riscos de fraudes, erros e conflitos de interesse** ao distribuir responsabilidades críticas entre diferentes indivíduos ou equipes. 

A ideia central é garantir que nenhuma pessoa tenha controle exclusivo sobre todas as etapas de um processo crítico, criando um sistema de **verificação cruzada** e **equilíbrio de poder**.

Essa prática é fundamental em áreas como finanças, operações, TI e compliance, onde a concentração de funções sensíveis em uma única pessoa pode levar a abusos ou falhas operacionais.

| **Área**       | **Cenário de Risco sem SoD**                               | **Aplicação da SoD**                                                         |
| -------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **Financeiro** | Um funcionário aprova despesas e emite pagamentos.         | Separar quem **aprova despesas** de quem **emite pagos**.                    |
| **TI**         | Um administrador cria usuários e aprova acesso a sistemas. | Dividir funções entre **criação de usuários** e **aprovação de permissões**. |
| **Estoque**    | Um colaborador gerencia inventário e registra perdas.      | Separar **gestão física do estoque** de **registro contábil**.               |

#### **Princípios Básicos da SoD**

1. **Separação entre Autorização, Execução e Registro**:
    - Quem **autoriza** uma transação não deve ser o mesmo que a **executa** ou **registra** (ex.: compras, pagamentos).
2. **Separação entre Custódia e Controle**:
    - Quem tem acesso físico ou lógico a ativos (dinheiro, dados) não deve ser responsável por sua contabilização.
3. **Revisão Independente**:
    - Auditorias periódicas por terceiros para validar a integridade dos processos.
#### **Controle de Acesso**
O controle de acesso autentica usuários verificando várias credenciais de login, incluindo nomes de usuários e senhas, PINs, varreduras biométricas e tokens de segurança.

| Definição    | Entenda                                                                                                                                                                                                                                                                                              |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autenticação | Processo de verificar a identidade de um usuário ou sistema antes de permitir o acesso a recursos ou informações. (Biométrica, detecção de vivacidadde, autenticação baseada em conhecimento (geração de perguntas), Verificação de senha de uso único (SMS) e Senha )                               |
| Autorização  | Controle de acesso baseado em atributos (ABAC) para granularidade incomparável. Estabeleça políticas de acesso com base em atributos do usuário, condições ambientais e características de recursos.                                                                                                 |
| Auditoria    | Ferramentas avançadas de análise de log armadas com algoritmos de aprendizado de máquina oferecem uma abordagem proativa à segurança. Elas detectam padrões e anomalias em dados de log, permitindo que você identifique ameaças potenciais ou violações de política antes que elas causem estragos. |

#### Controle de acesso em diferentes domínios

| Definição                     | Entenda                                                                                                                                                                                                                                                                                                                                                                          |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tecnologia da Informação (TI) | Para proteger dados, redes e sistemas sensíveis.                                                                                                                                                                                                                                                                                                                                 |
| Segurança Física              | Restringe a entrada em instalações seguras, gerencia o acesso de visitantes e protege áreas sensíveis.                                                                                                                                                                                                                                                                           |
| Assistência Médica            | Privacidade do paciente e protege os registros eletrônicos de saúde (EHRs) na assistência médica. O pessoal autorizado pode acessar as informações do paciente implementando medidas de controle de acesso, minimizando violações de dados e cumprindo os padrões da indústria e regulamentações de privacidade como HIPAA(Health Insurance Portability and Accountability Act), |
| Finanças e serviços bancários | Proteger dados financeiros e informações de clientes. Medidas robustas como autenticação multifator protegem contas de clientes, previnem transações não autorizadas e mitigam roubo de identidade, fraude e riscos de segurança.                                                                                                                                                |

#### Autorização
A autorização é um lugar onde controlamos o acesso, decidindo o que uma pessoa pode ou não fazer. Abaixo estão os vários tipos de autorização:

- [ ] **Controle de acesso baseado em função (RBAC)**: Atribui permissões a funções e os usuários são atribuídos a essas funções.
	- [ ] **Casos de uso**: sistemas corporativos, onde as funções de trabalho determinam o acesso.
	- [ ] Exemplo: uma função de "Gerente" tem acesso a relatórios financeiros e os funcionários nessa função herdam essas permissões.
- [ ] **Controle de acesso baseado em atributos (ABAC)**: O acesso é concedido com base nos atributos do usuário, recurso, ambiente ou ação.
	- [ ] Atributos: Departamento do usuário, sensibilidade do recurso, tempo de acesso, etc.
	- [ ] Exemplo: Um usuário só pode acessar documentos marcados com "Confidencial" se seu "nível de liberação" for "Alto".
- [ ] **Controle de Acesso Discricionário (DAC)**: O proprietário do recurso decide quem pode acessar seus recursos.
	- [ ] Exemplo: um proprietário de arquivo pode conceder acesso de leitura/gravação a usuários específicos
- [ ] **Controle de acesso obrigatório (MAC)**: O acesso é determinado por uma autoridade central com base nos níveis de classificação.
	- [ ] Exemplo: Um documento "Top Secret" só pode ser acessado por indivíduos com autorização "Top Secret".
- [ ] **Controle de acesso baseado em políticas (PBAC)**: As decisões são tomadas com base em políticas definidas pelos administradores.
	- [ ] Exemplo: o acesso é permitido se o local do usuário for "EUA" e o nível de assinatura for "Premium".
- [ ] **Controle de Acesso Baseado em Identidade (IBAC)**: O acesso é concedido diretamente a uma identidade individual, em vez de funções ou atributos.
	- [ ] Exemplo: conceder a um usuário específico acesso a um único recurso.
- [ ] **Controle de acesso refinado**: Decisões de acesso granular com base em critérios detalhados, geralmente uma combinação de ABAC e PBAC.
	- [ ] Exemplo: um usuário só pode editar seções específicas de um documento durante o horário de trabalho.
- [ ] **Controle de acesso sensível ao contexto**: Considera o contexto, como dispositivo, localização ou padrões de comportamento, para decidir o acesso.
	- [ ] Exemplo: permita o acesso somente se o usuário estiver em um dispositivo confiável em um local específico.
- [ ] **Controle de acesso Zero Trust**: "Nunca confie, sempre verifique." O acesso é avaliado continuamente, mesmo após a autenticação inicial.
	- [ ] Exemplo: um usuário é obrigado a se autenticar novamente ao acessar um recurso confidencial, mesmo em uma sessão confiável.
- [ ] **Agosto Controle de acesso baseado em uso (UBAC)**: O acesso é baseado em padrões e cotas de uso de recursos.
	- [ ] Exemplo: um usuário pode fazer upload de arquivos com um limite de até 10 GB por mês.
- [ ] **Agosto Controle de acesso baseado em tarefas (TBAC)**: O acesso é concedido com base nas tarefas que o usuário precisa executar.
	- [ ] Exemplo: Um usuário pode aprovar um documento somente se fizer parte da cadeia de tarefas de aprovação.

·