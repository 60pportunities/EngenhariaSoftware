A transição de software para a equipe de sustentação é uma etapa crítica no ciclo de vida do desenvolvimento de software.

Essa transição geralmente envolve uma série de atividades para garantir que o projeto seja entregue com sucesso e que a equipe de sustentação possa assumir a responsabilidade pela operação contínua do software.

Para o serviço de sustentação ser eficaz e efetivo, ele esta sendo dividido em grupos específicos:

| MOTS/COTS/SI/OSS | Tipo        |        N1         | N2                | N3                | Master          |
| ---------------- | ----------- | :---------------: | ----------------- | ----------------- | --------------- |
| XxxxxxxxxxxX     | Incidente   | Suporte Técnico 1 | Funcional/Projeto | Funcional/Projeto | Account Manager |
|                  | Solicitação |       ----        | Projeto           |                   | PO Prioriza     |
|                  | Projeto     |       ----        | Funcional/Projeto |                   | PO Prioriza     |
| XxxxxxxxxxxX     | Incidente   | Suporte Técnico 1 | Funcional/Projeto | Funcional/Projeto | Account Manager |
|                  | Solicitação |       ----        | Projeto           |                   | PO Prioriza     |
|                  | Projeto     |       ----        | Funcional/Projeto |                   | PO Prioriza     |
| XxxxxxxxxxxX     | Incidente   | Suporte Técnico 1 | Funcional/Projeto | Funcional/Projeto | Account Manager |
|                  | Solicitação |       ----        | Projeto           |                   | PO Prioriza     |
|                  | Projeto     |       ----        | Funcional/Projeto |                   | PO Prioriza     |
| XxxxxxxxxxxX     | Incidente   | Suporte Técnico 1 | Funcional/Projeto | Funcional/Projeto | Account Manager |
|                  | Solicitação |       ----        | Funcional/Projeto | Funcional/Projeto | PO Prioriza     |
|                  | Projeto     |       ----        | Funcional/Projeto | Funcional/Projeto | PO Prioriza     |

Alguns passos comuns nesse processo:

| Processo                                              | Entenda                                                                                                                                                                                                                       |
| ----------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Documentação**                                      | Dê acesso aos membros da sustentação e inclua o time no projeto, para que eles possam ler o material.                                                                                                                         |
| **Treinamento**                                       | A sustentação ser devidamente treinada para lidar com os problemas que podem surgir após o lançamento do software.                                                                                                            |
| **Sessões de transferência de conhecimento**          | O PO/SM deverão transferir conhecimento para a equipe de sustentação. Deve ser feito por meio de sessões de treinamento, documentação detalhada e acompanhamento para responder a perguntas e resolver problemas específicos. |
| **Ambiente de desenvolvimento e teste compartilhado** | Garanta que a equipe de sustentação tenha acesso total ao ambiente de desenvolvimento e teste. Isso permite que eles pratiquem e experimentem sem medo de causar danos aos sistemas de produção.                              |
| **Processos de Suporte**                              | Processos claros para o suporte ao software, incluindo como os tickets de suporte são criados, priorizados e resolvidos.                                                                                                      |
| **Monitoramento e Melhoria Contínua**                 | Crucial monitorar o desempenho do suporte e coletar feedback dos usuários para identificar áreas de melhoria.                                                                                                                 |
| **Suporte contínuo**                                  | Canais abertos de comunicação entre a equipe de desenvolvimento e a equipe de sustentação.                                                                                                                                    |
| **Avaliação e ajuste**                                | Solicite feedback da equipe de sustentação sobre o que está funcionando bem e onde podem haver áreas de melhoria.                                                                                                             |
| **Integração**                                        | Abertura e vinculação no OTRS do Incidente ao Produto, indicando um funcional para a realização do N2.                                                                                                                        |

No cotidiano do funcionário responsável, estão as seguintes atividades de sustentação:

- [ ] Monitorar a satisfação dos usuários em relação aos atendimentos;
- [ ] Investigar e diagnosticar incidentes;
- [ ] Aprovar ou rejeitar a correção;
- [ ] Acompanhar todo o ciclo de vida do incidente: da abertura até o encerramento, controlando os SLAs
- [ ] Identificar e registrar workarounds, data-fix e etc;
- [ ] Manter atualizada a base de conhecimento com as soluções;
- [ ] Fechar os chamados SEM a devida resposta ou contato em um prazo de 3 dias úteis;

## Processo de Classificação e Metrificação

- [ ] O Suporte Técnico 1 ao receber a demanda de "ACESSO A BANCO DE DADOS", deverá colocar uma NOTA:
```Pedido deverá ser SOLICITADO para o PRODUCT OWNER e este deverá criar um CHAMADO com os DADOS a serem liberados.```
- [ ] O Suporte Técnico 1, deverá atribuir ao usuário 'app-peoplesoftad@60opt.com.br', desde que não seja CONFIGURAÇÃO de Aplicativos MOTS, todas as SOLICITAÇÕES DE DEMANDA;
- [ ] Processo de Atendimento Acordado;
- [ ] Métricas;
