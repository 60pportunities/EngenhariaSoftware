## **Entrevistador**
Para garantir que um entrevistado se sinta tranquilo durante uma entrevista técnica, o entrevistador deve adotar uma abordagem estruturada e empática, seguindo estes passos:

- [ ] **Forneça opções de perguntas**: Permitir que os candidatos escolham entre algumas perguntas pode reduzir a ansiedade e permitir que demonstrem suas melhores habilidades.
- [ ] **Quebra-gelo inicial**: Cumprimente calorosamente e inicie com uma conversa casual, mantendo o um tom amigável e sorriso genuíno para estabelecer confiança.
- [ ] **Clareza no processo**: Explique o formato da entrevista: duração, etapas e objetivos.
- [ ] **Ambiente acolhedor**: 
	- [ ] **Presencial**: Ofereça água, certifique-se de que a sala esteja silenciosa e bem iluminada.
	- [ ] **Remoto**: Verifique a conexão, áudio e ferramentas antes de começar.
- [ ] **Comunicação Aberta**
	- [ ] Encoraje perguntas: _“Se algo não estiver claro, pode pedir para repetir ou detalhar.”_
	- [ ] Evite interromper; ouça ativamente com acenos e contato visual.
- [ ] **Abordagem colaborativa**
	- [ ] Trate a resolução de problemas como uma atividade conjunta: _“Vamos explorar juntos como resolver isso.”_
	- [ ] Permita flexibilidade: aceite linguagens ou ferramentas que o candidato prefira (se aplicável).
- [ ] **Feedback positivo**    
	- [ ] Reconheça progressos, mesmo parciais: _“Você identificou bem o ponto crítico. Vamos ver como implementar?”_
	- [ ] Normalize erros: _“Não se preocupe em acertar de primeira; queremos entender seu raciocínio.”_
- [ ] **Gestão da ansiedade**
	- [ ] Se o candidato travar, sugira uma pausa ou retomar o problema mais tarde.
	- [ ] Evite pressão excessiva: _“Respire, não há problema em levar um tempo.”_
- [ ] **Foco no processo, não só na resposta**
	- [ ] Use cenários práticos e valorize a lógica: _“Como você estruturaria essa solução considerando escalabilidade?”_
	- [ ] Pergunte sobre trade-offs e alternativas para entender a profundidade do pensamento.
- [ ] **Encerramento aberto**
	- [ ] Reserve tempo para o candidato fazer perguntas sobre a empresa, equipe ou cultura.
	- [ ] Agradeça pela participação e informe os próximos passos (ex.: prazo para feedback).
	- [ ] Explique como será a contratação (CLT, PJ, Prestador de Serviço)
	- [ ]  **Não subestime seus candidatos**: Se gostar de um candidato, faça uma oferta justa sem "joguinhos".
	- [ ] **Não brinque ao fazer uma oferta**: Seja transparente e justo na proposta salarial e benefícios.
## **Entrevistado**

- [ ] **Pesquisa sobre o papel e a empresa**: A importância de se informar sobre a empresa antes da entrevista.
- [ ] **Entrevista por telefone com o recrutador**: As perguntas geralmente focam no conhecimento de DOM (Document Object Model).
- [ ] **Desafios de Codificação**: Podem envolver duas ou três perguntas menores ou um projeto de codificação. Habilidades em desenvolvimento web, incluindo HTML, CSS e JavaScript, são testadas. A familiaridade com princípios básicos de acessibilidade web e HTML semântico (como `<nav>` e `<header>`) também é crucial.
- [ ] **Projetos de Codificação**: São prompts encapsulados para criar pequenas aplicações. É importante perguntar se esperam o uso de alguma estrutura ou biblioteca específica. Incluir fluxos de usuário, documentação e áreas de melhoria demonstra atenção aos detalhes e autoconsciência. O código deve ser organizado (arquivos CSS/Sass), performático e livre de comentários desnecessários. Exemplos de projetos incluem uma "Aplicação de Tarefas".
- [ ] **Entrevistas Técnicas Presenciais**: Visam testar o conhecimento sobre estruturas de dados e algoritmos. Um exemplo de pergunta envolve otimização de desempenho de imagens (formato Webp, carregamento lento).
- [ ] **Entrevistado**: O que fazer se ficar preso? Manter a calma, respirar e pedir ajuda ao entrevistador.

## Estruturas de Dados e Algoritmos:

- [ ] **Pilhas (Stacks)**: Estrutura de dados LIFO (Last-In, First-Out). Métodos push, pop, peek, isEmpty, getLength. Implementação em JavaScript usando a notação de classe e arrays nativos.
- [ ] **Filas (Queues)**: Estrutura de dados FIFO (First-In, First-Out). Métodos enqueue, dequeue, isEmpty, getLength, peek. Implementação em JavaScript usando arrays (push e shift).
- [ ] **Listas Ligadas (Linked Lists)**: Sequência de nós onde cada nó aponta para o próximo. Podem ser simples ou duplamente ligadas. Operações de push, pop, get (por índice).
- [ ] **Gráficos (Graphs)**: Estrutura de dados com nós e arestas. Operações de addNode, addEdge, getNode, removeNode.
- [ ] **Árvores (Trees)**: Estrutura hierárquica onde um nó pode ter zero ou mais filhos. O nó mais alto é a raiz, e nós sem filhos são folhas. A altura da árvore é a distância entre a folha mais distante e a raiz.
- [ ] **Árvores Binárias**: Cada nó tem no máximo dois filhos (esquerda e direita).
- [ ] **Árvores Binárias Completas**: Todos os níveis, exceto o último, estão completos.
- [ ] **Árvores Binárias Perfeitas**: Todos os níveis, incluindo o último, estão cheios.
- [ ] **Árvores de Busca Binárias**: Valores à esquerda são menores e valores à direita são maiores que o nó atual. Operação de addChild com lógica para evitar duplicatas. Remoção de nós com diferentes casos (folha, um filho, dois filhos).
- [ ] **Notação Big-O**: Avaliação da eficiência de algoritmos em termos de tempo e espaço, à medida que o tamanho da entrada aumenta. Descarte de constantes e termos menos significativos. Exemplos de complexidade: O(1) (tempo constante), O(log n) (tempo logarítmico - Busca Binária), O(n) (tempo linear), O(n log n), O(n²) (tempo quadrático - Bubble Sort), O(2ⁿ) (tempo exponencial - Fibonacci recursivo).
- [ ] **Travessias de Árvores**: Pré-ordem (nó atual, filho esquerdo, filho direito), em-ordem (filho esquerdo, nó atual, filho direito), pós-ordem (filho esquerdo, filho direito, nó atual).
- [ ] **Busca em Árvore**: Busca em Profundidade (DFS) e Busca em Largura (BFS). Implementação de DFS para um grafo usando uma matriz de hash para rastrear nós visitados.

## Design de Sistemas

- [ ] **Sistemas Distribuídos:** Sistemas com componentes em diferentes máquinas.
- [ ] **Escalabilidade**: Capacidade de lidar com aumento de carga.
- [ ] **Escala Vertical**: Aumentar os recursos de um único servidor.
- [ ] **Escala Horizontal**: Adicionar mais servidores.
- [ ] **Confiabilidade / Tolerância a Falhas**: Capacidade de o sistema continuar funcionando apesar de falhas (exemplo: Amazon).
- [ ] **Balanceamento de Carga**: Distribuição de tráfego entre servidores para evitar sobrecarga em um único servidor. Algoritmos: Round Robin, Menor Conexão, Hash IP, Menor Largura de Banda, Método Ponderado.
- [ ] **Cache**: Armazenamento de dados frequentemente acessados para melhorar o desempenho.
- [ ] **Invalidação de Cache**: Estratégias para atualizar o cache quando os dados mudam (Write-Through, Write-Back, Write-Around).
- [ ] **Políticas de Despejo de Cache**: Estratégias para remover itens do cache quando ele está cheio (Menos Usado Recentemente - LRU, Mais Recentemente Usado - MRU, Primeiro a Entrar, Primeiro a Sair - FIFO).
- [ ] **Particionamento de Dados**: Segmentação de um grande banco de dados para otimização.
- [ ] **Particionamento Horizontal (Sharding)**: Diferentes linhas em tabelas diferentes.
- [ ] **Particionamento Vertical**: Diferentes colunas em tabelas diferentes.

## Bancos de Dados SQL vs. NoSQL

- [ ] **Bancos de Dados SQL (Relacionais)**: MySQL, Oracle, Postgres: Armazenam dados em linhas, colunas e tabelas.
- [ ] **Bancos de Dados NoSQL (Não Relacionais)**:Bancos de Dados de Chave-Valor: Dynamo, Redis.
- [ ] **Bancos de Dados de Documentos**: CouchDB, MongoDB.
- [ ] **Bancos de Dados de Colunas Largas**: Cassandra.
- [ ] **Bancos de Dados de Gráficos**: Neo4J.
- [ ] **Higienize os dados**: Importante ao interagir com bancos de dados para evitar ataques.
- [ ] **Use ARIA**: (Accessible Rich Internet Applications) para tornar aplicações web mais acessíveis a leitores de tela.
- [ ] **Replicação**: Criação de cópias de dados para redundância e disponibilidade.

### Por fim

- [ ] **Seja honesto**: Se não souber a resposta para uma pergunta, admita e, se quiser, faça um palpite com sua justificativa.

### Grande Equipe

| Grande Equipe                        | Entenda                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ofereça oportunidades de crescimento | Promover o desenvolvimento contínuo dos membros da equipe é essencial para mantê-los motivados e engajados. Investir em treinamentos, cursos e novas responsabilidades permite que as pessoas evoluam, se sintam valorizadas e adquiram habilidades que contribuem tanto para seu crescimento profissional quanto para o sucesso da organização.                                                                                 |
| Crie um ambiente seguro              | Garantir um espaço de trabalho onde todos se sintam seguros para expressar suas opiniões e ideias sem medo de retaliações ou julgamentos é fundamental. Isso inclui promover uma cultura de respeito, inclusão e apoio, onde os colaboradores possam ser autênticos e confiar uns nos outros. Um ambiente seguro estimula a criatividade e o bem-estar emocional, o que resulta em maior produtividade e satisfação no trabalho. |
| Ofereça e busque feedback            | Oferecer feedback construtivo ajuda os colaboradores a identificar pontos de melhoria, enquanto buscar opiniões sobre o próprio desempenho demonstra abertura para evolução. Essa troca contínua contribui para um ambiente de aprendizado constante, além de fortalecer a comunicação e o relacionamento interpessoal dentro da equipe.                                                                                         |
| Incentive a colaboração              | Fomentar a colaboração entre os membros da equipe é vital para alcançar resultados mais eficazes e criativos. Através do trabalho em conjunto, é possível unir diferentes habilidades e perspectivas, criando soluções inovadoras e superando desafios de maneira mais eficiente.                                                                                                                                                |
| Defina expectativas claras           | A clareza nas metas ajuda os colaboradores a direcionarem seus esforços de maneira mais eficiente, evitando mal-entendidos e frustrações.                                                                                                                                                                                                                                                                                        |
| Incentive a inovação                 | Estimular os colaboradores a pensar fora da caixa, explorar novas ideias e adotar novas tecnologias pode resultar em soluções criativas que tragam vantagens competitivas.                                                                                                                                                                                                                                                       |
| Comunique-se abertamente             | Uma comunicação clara e transparente é a chave para a eficácia de qualquer equipe. Manter um fluxo aberto de informações evita mal-entendidos, promove o alinhamento das equipes e fortalece a confiança entre os colaboradores.                                                                                                                                                                                                 |
| Comemore pequenas vitórias           | Celebrar pequenas vitórias reforça o comprometimento e o senso de realização da equipe, além de criar um ambiente positivo e encorajador. Essas comemorações são uma maneira de mostrar que todo progresso, por menor que seja, é valorizado e contribui para o sucesso final.                                                                                                                                                   |
| Admita seus erros                    | Quando os líderes reconhecem suas falhas e assumem responsabilidades, eles demonstram vulnerabilidade e autenticidade, criando um ambiente em que todos se sentem mais à vontade para aprender com seus próprios erros.                                                                                                                                                                                                          |
| Crie conexões                        | Quando as pessoas se conectam em um nível mais pessoal, elas colaboram melhor, comunicam-se de forma mais eficaz e, muitas vezes, superam desafios juntos com mais facilidade.                                                                                                                                                                                                                                                   |
| Reconheça os esforços                | Reconhecer publicamente os avanços e o trabalho árduo demonstra respeito pelo empenho de cada membro e reforça a importância do esforço contínuo.                                                                                                                                                                                                                                                                                |
| Lidere pelo exemplo                  | Liderar pelo exemplo é um dos caminhos mais eficazes para criar uma cultura organizacional positiva. Quando os líderes demonstram comprometimento, ética e trabalho em equipe, os colaboradores tendem a seguir esse exemplo, elevando os padrões gerais da equipe.                                                                                                                                                              |
| Mostre empatia                       | A empatia é um ingrediente fundamental para um bom relacionamento interpessoal. Quando os líderes demonstram compreensão e consideração pelas dificuldades e necessidades dos membros da equipe, eles criam um ambiente mais humano e acolhedor.                                                                                                                                                                                 |
| Seja transparente                    | A transparência é crucial para construir um ambiente de confiança. Quando os líderes compartilham informações importantes, tomam decisões de forma aberta e comunicam os desafios enfrentados pela organização, eles incentivam a participação e o engajamento da equipe.                                                                                                                                                        |

