https://www.stateofdocs.com/2025/introduction-basic-stats
## O que precisa ser documentado para uma API
Uma API é uma linguagem de codificação. Linguagens de codificação são semelhantes às linguagens naturais, pois seguem regras tanto de estrutura quanto de uso. A diferença é que as regras são rígidas e inflexíveis, devendo ser seguidas à risca para que o código funcione. Para usar uma API com sucesso, um programador precisa conhecer a _sintaxe_ e _a semântica_ da linguagem em que a API foi escrita, bem como as regras específicas que se aplicam aos elementos da API dentro dessa linguagem.

- [ ] **Sintaxe** é a _estrutura_ dos elementos:
	- [ ] Nomes dos elementos;
	- [ ] Requisitos de pedido e tipo;
	- [ ] Regras de construção para declarações;
- [ ] **Semântica** é o _significado_ dos elementos:
	- [ ]  Como os elementos estão relacionados
	- [ ] Que afirmações fazem

A função principal de uma referência de API é descrever a sintaxe e a semântica dos elementos públicos da API, com detalhes suficientes para que um programador possa usar a linguagem corretamente para escrever código funcional.

Este documento em particular destina-se especificamente a ser usado como _referência_ . Você pode esperar que um programador ou desenvolvedor o utilize durante a codificação para procurar a sintaxe exata ou o elemento da linguagem que precisa usar, conforme necessário. Para usar o elemento corretamente, no entanto, eles precisam entender mais do que a sintaxe. Eles precisam saber, por exemplo, o que cada valor possível de cada entrada significa e como esse valor afeta o resultado da chamada.

Os desenvolvedores precisam conhecer nuances de significado que podem não ser óbvias no código. Considere, por exemplo, uma propriedade definida como **nome** . Seu significado provavelmente é óbvio para o desenvolvedor que a nomeou e, se ele fornecer uma descrição, pode ser:

`**@param name** O nome do widget.`

Essa descrição não é mais útil do que o próprio nome da propriedade, porque não esclarece o contexto e a intenção que o desenvolvedor presumiu serem óbvios.

Uma descrição adequada agrega _valor_ e _elimina ambiguidades_ . Uma descrição em material de referência deve ser o mais explícita e específica possível, mas ainda assim ser apresentada em linguagem concisa e direta. Por exemplo, esta propriedade pode ser usada para significar qualquer um dos seguintes:

**Nome da propriedade e seus possíveis significados**

| Propriedade | Descrição                                                                                                             |
| ----------- | --------------------------------------------------------------------------------------------------------------------- |
| **nome**    | Uma sequência de exibição localizável.                                                                                |
| **nome**    | Um rótulo de exibição descritivo.                                                                                     |
| **nome**    | Uma sequência de identificação, única dentro do escopo da solicitação.                                                |
| **nome**    | Um identificador opaco gerado, conforme retornado pela função de criação.                                             |
| **nome**    | Um identificador exclusivo definido pelo desenvolvedor usado para associar uma resposta a uma solicitação específica. |

Esse tipo de descrição adiciona informações sobre a fonte, o uso esperado e as restrições à informação transmitida. Aumenta significativamente a probabilidade de o elemento descrito ser compreendido imediatamente e utilizado corretamente por usuários novos e experientes.

##  Conteúdo de referência da API vs. conteúdo para outros tipos de documentos
Para usar uma API, um programador precisa ter acesso a ela e entender o ambiente em que ela é utilizada.
Os _casos de uso_ da sua API e as _tarefas que_ ela possibilita dentro do seu domínio e dentro de um ambiente de desenvolvimento específico constituem o **contexto** para os detalhes de referência factuais sobre como fazer chamadas.

É importante que uma referência de API estabeleça contexto suficiente para tornar os detalhes técnicos úteis aos desenvolvedores.
O contexto define para que serve a API, quais recursos ela possui e o que o desenvolvedor deve fazer com ela. Para quem não está familiarizado com ela, pode ser muito difícil entender o contexto geral apenas com base em detalhes técnicos.

Informações introdutórias e semânticas de alto nível na referência fornecem contexto para as informações de sintaxe específicas de baixo nível. Isso se aplica tanto à API como um todo quanto a cada elemento.

- [ ] Uma referência de API deve fornecer uma visão geral do que a API faz e para que é usada, bem como descrições introdutórias que descrevam o que cada elemento principal faz e para que é usado.
- [ ] Uma referência de API deve incluir **exemplos de código na forma de snippets que ilustrem o uso correto de elementos específicos e valores de parâmetros especiais**.
- [ ] O texto introdutório deve esclarecer o que cada exemplo demonstra.
- [ ] Uma referência de API **não** é o lugar para tutoriais, exemplos extensos ou discussões conceituais aprofundadas. Esses elementos são importantes e devem ser fornecidos em algum lugar da documentação do produto — mas não na referência de API. Se um documento conceitual e de uso estiver disponível, a referência deve conter links ou indicações para ele.

## Requisitos de documentação da API
Um documento de referência de API deve fornecer informações básicas sobre como acessar e usar a API associada, e quais conhecimentos prévios ou preparação são necessários. Para usar uma API REST, por exemplo, espera-se que os desenvolvedores saibam como usar o protocolo HTTP/HTTPS e o formato de transferência de dados (como JSON). A referência precisa fornecer detalhes específicos de autenticação e autorização, além do URI base para os recursos. As informações básicas de uso também incluem informações como idiomas e plataformas suportados, tratamento de erros, como obter resultados paginados, e assim por diante.

Além desse material introdutório, a referência deve fornecer detalhes sintáticos completos e descrições semânticas de cada elemento público. Os elementos específicos que precisam ser documentados são diferentes para cada tipo de API.

Existem três tipos básicos de API: Código nativo, REST e linha de comando.

As estruturas e os casos de uso dessas APIs são diferentes. Elas usam terminologias diferentes e têm requisitos de documentação diferentes.

### Tipos de API

| Tipo                          | Entenda                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| APIs de código nativo         | Código nativo é a linguagem na qual um aplicativo ou sistema é (ou pode ser) escrito. Uma API oferece aos desenvolvedores uma maneira de estender o sistema ou controlá-lo programaticamente. Para um aplicativo de código aberto, uma referência completa à API é essencial para permitir contribuições da comunidade.<br><br>Esse tipo de API tende a ser mais complexo do que APIs REST e linguagens de comando. APIs de código nativo podem incluir ferramentas para formular solicitações REST e lidar com respostas.<br><br>- Uma API pode estar em uma linguagem compilada, como C/C++ ou Java, ou em uma linguagem interpretada (de script), como JavaScript/Typescript. APIs de script podem estar disponíveis em diferentes linguagens para o mesmo aplicativo e, normalmente, se comunicam com aplicativos ou sistemas criados em uma linguagem compilada.<br>- **APIs de** código nativo podem usar uma abordagem orientada a objetos ou uma abordagem orientada a funções (tecnicamente chamada de DSL, ou **Linguagem** Específica de Domínio **)** . Essas abordagens não são mutuamente exclusivas, mas as duas abordagens têm necessidades de documentação ligeiramente diferentes. A maioria das linguagens modernas é otimizada para o estilo de programação orientada a objetos. Os principais elementos a serem documentados são classes com métodos e propriedades, funções de nível superior e estruturas de dados.                                                                                                                                                                                                                                                                               |
| APIs REST                     | REST (Representational State Transfer Architecture) fornece um protocolo para comunicação via HTTP. Uma API RESTful define chamadas específicas usando esse protocolo.<br><br>A [especificação OpenAPI (OAS)](https://www.openapis.org/) é um padrão de fato para a criação de APIs REST e é muito popular na comunidade OSS. A iniciativa OpenAPI (OAI) não utiliza o termo REST, mas a terminologia e os requisitos de documentação são os mesmos.<br><br>As APIs REST são atualmente o tipo mais comum de API em produção que requer documentação pública. A API REST se comunica entre sistemas escritos em código nativo — geralmente um cliente e um servidor. As chamadas de API normalmente enviam dados entre aplicativos, mas também podem emitir instruções para iniciar alguma ação em ambas as extremidades.<br><br>Para usar uma API REST, você precisa ter sistemas de código nativo em ambas as extremidades para formular solicitações e processar respostas, e para produzir ou utilizar os dados transmitidos. A linguagem usada para formular chamadas é irrelevante para os detalhes sintáticos e semânticos das solicitações, respostas e esquemas de dados. Um programador pode formular chamadas em diversas linguagens de codificação, incluindo muitas linguagens modernas otimizadas para esse fim. A documentação normalmente inclui exemplos em diversas linguagens comuns, como Python, C++, Java, JavaScript, TypeScript, Ruby, Go e assim por diante.<br><br>Os principais elementos a serem documentados para uma API REST são _recursos_ com _endpoints_ , _operações_ suportadas para cada endpoint, sintaxe _de solicitação_ e _resposta_ para cada operação e _esquemas de dados_ . |
| Interface de linha de comando | Uma interface de linha de comando (CLI) é semelhante a uma API REST, pois é usada para emitir comandos parametrizados para um sistema. A diferença é que uma API REST se comunica com um aplicativo ou servidor por meio de uma conexão de rede, enquanto uma CLI se comunica com um servidor diretamente por meio de um script ou shell de comando.<br><br>As CLIs são geralmente usadas por administradores para configuração do sistema ou por desenvolvedores durante o desenvolvimento do sistema. Elas podem ser usadas para escrever scripts de automação para um aplicativo.<br><br>Uma CLI é um conjunto de _comandos_ . Os comandos recebem _entradas_ (argumentos, opções e sinalizadores), executam uma ação e podem ou não produzir _uma saída_ . _Argumentos_ são parâmetros para o comando. _Opções_ são argumentos opcionais que regem o comportamento do comando e podem ou não receber parâmetros próprios. Opções que não recebem parâmetros são _sinalizadores_ .<br><br>_**NOTA** : Não é incomum que o mesmo produto forneça APIs de diferentes tipos. Um produto pode ter APIs de código nativo em diferentes linguagens, além de uma CLI para configuração ou administração e uma API REST para comunicação cliente-servidor — e talvez uma API de script para gerar solicitações REST e lidar com respostas._                                                                                                                                                                                                                                                                                                                                                                                   |

# Elementos que requerem documentação de referência

Cada tipo de API usa terminologia diferente e tem requisitos de documentação diferentes.

**Tipos e elementos da API**

|Tipo de API|Elementos|
|---|---|
|API REST|Para uma API REST, a referência deve documentar os seguintes elementos públicos:<br><br>- Listar _recursos_ e _endpoints_  <br>    disponíveis - Descrever requisitos _de acesso e autorização_  <br>    - Listar _operações HTTP_ suportadas para cada endpoint<br>- Para cada operação de ponto de extremidade  <br>    - Forneça detalhes e parâmetros _da solicitação_ - Forneça detalhes _da resposta_  <br>    bem-sucedida e malsucedida<br>- Para _objetos de dados_ que estão sendo transferidos  <br>    - Liste e descreva todas _as propriedades_ em cada esquema  <br>    - Para cada propriedade, liste e descreva _os valores permitidos_|
|API de código nativo|Para uma API de código nativo, a referência deve documentar os seguintes elementos públicos:<br><br>- Listar e descrever todas _as classes_ (ou tipos de objetos ou interfaces)  <br>    - Descrever a instanciação (criação de objetos)  <br>    - Listar e descrever todas _as propriedades_ (dados) e métodos (ações)<br>- _Listar e descrever todas as funções_ de nível superior (ou seja, funções que não são métodos de objeto)<br>- Para métodos e funções, mostre todas _as entradas_ (parâmetros) e _saídas_ (valores de retorno)<br>- Para propriedades, liste e descreva _os valores permitidos_<br>- Listar e descrever todas _as estruturas de dados_ (tipos e enumerações)|
|CLI|Para uma CLI, a referência deve documentar os seguintes elementos públicos:<br><br>- Listar e descrever todos _os comandos_ (ações)<br>- Para cada comando, liste e descreva _argumentos_ e _opções_  <br>    - Argumentos são variáveis; liste e descreva _valores permitidos - Para opções, liste e descreva todos_ _os parâmetros_  <br>    obrigatórios e opcionais com _valores permitidos_|

Qual é a sintaxe de um elemento de API?

a . Os motivos para fazer chamadas
b . A relação do elemento com outros elementos
c . As regras para fazer chamadas e passar dados
     C: Informações sintáticas são sobre estrutura e regras.

Verdadeiro ou falso? Informações sobre razões e relacionamentos agregam valor à descrição da sintaxe.

a . Verdadeiro (Correto: R: Para usar a API corretamente, o usuário precisa entender o significado de uma chamada, bem como sua estrutura.)
b . Falso

Uma boa descrição de parâmetro fornece informações sobre:

a . Valores possíveis
b . O que os valores significam
c . De onde vêm os valores
d . Como os valores serão usados
e . Tudo o que precede (E: Boas descrições incluem o máximo possível de informações de uso e contexto.)

## Anotando o código-fonte
Ferramentas de geração de documentação normalmente produzem documentação de API a partir de código-fonte ou especificações, extraindo informações estruturais de definições de funções e tipos de dados e procurando por comentários e tags especialmente formatados que identificam e descrevem elementos públicos.

Para tornar o código-fonte da sua API "autodocumentado" com essas ferramentas, você precisa adicionar comentários e tags ao código-fonte. Seu padrão de codificação deve incluir a tarefa de verificar e adicionar a estrutura de documentação como parte do processo de revisão de código.

Arquivos de origem que definem classes e funções, como **myClass.java** , fornecem informações estruturais para APIs de código nativo. Para linguagens como C/C++, arquivos de cabeçalho ( ***.h** ) definem as estruturas de dados e as assinaturas de função e classe, mas não contêm o código de implementação.

Ferramentas como [Doxygen](https://www.doxygen.nl/) , [JavaDoc](https://javadoc.io/) e [GitBook](https://www.gitbook.com/) exigem um comentário especialmente formatado em elementos públicos nos arquivos de origem ou de cabeçalho para gerar a documentação.

- Para linguagens interpretadas como JavaScript, a fonte de informações estruturais é o arquivo de implementação real ( ***.js** ). Ferramentas como [JSDoc](https://jsdoc.app/) buscam o mesmo tipo de comentário específico da documentação nas definições de elementos públicos.
- [Sphinx](https://www.sphinx-doc.org/en/master/) é uma ferramenta Python que pode gerar documentação a partir de comentários em qualquer tipo de arquivo de texto, incluindo código-fonte CLI.

Para APIs REST, ferramentas como [Swagger](https://swagger.io/) e [Redoc](https://redoc.co/) geram documentação a partir de arquivos de descrição de API YAML ou JSON que estão em conformidade com a especificação OpenAPI.

## Documentação de suporte para código-fonte aberto
Para um projeto de código aberto, é particularmente importante documentar exatamente como a documentação gerada é produzida. Os colaboradores precisam saber quais ferramentas estão sendo utilizadas e como essas ferramentas estão configuradas.

- Os colaboradores do código precisam saber se e como adicionar a infraestrutura de comentários às novas definições, e se e como adicionar novos arquivos à infraestrutura de geração de documentos.
- Os membros da comunidade que desejam editar ou adicionar informações à documentação precisam saber como e onde fazer alterações. Um colaborador pode facilmente cometer o erro de editar diretamente um arquivo de documentação gerado, apenas para descobrir que suas contribuições são substituídas na próxima vez que a tarefa de geração automática de documentos for executada.

Incentive ambos os tipos de contribuição e multiplique o valor de suas ferramentas de geração de documentos incluindo requisitos de documentação em suas políticas e instruções de contribuição.
## Maneiras de melhorar a documentação gerada

Normalmente, as ferramentas geram uma página HTML por elemento principal com toda a sintaxe representada. A saída é configurável — geralmente com um makefile ou arquivo de configuração — com opções que controlam a aparência e heurísticas que controlam quais informações são incluídas.

Todas essas ferramentas são otimizadas para representação sintática, não para descrição semântica. Uma listagem básica de elementos como nomes e tipos de parâmetros está incorporada ao formato, mas você pode e deve adicionar descrições úteis. As ferramentas geralmente incluem uma propriedade ou tag "description", onde você pode adicionar uma string descritiva que explique o significado e o uso pretendido de cada elemento.

Os campos de descrição **não** recebem valores padrão. Mesmo que o seu modelo de comentário inclua os espaços reservados para strings descritivas, o conteúdo semântico ainda precisa ser adicionado. Se você não o adicionar, obterá uma lista básica de detalhes de sintaxe, como nomes de propriedades, tipos e valores permitidos — mas os usuários precisam descobrir por si mesmos o significado desses valores e qual pode ser o uso pretendido.

Mesmo quando os engenheiros adicionam comentários descritivos na documentação do código-fonte, eles quase sempre podem ser aprimorados. Os desenvolvedores de API a) geralmente não são escritores profissionais, b) não analisam toda a API pública e c) geralmente se concentram na implementação, em vez da experiência do usuário.

- Se você precisa de um redator profissional para ajudá-lo a adicionar e editar descrições semânticas, essa pessoa precisa ter acesso ao código-fonte. Escolha um redator técnico que entenda de desenvolvimento de software e seja confiável para manter a integridade do código sem comentários. Ele não precisa ser um desenvolvedor especialista ou saber programar na linguagem que você está usando, basta aprender a sintaxe e ler o código.
- Para um projeto de código aberto, incentive contribuições de documentação de membros da comunidade com habilidades de edição e escrita, especificando os requisitos e padrões de documentação do projeto.
- Certifique-se de que seu projeto tenha uma maneira de rotular problemas de documentação e uma política para contribuições de documentos. Se a documentação gerada tiver a opção "Editar esta página", certifique-se de que ela aponte para a política de contribuição de documentos. A política deve descrever como e onde fazer alterações compatíveis com o processo de geração automática e também listar especialistas específicos no assunto que podem revisar e aprovar contribuições de documentação em suas áreas.

## Adicionando Visões Gerais e Introduções aos Documentos Gerados
Informações conceituais que explicam para que serve uma API e como ela deve ser usada não podem ser geradas diretamente a partir de anotações no código-fonte. Em vez disso, você deve adicionar explicitamente páginas somente texto, como visões gerais e introduções, ao conjunto de arquivos que sua ferramenta está analisando e formatando.

Normalmente, uma página de visão geral para cada classe ou recurso deve incluir uma descrição de como, por que e quando usar essa classe ou recurso, juntamente com um índice de quais métodos ou operações são suportados. O índice pode ser vinculado diretamente à página de sintaxe gerada para cada elemento, servindo como um auxílio de navegação para os usuários.

Você também pode criar documentos de API adicionais inteiros, como guias conceituais e tutoriais, diretamente em marcação e HTML (ou qualquer formato que sua ferramenta use) e configurar a ferramenta para adicioná-los às páginas de sintaxe geradas.

## Explorando ferramentas de documentação de API
Existem muitas ferramentas, frameworks e plataformas de documentação de API para escolher. A escolha da ferramenta geralmente depende da linguagem de programação, dos requisitos do projeto e das preferências pessoais. Você deve explorar e avaliar diferentes ferramentas com base nas suas necessidades específicas antes de decidir sobre o conjunto de ferramentas mais adequado para o seu projeto.

A tabela a seguir lista algumas ferramentas comuns que podem gerar documentação de API a partir do código-fonte ou de especificações, ou integrar-se a ferramentas de geração para produzir sites de documentação abrangentes que incluem o conteúdo gerado. É claro que muitas outras ferramentas semelhantes estão se tornando disponíveis a cada dia neste campo em rápida evolução e crescimento.

### Ferramentas de documentação que oferecem suporte à geração a partir do código**

| Ferramenta                                                                            | Descrição                                                                                                                                                                                                                                                                                                                                                   | API Type              |
| ------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| [DapperDox](http://dapperdox.io/)                                                     | Gerador e servidor de documentação de API de código aberto para especificações do OpenAPI Swagger. Combina especificações com documentação, guias e diagramas, todos os quais podem ser criados em Markdown com suporte do GitHub.                                                                                                                          | REST                  |
| [Doxygen](https://www.doxygen.nl/index.html)                                          | Uma ferramenta de documentação amplamente utilizada para C++, C, Objective-C e diversas outras linguagens de programação. Ela gera documentação a partir de comentários no código-fonte e suporta diversos formatos de saída, incluindo HTML, PDF e LaTeX.                                                                                                  | Native code           |
| [Javadoc](https://www.oracle.com/technical-resources/articles/java/javadoc-tool.html) | Uma ferramenta de documentação projetada especificamente para gerar documentação de API para projetos Java. Ela extrai comentários do código-fonte e produz documentação baseada em HTML.                                                                                                                                                                   | Native code           |
| [JSDoc](https://jsdoc.app/)                                                           | Uma linguagem de marcação usada para anotar arquivos de código-fonte JavaScript. Semelhante ao Javadoc, mas especializada em lidar com o comportamento dinâmico do JavaScript.                                                                                                                                                                              | Native code           |
| [RapiDoc](https://github.com/rapi-doc/RapiDoc)                                        | Uma ferramenta interativa que permite criar documentos visualmente atraentes usando a especificação OpenAPI, com um console para fazer chamadas de API e testar APIs.                                                                                                                                                                                       | REST                  |
| [ReadMe](https://readme.com/)                                                         | Uma plataforma que ajuda você a criar, gerenciar e manter um hub de desenvolvedores online com diferentes tipos de documentos. Pode gerar automaticamente documentação de referência de API interativa a partir de especificações OpenAPI, RAML ou GraphQL. Integra-se com diversas ferramentas e serviços de desenvolvimento, como GitHub, GitLab e Slack. | REST  <br>Native Code |
| [Read the Docs](https://about.readthedocs.com/)                                       | Uma plataforma de hospedagem de documentação que se integra a geradores de documentação populares, como Sphinx e MkDocs. Cria e implementa automaticamente a documentação a partir do seu repositório de código-fonte, usando o padrão " [docs as code ".](https://docs-as-co.de/)                                                                          | REST  <br>Native Code |
| [Redoc](https://redocly.com/docs/redoc/)                                              | Produz documentação pronta para a web a partir de uma descrição OpenAPI ou Swagger.                                                                                                                                                                                                                                                                         | REST                  |
| [Redocly CLI](https://redocly.com/docs/cli/)                                          | Ferramenta de linha de comando de código aberto para trabalhar com descrições OpenAPI, portais de desenvolvedores e outras operações de ciclo de vida de API, incluindo linting, aprimoramento e agrupamento de API.                                                                                                                                        | REST                  |
| [Sphinx](https://www.sphinx-doc.org/en/master/)                                       | Um gerador de documentação comumente usado no ecossistema Python. Suporta diversas linguagens de marcação, incluindo reStructuredText (RST) e Markdown. O Sphinx pode gerar vários formatos de saída, como HTML, PDF e ePub.                                                                                                                                | REST  <br>Native Code |
| [Stoplight](https://stoplight.io/)                                                    | Plataforma que inclui ferramentas para gerar documentação de API a partir de uma especificação OpenAPI. Inclui modelos para páginas de Visão Geral da API, Guias de Início Rápido e Tutoriais Práticos.                                                                                                                                                     | REST                  |
| [Swagger Codegen](https://swagger.io/tools/swagger-codegen/)                          | Gera uma interface HTML interativa que permite aos usuários explorar os pontos de extremidade da API, parâmetros, exemplos de solicitação/resposta e muito mais.                                                                                                                                                                                            | REST                  |

Generation tools generate documentation from:

a. Specially formatted annotations in source code
b. The structural information implicit in function definitions
c.The data types defined in source code
d. All of the above
    D: Tools can extract structural information directly from the code. Annotations add semantic information.



True or False? Generated documentation automatically provides all of the information users need to use an API successfully.

a. True
b. False
 By default, tools generate only syntactic information. Semantic information must be added to the sources.


True or False? Adding and providing content for "description" tags provides all of the information users need to use an API successfully.
a. True
b. False
B: Para fornecer contexto suficiente, páginas de visão geral somente com texto devem ser adicionadas ao modelo de geração de documentação.


## Visão geral do capítulo
Solicitar que sua equipe de desenvolvimento documente seu próprio código tem um impacto real em seu esforço de desenvolvimento. Programadores não são, tipicamente ou principalmente, escritores em linguagem natural; a habilidade de escrever código é diferente da habilidade de escrever em linguagem natural. Mesmo quando os engenheiros têm boas habilidades de escrita e comunicação, eles geralmente não estão familiarizados com as questões de planejamento e organização e com os problemas da produção de documentação técnica. Além disso, as tarefas de escrita geralmente estão em desacordo com as responsabilidades de codificação e design de código, tanto no sentido da alocação de tarefas quanto da mentalidade necessária para executá-las.

Em suma, é mais eficiente e gera melhores resultados delegar o planejamento e a produção da sua documentação a profissionais de comunicação técnica. Seus recursos de engenharia podem contribuir para a qualidade da documentação, fornecendo informações técnicas aos redatores e revisando o conteúdo dos rascunhos.

# A transferência eficaz de conhecimento requer habilidades específicas

O objetivo da documentação técnica é transferir conhecimento de forma eficiente das pessoas que o possuem (como a equipe de desenvolvimento de um aplicativo de software de código aberto) para as pessoas que precisam dele (como desenvolvedores que desejam usar uma API).

A eficácia da documentação do produto é medida pelo sucesso do usuário. Um usuário bem-sucedido é aquele que conseguiu encontrar e compreender as informações necessárias para realizar suas tarefas. Você pode perceber que a documentação do seu produto precisa de melhorias quando sua equipe de suporte está sobrecarregada ajudando novos usuários a começar, suas equipes de engenharia estão dando muita assistência aos usuários atuais e sua equipe de marketing está tendo dificuldades para fazer com que os avaliadores entendam os benefícios e os pontos fortes do produto.

Criar documentação eficaz para um assunto técnico complexo requer dois conjuntos de habilidades específicas.

- _Engenharia do conhecimento
    _A arte de obter informações de um ou mais especialistas no assunto (SMEs) e analisá-las com o objetivo específico de entender e comunicar essas informações a outros.
- _Arquitetura da informação
    _A arte de organizar, arranjar e apresentar um corpo de conhecimento de modo que ele seja acessível a diferentes tipos de usuários e potenciais usuários.

Redatores técnicos experientes desenvolvem essas habilidades. O engenheiro do conhecimento compreende e reconhece diferentes tipos de conhecimento, como factual e procedural. O arquiteto da informação entende como as pessoas podem absorver cada tipo de conhecimento com mais facilidade. Por exemplo, quando um usuário precisa de uma tabela de consulta e quando precisa de um tutorial?

Embora alguns arquitetos e engenheiros de software tenham habilidades de escrita e comunicação razoáveis ​​ou até excelentes, esta não é sua principal área de especialização. Eles também estão totalmente ocupados projetando e construindo o software. Para outros, escrever é uma luta, e esperar que eles se dediquem muito a isso não significa aproveitar bem o seu tempo. Geralmente, é mais construtivo para uma equipe de desenvolvimento trabalhar com escritores e editores profissionais para produzir uma documentação de qualidade que atraia usuários e colaboradores, e permita que as pessoas aprendam e usem seu software com sucesso.
