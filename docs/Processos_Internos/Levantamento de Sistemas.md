### Etapa 1: Defina o escopo do seu trabalho
O primeiro passo no processo de modelagem de ameaças envolve entender o que você está fazendo. Isso pode envolver:

- Desenhar diagramas, geralmente diagramas de fluxo de dados.
- Identificar pontos de entrada para ver onde um possível invasor pode interagir com o aplicativo.
- Tentando identificar “ativos”
- Identificar níveis de confiança que representam os direitos de acesso que o aplicativo concederá a entidades externas.
- Ler uma história de usuário ou criar uma.

### Etapa 2: Determinar ameaças
A utilização de uma metodologia de categorização de ameaças é essencial para a identificação de ameaças. [STRIDE](https://en.wikipedia.org/wiki/STRIDE_%28security%29) é frequentemente usado em modelagem de ameaças, e kill chains, incluindo MITRE ATT&CK, são frequentemente usadas em modelagem de ameaças operacionais.

O objetivo da categorização de ameaças é ajudar a identificar ameaças vindas tanto do invasor ( [STRIDE](https://en.wikipedia.org/wiki/STRIDE_%28security%29) ).

### Etapa 3: Determinar contramedidas e mitigação

Uma vulnerabilidade pode ser mitigada com a implementação de uma contramedida. Tais contramedidas podem ser identificadas por meio de listas de mapeamento de ameaças e contramedidas. A priorização de contramedidas é um tópico complexo e controverso. Existem muitas abordagens, e as organizações precisam selecionar aquelas que funcionam para elas. Os fatores frequentemente incluídos são a probabilidade de ataque, os danos causados ​​por um ataque e a complexidade ou o custo da correção.

A estratégia de mitigação de riscos pode envolver a avaliação dessas ameaças com base no impacto que elas representam para os negócios. Uma vez identificado o possível impacto, as opções para lidar com o risco incluem:

- Aceitar: decidir que o impacto comercial é aceitável e documentar quem escolheu aceitar o risco
- Eliminar: remover componentes que tornam a vulnerabilidade possível
- Mitigar: adicionar verificações ou controles que reduzam o impacto do risco ou as chances de sua ocorrência
- Transferência: transferir risco para uma seguradora ou cliente.


Os documentos de modelo de ameaça em cascata ou entregues por consultores geralmente incluem o seguinte:

1. **Nome do aplicativo** : O nome do aplicativo examinado.
2. **Versão do aplicativo** : a versão do aplicativo examinado.
3. **Descrição** : Uma descrição de alto nível do aplicativo.
4. **Proprietário do documento** : o proprietário do documento de modelagem de ameaças.
5. **Participantes** : Os participantes envolvidos no processo de modelagem de ameaças para este aplicativo.
6. **Revisor** : o(s) revisor(es) do modelo de ameaça.


### Ativos

Muitos possuem algo no qual um ou mais invasores estão interessados; esses itens ou áreas de interesse são frequentemente rotulados como "ativos". Ativos podem ser tanto ativos físicos quanto abstratos.

Os ativos são documentados neste modelo de ameaça de amostra da seguinte forma:

1. **ID** : Um ID exclusivo é atribuído para identificar cada ativo. Ele será usado para fazer referência cruzada do ativo com quaisquer ameaças ou vulnerabilidades identificadas.
2. **Nome** : Um nome descritivo que identifica claramente o ativo.
3. **Descrição** : Uma descrição textual do que é o ativo e por que ele precisa ser protegido.
4. **Níveis de Confiança** : O nível de acesso necessário para acessar o ponto de entrada está documentado aqui. Estes serão referenciados com os níveis de confiança definidos na próxima etapa.

### Níveis de confiança

Os níveis de confiança representam os direitos de acesso que o aplicativo concederá a entidades externas. Os níveis de confiança são referenciados de forma cruzada com os pontos de entrada e ativos.

Os níveis de confiança são documentados no modelo de ameaça da seguinte forma:

1. **ID** : Um número exclusivo é atribuído a cada nível de confiança. Ele é usado para fazer referência cruzada do nível de confiança com os pontos de entrada e ativos.
2. **Nome** : Um nome descritivo que permite identificar as entidades externas que receberam esse nível de confiança.
3. **Descrição** : Uma descrição textual do nível de confiança detalhando a entidade externa à qual o nível de confiança foi concedido.

## Determine as Ameaças
Um mnemônico de ameaças como o STRIDE é útil na identificação de ameaças, pois nos leva a pensar sobre as etapas do invasor, como:

## Lista de ameaças STRIDE

| Tipo                                               | Descrição                                                                                                                                                                                                            | Controle de Segurança |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| Spoofing (Falsificação)                            | Ação de ameaça que visa acessar e utilizar credenciais de outro usuário, como nome de usuário e senha.                                                                                                               | Autenticação          |
| Tampering(Adulteração)                             | Ação de ameaça que visa alterar ou modificar maliciosamente dados persistentes, como registros em um banco de dados, e a alteração de dados em trânsito entre dois computadores em uma rede aberta, como a Internet. | Integridade           |
| Repudiation(Repúdio)                               | Ação de ameaça que visa executar operações proibidas em um sistema que não tem capacidade de rastrear as operações.                                                                                                  | Não-Repúdio           |
| Information disclosure (Divulgação de informações) | Ação de ameaça com a intenção de ler um arquivo ao qual não foi concedido acesso ou de ler dados em trânsito.                                                                                                        | Confidencialidade     |
| Denial of service (Negação de serviço)             | Ação de ameaça que tenta negar acesso a usuários válidos, como tornar um servidor web temporariamente indisponível ou inutilizável.                                                                                  | Disponibilidade       |
| Elevation of privilege(Elevação de privilégio)     | Ação de ameaça que visa obter acesso privilegiado a recursos para obter acesso não autorizado a informações ou comprometer um sistema.                                                                               | Autorização           |

[Supply chain Levels for Software Artifacts](https://slsa.dev),

## Trust boundary (Limite da Confiança)

![[Pasted image 20250524062459.png]]

Para cada Par Poderíamos Ter


| Tipo                                               | Forças | Ameaças                                                 |
| -------------------------------------------------- | ------ | ------------------------------------------------------- |
| Spoofing (Falsificação)                            |        | VULN01: Modificar prompt do sistema (injeção de prompt) |
| Tampering(Adulteração)                             |        | VULN02: Modificar parâmetros LLM (temperatura, comprimento, modelo, etc.)                                                |
| Repudiation(Repúdio)                               |        |                                                         |
| Information disclosure (Divulgação de informações) |        |                                                         |
| Denial of service (Negação de serviço)             |        |                                                         |
| Elevation of privilege(Elevação de privilégio)     |        |                                                         |

**Lista completa de vulnerabilidades**

|                           |                                                                                             |                                                                                                                                                                                   |
| ------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ID da vulnerabilidade** | **Descrição**                                                                               | **Exemplos**                                                                                                                                                                      |
| VULN01                    | Modificar prompt do sistema (injeção de prompt)                                             | Os usuários podem modificar as restrições de prompt no nível do sistema para "desbloquear" o LLM e substituir os controles anteriores.                                            |
| VULN02                    | Modificar parâmetros LLM (temperatura, comprimento, modelo, etc.)                           | Os usuários podem modificar os parâmetros da API como entrada para o LLM, como temperatura, número de tokens retornados e modelo em uso.                                          |
| VULN03                    | Inserir informações confidenciais em um site de terceiros (comportamento do usuário)        | Os usuários podem, consciente ou inconscientemente, enviar informações privadas, como detalhes da HIPAA ou segredos comerciais, para LLMs.                                        |
| VULN04                    | Os LLMs não conseguem filtrar informações sensíveis (área de pesquisa aberta)               | Os LLMs não conseguem ocultar informações sensíveis. Qualquer coisa apresentada a um LLM pode ser recuperada por um usuário. Esta é uma área de pesquisa em aberto.               |
| VULN05                    | Saída controlada por entrada de prompt (não filtrada)                                       | A saída do LLM pode ser controlada por usuários e entidades externas. A aceitação não filtrada da saída do LLM pode levar à execução indesejada de código.                        |
| VULN06                    | A saída do lado do servidor pode ser alimentada diretamente de volta ao LLM (requer filtro) | A entrada irrestrita de funções do lado do servidor pode resultar em divulgação de informações confidenciais ou SSRF. Controles do lado do servidor mitigariam esse impacto.      |
| VULN07                    | Acesso a informações sensíveis                                                              | Os LLMs não têm o conceito de autorização ou confidencialidade. O acesso irrestrito a bancos de dados privados permitiria que os usuários recuperassem informações confidenciais. |

**Lista completa de recomendações**

|               |                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ID do REC** | **Recomendações**                                                                                                                                                                                                                                                                                                                                                                                  |
| REC01         | Não há muito que possamos fazer diretamente, mas podemos mitigar os efeitos posteriores. Garantir que o LLM não seja treinado com dados não públicos ou confidenciais. Além disso, tratar todas as saídas do LLM como não confiáveis ​​e aplicar as restrições necessárias aos dados ou ações solicitadas pelo LLM.                                                                                |
| REC02         | Limite a superfície de ataque da API exposta a fontes externas de prompts (usuários, conteúdo de sites, corpos de e-mail, etc.). Como sempre, trate as entradas externas como não confiáveis ​​e aplique filtragem quando apropriado.                                                                                                                                                              |
| REC03         | Este é um problema de comportamento do usuário, mas podemos educá-los por meio de declarações apresentadas durante o processo de inscrição e por meio de notificações claras e consistentes sempre que um usuário se conecta ao LLM.                                                                                                                                                               |
| REC04         | Não treine LLMs em dados sensíveis aos quais todos os usuários não devem ter acesso. Além disso, não confie nos LLMs para impor controles de autorização às fontes de dados. Em vez disso, aplique esses controles às próprias fontes de dados.                                                                                                                                                    |
| REC05         | Trate todas as saídas do LLM como não confiáveis ​​e aplique as restrições apropriadas antes de usar os resultados como entrada para funções adicionais. Isso atenuará o impacto que um prompt criado com códigos maliciosos poderia ter nas funções e serviços do ambiente interno.                                                                                                               |
| REC06         | Execute a filtragem adequada na saída da função do lado do servidor. Se o LLM armazenar a saída para dados de treinamento futuros, certifique-se de que as informações confidenciais sejam higienizadas antes do retreinamento. Se o LLM retornar a saída da função (em qualquer formato) para um usuário, certifique-se de que as informações confidenciais sejam removidas antes de retorná-las. |
| REC07         | Trate o acesso do LLM como se fosse de um usuário típico. Aplique controles padrão de autenticação/autorização antes do acesso aos dados. Os LLMs não têm como proteger informações confidenciais de usuários não autorizados, portanto, os controles devem ser implementados aqui.                                                                                                                |

Elabore um Software Development Life Cycle, em mermaid que leve em consideração:
- Concepção, ou seja, a selecção e a priorização do Projeto;
- Inicialização do Projeto
- Desenvolva um Plano de Requisitos
	- Funcionais
	- Não Funcionais
	- Lista de Ameaças (Stride)
- Análise de Riscos
	- Identificação
	- Estratégia de mitigação
- Protótipos
- Design Detalhamento
- Registros de Decisão da Arquitetura
- Estruturação do Código
	- Front-End
	- Back-End
- Estratégia de Branch
- Estratégias de Integração
- Estratégia de Documentação
- Estratégia de Teste
- Estratégia de Implantação
- Verificação e Validação


```mermaid
graph TD
    A[Concepção<br/>Seleção e Priorização do Projeto] --> B[Inicialização do Projeto]
    B --> C[Plano de Requisitos]
    C --> C1[Requisitos Funcionais]
    C --> C2[Requisitos Não Funcionais]
    C --> C3[Lista de Ameaças (STRIDE)]

    C --> D[Análise de Riscos]
    D --> D1[Identificação de Riscos]
    D --> D2[Estratégias de Mitigação]

    D --> E[Protótipos]
    E --> F[Design e Detalhamento]
    F --> G[Registros de Decisão da Arquitetura]

    G --> H[Estruturação do Código]
    H --> H1[Front-End]
    H --> H2[Back-End]

    H --> I[Estratégia de Branch]
    I --> J[Estratégias de Integração]
    J --> K[Estratégia de Documentação]
    K --> L[Estratégia de Teste]
    L --> M[Estratégia de Implantação]
    M --> N[Verificação e Validação]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style C fill:#ccf,stroke:#333,stroke-width:1px
    style D fill:#ccf,stroke:#333,stroke-width:1px
    style E fill:#cfc,stroke:#333,stroke-width:1px
    style F fill:#cff,stroke:#333,stroke-width:1px
    style G fill:#fcf,stroke:#333,stroke-width:1px
    style H fill:#ffc,stroke:#333,stroke-width:1px
    style I fill:#eef,stroke:#333,stroke-width:1px
    style J fill:#eef,stroke:#333,stroke-width:1px
    style K fill:#eef,stroke:#333,stroke-width:1px
    style L fill:#efe,stroke:#333,stroke-width:1px
    style M fill:#cfe,stroke:#333,stroke-width:1px
    style N fill:#dfd,stroke:#333,stroke-width:2px

```
