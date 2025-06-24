**Engenharia de Software** é a disciplina da computação que trata da aplicação sistemática de princípios, técnicas e métodos de engenharia para o desenvolvimento, operação e manutenção de software. Ela busca garantir que o **software seja construído com qualidade, dentro do prazo e orçamento**, atendendo às necessidades do usuário final.

## Principais objetivos:

- [ ] Criar software **confiável**, **eficiente** e **escalável**
- [ ]  Reduzir **custos de desenvolvimento e manutenção**
- [ ] Melhorar a **produtividade e previsibilidade**
- [ ] Promover a **colaboração entre equipes técnicas e de negócio**

```mermaid
flowchart TD
    A[Planejamento<br>Requisitos MVP] --> B[Design Arquitetural<br>Arquitetura de Software]
    B --> B1[Definição de Arquitetura<br>Camadas - Estilo - Padrões]
    B1 --> B2[Registros de Decisão - ADRs<br>trade-offs - justificativas]
    B2 --> C[Implementação<br>Git - TDD - CI/CD]
    C --> D[Testes<br>Unitários - Integração]
    D --> E[Deploy<br>CI/CD Automatizado]
    E --> F[Produção<br>Monitoramento - Logs - Alertas]

    subgraph SRE[Site Reliability Engineering]
        G[SLIs e SLOs]
        H[Observabilidade Logs - Traces]
        I[Gestão de Incidentes]
        J[Automação de Tarefas Toil Reduction]
        K[Postmortem e Feedback]
    end

    F --> G
    F --> H
    F --> I
    I --> J
    I --> K
    K --> A

    %% Estilos
    style SRE fill:#fdf6e3,stroke:#d33682,stroke-width:2px
    style A fill:#e0f7fa
    style F fill:#ffe0b2
    style B1 fill:#ede7f6,stroke:#7e57c2
    style B2 fill:#f3e5f5,stroke:#ab47bc

```


- [ ] **Toil Reduction** é a prática de **reduzir o trabalho repetitivo, manual, e operacional** que **não agrega valor direto ao usuário**, mas que é necessário para manter os sistemas funcionando. Essa ideia vem do **Site Reliability Engineering (SRE)**, criado pelo Google.
- [ ]
