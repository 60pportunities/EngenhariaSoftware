O teste de software é uma prática essencial de desenvolvimento de software moderno.

| Valor                 | Entenda                                                                                                                                                                           |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Economicidade         | Testar seu software acabará economizando dinheiro no longo prazo, pois testar o software permitirá que você descubra bugs logo no início, quando custaria menos para corrigi-los. |
| Segurança             | Garante que o software que você está lançando estara livre de quaisquer problemas conhecidos e/ou mapeados.                                                                       |
| Qualidade             |                                                                                                                                                                                   |
| Satisfação do cliente | Garantir que eles forneçam a melhor experiência possível ao usuário, garantindo que as versões sejam estáveis ​​e sem problemas, alcançando assim a satisfação do cliente.        |
## Teste Unitário
Valida e verifica unidades ou componentes de software individuais para garantir que cada unidade funcione conforme planejado.
Uma unidade pode ser uma função, procedimento, método, objeto ou módulo. O teste de unidade ocorre durante a fase de codificação do ciclo de vida de desenvolvimento de software e pode ajudar a identificar erros de codificação, problemas de qualidade de código e problemas de segurança.

* Escreva testes simples e legíveis
* Escreva testes determinísticos: Apresenta o mesmo comportamento desde que o código permaneça inalterado;
* Teste manual: normalmente envolve testar vários cenários;
* Testes unitários devem ser automatizados;
* Testes de unidade isolados;
* Evite a interdependência dos testes;
* Evite chamadas de API ativas;
* Combine testes unitários e de integração;
* Certifique-se de que os testes unitários sejam repetíveis e escaláveis;
* Teste problemas de segurança como parte de seus testes de unidade.
## Teste de validação
Esse tipo de teste garante que a API retorne os resultados esperados e no formato correto. O teste de validação envolve a verificação de que os parâmetros de entrada, formato de saída, código de resposta e tipo de dados estão corretos.

## Teste Funcional
Verifica se a API funciona corretamente e atende às especificações exigidas. Esse tipo de teste pode incluir o teste da lógica de negócios da API, validação de entrada, validação de saída e tratamento de erros.

## Teste de IU
Valida se a API funciona corretamente na interface do usuário do aplicativo. Esse tipo de teste garante que a IU reflita com precisão os resultados da API e que a API esteja manipulando as entradas da IU corretamente

## Teste de Stress
Envolve testar o desempenho e a estabilidade da API sob condições estressantes. Esse tipo de teste simula cenários de alto tráfego e uso intenso para garantir que a API possa lidar com um grande número de usuários e solicitações simultâneas.

## Tempo de execução e detecção de erros
Esse tipo de teste garante que a API possa lidar com erros e exceções de tempo de execução.

## Teste de penetração
O teste de penetração é um tipo de teste de segurança que envolve a simulação de ataques de hackers para detectar vulnerabilidades e pontos fracos na API.

## Hacking de API
Os invasores (e testadores) podem ter como alvo os endpoints da API para obter acesso aos dados, interromper serviços ou sequestrar todo o sistema. Os hackers éticos podem treinar atacando APIs intencionalmente vulneráveis, que podem ser baixadas da Internet.
## Teste de segurança
Visam identificar vulnerabilidades e falhas relacionadas à segurança na API e garantir que a API atenda aos padrões de segurança exigidos. Esse tipo de teste inclui testes de vulnerabilidades, como injeção de SQL, script entre sites (XSS), falsificação de solicitação entre sites (CSRF) e outros.
## Teste de Fuzz
Envolve alimentar entradas inesperadas e inválidas na API para testar sua capacidade de lidar com entradas inesperadas e se recuperar de erros. Esse tipo de teste pode revelar vulnerabilidades de segurança ou comportamentos inesperados na API.
## Teste de Integração de sistema
É garantir que todos os módulos de um aplicativo funcionem juntos sem problemas e possam se comunicar entre si. A interação com o banco de dados também é testada.
## Teste Alfa
Depois que o teste de aceitação do usuário for realizado nas equipes de desenvolvimento e produto, o teste poderá ser expandido para incluir outros tipos de usuários.
## Teste Beta
O software é lançado para um número limitado de usuários reais fora da organização para obter feedback, que é então encaminhado aos desenvolvedores para otimizar e melhorar o lançamento conforme necessário antes de liberá-lo para todos os usuários.
# Framework de Teste

| Ferramenta      | Entenda                                                                                                                                                                                                                                                             |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ChaiJS          | ChaiJS foi projetada explicitamente para testes orientados por comportamento em JavaScript.                                                                                                                                                                         |
| Jest            | Jest é um framework JavaScript desenvolvido inicialmente pela Meta e posteriormente lançado como um projeto de código aberto.                                                                                                                                       |
| JUnit           | JUnit é uma estrutura de código aberto que você pode usar para escrever e executar testes.                                                                                                                                                                          |
| NUnit           | NUnit é uma estrutura de código aberto que você pode usar para escrever e executar testes em .NET.                                                                                                                                                                  |
| Mocha           | Mocha.js é uma estrutura de teste JavaScript que pode ser executada no navegador e no Node.js.                                                                                                                                                                      |
| Cypress         | Cypress é uma ferramenta de código aberto para testar aplicativos web front-end.                                                                                                                                                                                    |
| Jasmine         | Jasmine é uma estrutura de teste que você pode executar em plataformas habilitadas para JavaScript sem interferir no IDE ou no aplicativo.                                                                                                                          |
| Storybook       | Storybook é uma ferramenta que permite construir e testar interfaces de usuário (UI).                                                                                                                                                                               |
| Testcafe        | Test Cafe é uma ferramenta de automação Node.js de código aberto para testar aplicativos da web.                                                                                                                                                                    |
| TestNG          | TestNG cobre uma ampla gama de categorias de testes, que incluem testes unitários, funcionais, ponta a ponta e de integração.                                                                                                                                       |
| PHPUnit         | O PHPUnit é baseado na ideia que o desenvolvedor deve encontrar erros no código-fonte o mais rápido possível, se possível, antes mesmo do usuário reportar.                                                                                                         |
| Pytest          | Pytest é uma excelente estrutura de testes de automação que pode ser usada para todos os tipos de testes de software.                                                                                                                                               |
| Puppeteer       | O Puppeteer , criado por uma equipe do Google, é um ótimo framework para execução de testes. Ele oferece uma API especial do Chrome que pode ser usada com aplicativos NodeJS.                                                                                      |
| MSTest          |                                                                                                                                                                                                                                                                     |
| Test::Unit      | Test::Unit é baseado nos princípios xUnit e está disponível com a biblioteca padrão do Ruby.                                                                                                                                                                        |
| utPLSQL         | utPLSQL é uma estrutura de teste de unidade para Oracle PL/SQL. A estrutura segue os padrões da indústria e os melhores padrões de estruturas modernas de testes de unidade, como JUnit e RSpec.                                                                    |
| RSpec           | RSpec é composto por múltiplas bibliotecas, que são projetadas para funcionarem juntas ou podem ser usadas independentemente com outras ferramentas de teste como Cucumber ou Minitest.                                                                             |
| Robot Framework | Robot Framework é uma estrutura de automação de teste de código aberto orientada por palavras-chave, projetada para simplificar o processo de automação de testes, especialmente para testes de aceitação e desenvolvimento orientado a testes de aceitação (ATDD). |
| Selenide        | Selenide é uma estrutura de teste Java amplamente utilizada que funciona junto com o Selenium WebDriver, expandindo os recursos do WebDriver e JUnit.                                                                                                               |

## Matriz de Rastreabilidade


Esta matriz mapeia cada requisito funcional para os casos de teste que o validam.



| ID do Requisito | Descrição do Requisito                                                           | Caso(s) de Teste                                                                                                                                                                                   |
| --------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| FR01            | O usuário deve conseguir efetuar login com credenciais válidas                   | [equivalence-partitioning-login.md](tests/test-cases/equivalence-partitioning-login.md)                                                                                                            |
| FR02            | O sistema deve exibir uma mensagem de erro para tentativas de login inválidas    | [equivalence-partitioning-login.md](tests/test-cases/equivalence-partitioning-login.md)                                                                                                            |
| FR03            | O usuário deve visualizar a lista de produtos disponíveis                        | (coberto como pré-condição em casos de teste)                                                                                                                                                      |
| FR04            | O usuário pode adicionar produtos ao carrinho                                    | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)                                                                                            |
| FR05            | O usuário pode remover produtos do carrinho                                      | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)                                                                                            |
| FR06            | O usuário pode visualizar os itens do carrinho                                   | [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md)                                                                                            |
| FR07            | O usuário pode iniciar o processo de finalização da compra                       | [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md), [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md) |
| FR08            | O usuário deve preencher o nome, sobrenome e CEP durante a finalização da compra | [boundary-value-analysis-postalcode.md](tests/test-cases/boundary-value-analysis-postalcode.md), [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md)         |
| FR09            | O sistema deve validar os campos obrigatórios durante a finalização da compra    | [boundary-value-analysis-postalcode.md](tests/test-cases/boundary-value-analysis-postalcode.md), [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md)         |
| FR10            | O usuário pode concluir uma compra com sucesso                                   | [decision-table-testing-checkout.md](tests/test-cases/decision-table-testing-checkout.md), [state-transition-testing-cart-checkout.md](tests/test-cases/state-transition-testing-cart-checkout.md) |
| FR11            | O usuário pode sair do aplicativo                                                | (opcional: adicione se você documentar um caso de teste de logout)                                                                                                                                 |



---



**Observação:**

- Os nomes dos arquivos dos casos de teste agora vinculam-se diretamente aos arquivos em `/tests/test-cases/`.
