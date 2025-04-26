
```mermaid
graph TD
A[Iniciar/Clonar] --> B[Trabalhar no Código]
B --> C[Adicionar Alterações]
C --> D[Commit]
D --> E[Sincronizar com Remoto]
E --> F[Finalizado]
```

```mermaid
graph TD

```
```mermaid
   flowchart
   subgraph ideia
      r1(Req-APP-01) & r2(Req-APP-02) & rn(Req-APP-nn) --> A
      A@{ shape: div-rect, label: "Feature Flag" }
      ADM@{ shape: lin-cyl, label: "Regras Feature Flag" }
      A <-->ADM
   end
```

```mermaid
flowchart
subgraph ideia
r1(Request) --> feature-flag
subgraph feature-flag
A@{ shape: div-rect, label: "Alvo" }
A --> P1(true)
A --> P2(false)
end
P1 & P2 <--> B@{ shape: lin-cyl, label: "Regras Feature Flag" }
end
```

```mermaid
graph TD

A[Iniciar/Clonar] --> B[Trabalhar no Código]

B --> C[Adicionar Alterações]

C --> D[Commit]

D --> E[Sincronizar com Remoto]

E --> F[Finalizado]



subgraph Comandos Básicos

A[Iniciar/Clonar] -->|git init| A1["Inicializa repositório"]

A -->|git clone <url>| A2["Clona repositório remoto"]

B -->|Editar arquivos| B1["Modificações no código"]

C -->|git add <arquivo>| C1["Prepara arquivos para commit"]

C -->|git add .| C2["Prepara todas as alterações"]

D[Commit] -->|git commit -m 'Mensagem'| D1["Registra alterações no histórico"]

E[Sincronizar com Remoto] -->|git push| E1["Envia commits para o remoto"]

E -->|git pull| E2["Atualiza do remoto"]

end



subgraph Branching

G[git branch <nome>] --> H["Cria nova branch"]

I[git checkout <branch>] --> J["Muda para branch"]

K[git merge <branch>] --> L["Combina branches"]

end



subgraph Consultas

M[git status] --> M1["Verifica estado do repositório"]

N[git log] --> N1["Exibe histórico de commits"]

O[git diff] --> O1["Mostra diferenças não commitadas"]

end



subgraph Remoto

P[git remote add <nome> <url>] --> P1["Adiciona repositório remoto"]

Q[git fetch] --> Q1["Busca alterações do remoto"]

end
```

# Requisitos de Arquitetura

[![](https://mermaid.ink/img/pako:eNp1U8tuGzEM_BVhTwkQIEDRk1E0MNYueogRxBs0F1_oFS2zWYkbPdI6QT6m6KGnnoJ-wf5YGNv7gJ3eRM4MOaSkp6xkjdkos-S0hXrhlPLM8eRk6iI6jf7T-dJ_ZuXQNC8l8enpG0WpLxDZY1D3CbeMnCtYsge7g5W6ZGfUmoLQNm2uQBdY5WxTRxuLSINBq75yJWwqoYW-UWh-c0eMFJNGlfvmb8-6TkBBQRB_JYZAGjSGVjKVcha8SiE1vzxxB2x1LnK4OMhIoejBBWj-NP_wAK4Uq4i25u3AYkXmrzlEuDhsWMqETjxKlX4ApeZYQWxexMmgcDErBtHtGmIY1_UgdYNgWydtgxssHVdsqFvW-DF57EUTfOB6MG_OMhw59GLCyJr7O7kkuWg_8MPOgb9Oy67aLS4L9A9U4qDg1XxStNFVkqUNsAlEuGTQfcbeaS4HjDZjofQc6ioZcseoqcis45J_viNEb4H0h_9J_fbthh9gDPpj0h7YsY7VezhRBPNOb3K02hwWreg-0RICDgX9WYR3fasin3WQodid5eFYio_ohqjl77SLJwRGvli_69l0fj6Zztsw_6hm8p2rDt5tSWxkZ9l-ZfLXn97wRRbXaHGRjeSocQWpiots4Z6FCilysXFlNoo-4VmWag0R992z0QqqgM-vXmNQaA?type=png)](https://mermaid.live/edit#pako:eNp1U8tuGzEM_BVhTwkQIEDRk1E0MNYueogRxBs0F1_oFS2zWYkbPdI6QT6m6KGnnoJ-wf5YGNv7gJ3eRM4MOaSkp6xkjdkos-S0hXrhlPLM8eRk6iI6jf7T-dJ_ZuXQNC8l8enpG0WpLxDZY1D3CbeMnCtYsge7g5W6ZGfUmoLQNm2uQBdY5WxTRxuLSINBq75yJWwqoYW-UWh-c0eMFJNGlfvmb8-6TkBBQRB_JYZAGjSGVjKVcha8SiE1vzxxB2x1LnK4OMhIoejBBWj-NP_wAK4Uq4i25u3AYkXmrzlEuDhsWMqETjxKlX4ApeZYQWxexMmgcDErBtHtGmIY1_UgdYNgWydtgxssHVdsqFvW-DF57EUTfOB6MG_OMhw59GLCyJr7O7kkuWg_8MPOgb9Oy67aLS4L9A9U4qDg1XxStNFVkqUNsAlEuGTQfcbeaS4HjDZjofQc6ioZcseoqcis45J_viNEb4H0h_9J_fbthh9gDPpj0h7YsY7VezhRBPNOb3K02hwWreg-0RICDgX9WYR3fasin3WQodid5eFYio_ohqjl77SLJwRGvli_69l0fj6Zztsw_6hm8p2rDt5tSWxkZ9l-ZfLXn97wRRbXaHGRjeSocQWpiots4Z6FCilysXFlNoo-4VmWag0R992z0QqqgM-vXmNQaA){width="1200" height="300" style="display: block; margin: 0 auto"}
CI/CD Pipelines

1 Software development Lifecycle




-------------------------- Develop ----------------------

Staged Changes (Changes tracked by git) --> Commit (Changes are informed to git) --> Push --> E2E Tests (This is where) --> Deploy(happens...)



2 CI/CD

Continuous Integration. | Continuous Delivery



* Build and test if code in commit works well with other components

*If everything is okay so far deploy & package

$ git clone repo

/-> Unit Test

Checkout Repo --> Build --> integration TesT --> deploy --> package

\-> Test on \-> Loging Monitoring



Every step is triggered one after the other of

in parallel, thus called

as pipelines
