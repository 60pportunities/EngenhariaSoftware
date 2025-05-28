Uma arquitetura é o conjunto de decisões significativas sobre a organização de um sistema de software, a seleção dos elementos estruturais e suas interfaces pelas quais o sistema é composto, juntamente com seu comportamento conforme especificado nas colaborações entre esses elementos, a composição desses elementos estruturais e comportamentais em subsistemas progressivamente maiores e o estilo de arquitetura que orienta essa organização — esses elementos e suas interfaces, suas colaborações e sua composição. (Booch, Rumbaugh e Jacobson 1999)

### **Diferença entre Arquitetura e Design**

| Conceito      | Arquitetura                                              | Design                                                  |
| ------------- | -------------------------------------------------------- | ------------------------------------------------------- |
| **Foco**      | Estrutura fundamental e de alto nível do sistema         | Detalhamento interno e implementação dos componentes    |
| **Propósito** | Definir a **visão macro**, guiar decisões críticas       | Especificar **como** os componentes serão construídos   |
| **Escopo**    | Abrange **componentes principais, integração e padrões** | Abrange **detalhes funcionais, fluxos e layouts**       |
| **Impacto**   | Alterações causam impacto amplo no sistema               | Mudanças tendem a ser locais e mais controláveis        |
| **Abstração** | Mais abstrato, independente de tecnologia específica     | Mais concreto, muitas vezes ligado a frameworks ou libs |
- **Arquitetura**:
    - Escolher entre microsserviços ou monólito.
    - Definir como serviços vão se comunicar (REST, gRPC, eventos).
    - Estabelecer políticas de segurança e governança.
- **Design**:
    - Como estruturar as classes de um módulo.
    - Que padrão de design usar (Factory, Strategy, etc).
    - Como validar um formulário no front-end.
## Técnicas
<p align="justify">É fundamental para manter a clareza sobre como um sistema foi projetado e para garantir que todos os envolvidos em um projeto, presentes e futuros, compreendam os motivos por trás das escolhas feitas.</p>
### Architectural Decision Record (ADR)
O registro **concentra-se em uma decisão arquitetônica significativa** que normalmente afeta a estrutura, o comportamento central ou as qualidades-chave do sistema - Michael Nygard, que [popularizou as ADRs em 2011](https://www.cognitect.com/blog/2011/11/15/documenting-architecture-decisions?ref=workingsoftware.dev) 

É um documento mais específico, focado em registrar decisões arquiteturais importantes feitas durante o desenvolvimento de um software. Ele explica as razões por trás de uma escolha arquitetural, o que pode ajudar na manutenção do sistema no futuro e no entendimento do processo de tomada de decisão.

O ADR é geralmente mais restrito ao contexto do projeto ou da equipe que está desenvolvendo o software, abordando decisões como escolha de frameworks, design de sistemas ou como resolver um problema específico no contexto arquitetural.

Os ADRs devem se concentrar principalmente nas escolhas arquitetônicas que afetam a estrutura do sistema, características não funcionais, dependências, interfaces ou técnicas de construção.

_[Um registro de decisão de arquitetura (ADR) é um documento que captura uma decisão arquitetônica essencial tomada juntamente com seu](https://github.com/joelparkerhenderson/architecture-decision-record) **[contexto](https://github.com/joelparkerhenderson/architecture-decision-record)** [e](https://github.com/joelparkerhenderson/architecture-decision-record) **[consequências](https://github.com/joelparkerhenderson/architecture-decision-record)** ._

- [ ] **Decisão de Arquitetura** (AD) é uma escolha de design de software que atende a um requisito significativo.
```
Cada ADR responde a algumas perguntas básicas sobre uma decisão:
- **O que foi decidido?**
- **Por que isso foi necessário?**
- **Quais alternativas foram consideradas (até 3)?**
- **Quais são as implicações?**

No contexto de <caso de uso/história de usuário>
enfrentando <preocupação x>
decidimos por <opção o>
alcançar <qualidade x>
aceitar <desvantagem x>
```
- [ ] **Registro de Decisão de Arquitetura (ADR)** é um documento conciso que registra uma única  decisão **importante**  sobre a arquitetura, o contexto e as consequências de um sistema de software.
- [ ] **Registro de Decisão de Arquitetura** (ADL - Architecture Decision Log) é a coleção de todos os ADRs criados e mantidos para um projeto (ou organização) específico.
- [ ] **Requisito Arquitetonicamente Significativo** (ASR - Architecturally-Significant Requirement) é um requisito que tem um efeito mensurável na arquitetura de um sistema de software.
- [ ] Tudo isso está dentro do tópico da **Gestão** do **Conhecimento de Arquitetura** (AKM - Architecture Knowledge Management).

| Campo         | Descrição                                             |
| ------------- | ----------------------------------------------------- |
| Título        |                                                       |
| Data          |                                                       |
| Contexto      |                                                       |
| Decisão       |                                                       |
| Alternativas  |                                                       |
| Consequencias |                                                       |
| Participantes |                                                       |
| Status        | [ ] Proposto [ ] Aceito [ ] Rejeitado [ ] Substituida |
|               |                                                       |
#### Exemplo com ferramenta
- [ ] `brew install adr-tools`
- [ ] adr init docs/architecture/architecture-decision-records/
- [ ] adr new Implement as Unix shell scripts

### RFC (Request for Comments)
<p align="justify">Documento técnico usado para propor, discutir e definir novos padrões, protocolos ou práticas no desenvolvimento de software, principalmente em comunidades de código aberto.</p>

Ele é um convite para que outras pessoas comentem, revisem e até modifiquem a proposta.

Pode abranger uma vasta gama de tópicos, desde detalhes técnicos de implementação até mudanças mais amplas em como as ferramentas ou frameworks devem evoluir. Um RFC pode ser uma proposta de mudança em qualquer área de desenvolvimento, não necessariamente ligada à arquitetura de um sistema.

| Campo          | Descrição |
| -------------- | --------- |
| Tema           |           |
| Número         |           |
| Data de Início |           |
| Responsável    |           |
| Contribuidor   |           |
| Tema1..N       |           |
# Algumas Ferramentas

- [ ] **adr-cli / adr** (existe para [Go](https://github.com/marouni/adr) , [Node.js](https://github.com/phodal/adr) , [Python](https://pypi.org/project/adr-tools-python/) , [C#](https://github.com/GingerTommy/adr-cli) , [Java](https://github.com/adoble/adr-j) , [PHP](https://github.com/bellangelo/phpadr) , [Rust](https://github.com/joshrotenberg/adrs) , [Powershell](https://github.com/rdagumampan/adr-ps) ): Há várias reescritas e ports do original `adr-tools`em diferentes linguagens de programação, como `adr-cli`(C#), `adr`(Go, Node.js) `adr-tools-python`, `ADR-py`(Python), `phpadr`(PHP), `adrs`(Rust) e módulos PowerShell.
- [ ]  **[adr-viewer](https://github.com/mrwilson/adr-viewer)** : Um aplicativo Python que gera um site navegável a partir de um conjunto de ADRs, facilitando a visualização por meio de uma interface web.
- [ ]  **[Ferramentas MADR](https://github.com/nioe/madr-tools)** . Um modelo estendido que mostra claramente os motivadores de decisão, as opções consideradas e os prós/contras de forma estruturada. O projeto MADR fornece modelos completos e minimalistas, além de suporte a ferramentas.
- [ ]  **[Log4brains](https://github.com/thomvaill/log4brains)** é uma ferramenta para registrar Registros de Decisões de Arquitetura (ADR) do seu IDE e publicá-los automaticamente como um site estático.
- [ ] [doctoolchain](https://doctoolchain.org/docToolchain/v2.0.x/):  É uma coleção de scripts que facilita a criação e a manutenção de documentação técnica robusta. Construído com as melhores tecnologias de código aberto, oferecemos a melhor cadeia de ferramentas de documentação para que você não precise se preocupar.
- [ ] [Structurizr](https://docs.structurizr.com/) se baseia em “diagramas como código”, permitindo que você crie **vários diagramas de arquitetura de software** usando o [modelo C4](https://c4model.com/) , em uma **variedade de ferramentas de renderização** , a partir de um **único modelo** .

## [](https://docs.structurizr.com/#quickstart)
# Alguns Exemplos

## Contexto e Declaração do Problema

{Descreva o contexto e a declaração do problema, por exemplo, de forma livre, usando duas a três frases ou na forma de uma história ilustrativa. Você pode articular o problema na forma de uma pergunta e adicionar links para painéis de colaboração ou sistemas de gerenciamento de problemas.}

<!-- Este é um elemento opcional. Sinta-se à vontade para removê-lo. -->
## Motivadores da Decisão

* {motivador da decisão 1, por exemplo, uma força, enfrentando preocupação, …}
* {motivador da decisão 2, por exemplo, uma força, enfrentando preocupação, …}
* … <!-- o número de motivadores pode variar -->

## Opções Consideradas

* {título da opção 1}
* {título da opção 2}
* {título da opção 3}
* … <!-- o número de opções pode variar -->

## Resultado da Decisão

Opção escolhida: "{título da opção 1}", porque {justificação. Ex.: única opção que atende ao critério k.o. driver de decisão | que resolve força {força} | … | sai melhor (veja abaixo)}.

<!-- Este é um elemento opcional. Sinta-se à vontade para remover. -->
### Consequências

* Bom, porque {consequência positiva, por exemplo, melhoria de uma ou mais qualidades desejadas, …}
* Ruim, porque {consequência negativa, por exemplo, comprometimento de uma ou mais qualidades desejadas, …}
* … <!-- o número de consequências pode variar -->

<!-- Este é um elemento opcional. Sinta-se à vontade para remover. -->
### Confirmação

{Descreva como a implementação/conformidade com a ADR pode/será confirmada. O design que foi decidido e sua implementação estão alinhados com a decisão tomada? Por exemplo, uma revisão de design/código ou um teste com uma biblioteca como o ArchUnit podem ajudar a validar isso. Não que, embora classifiquemos este elemento como opcional, ele esteja incluído em muitas ADRs.

<!-- Este é um elemento opcional. Sinta-se à vontade para removê-lo. -->
## Prós e Contras das Opções

### {título da opção 1}

<!-- Este é um elemento opcional. Sinta-se à vontade para removê-lo. -->
{exemplo | descrição | ponteiro para mais informações | …}

* Bom, porque {argumento a}
* Bom, porque {argumento b}
<!-- use "neutro" se o argumento fornecido não tiver peso nem bom nem ruim -->
* Neutro, porque {argumento c}
* Ruim, porque {argumento d}
* … <!-- o número de prós e contras pode variar -->

### {título da outra opção}

{exemplo | descrição | ponteiro para mais informações | …}

* Bom, porque {argumento a}
* Bom, porque {argumento b}
* Neutro, porque {argumento c}
* Ruim, porque {argumento d}
* …

<!-- Este é um elemento opcional. Sinta-se à vontade para removê-lo. -->
## Mais Informações

{Você pode fornecer evidências/confiança adicionais para o resultado da decisão aqui e/ou documentar o acordo da equipe sobre a decisão e/ou definir quando/como essa decisão deve ser implementada e se/quando deve ser revisada. Links para outras decisões e recursos também podem aparecer aqui.}

# Documento Original

## Documentando decisões de arquitetura
[Michael Nygard](https://www.cognitect.com/authors/MichaelNygard.html) - 15 de novembro de 2011
# Contexto

- [ ] A arquitetura para projetos ágeis precisa ser descrita e definida de forma diferente.
- [ ] Nem todas as decisões serão tomadas de uma só vez, nem todas serão implementadas no início do projeto.
- [ ] Métodos ágeis não se opõem à documentação, apenas à documentação sem valor.
- [ ] Documentos que auxiliam a própria equipe podem ter valor, mas somente se forem mantidos atualizados.
- [ ] Documentos grandes nunca são atualizados. Documentos pequenos e modulares têm pelo menos uma chance de serem atualizados.
- [ ] Ninguém lê documentos grandes.
- [ ] Partes pequenas são mais fáceis de serem consumidas por todos os stakeholders.

- [ ] Uma das coisas mais difíceis de rastrear durante a vida de um projeto é a motivação por trás de certas decisões.
- [ ] Um novato que assume um projeto pode estar perplexo, perplexo, encantado ou enfurecido com alguma decisão tomada no passado. Sem entender a lógica ou as consequências, essa pessoa tem apenas duas opções:

1. **Aceite cegamente a decisão.**: Essa resposta pode ser aceitável se a decisão ainda for válida. No entanto, pode não ser boa se o contexto mudou e a decisão realmente precisa ser revisada. Se o projeto acumular muitas decisões aceitas sem entendimento, a equipe de desenvolvimento fica com medo de mudar qualquer coisa e o projeto desmorona sob seu próprio peso.

2. **Mude-o cegamente.**: Novamente, isso pode ser aceitável se a decisão precisar ser revertida. Por outro lado, mudar a decisão sem entender sua motivação ou consequências pode significar prejudicar o valor geral do projeto sem que se perceba. (Por exemplo, a decisão apoiou um requisito não funcional que ainda não foi testado.)
# Decisão
Manteremos uma coleção de registros para decisões "arquitetonicamente significativas": aquelas que afetam a estrutura, características não funcionais, dependências, interfaces ou técnicas de construção.

- [ ] Um registro de decisão de arquitetura é um pequeno arquivo de texto em um formato semelhante ao padrão Alexandrino.
- [ ] Embora as decisões em si não sejam necessariamente padrões, elas compartilham o equilíbrio de forças característico.)
- [ ] Cada registro descreve um conjunto de forças e uma única decisão em resposta a essas forças.
- [ ] Observe que a decisão é a peça central aqui, portanto, forças específicas podem aparecer em vários ADRs.

- [ ] Manteremos os ADRs no repositório do projeto em doc/arch/adr-NNN.md
- [ ] Devemos usar uma linguagem de formatação de texto leve, como Markdown ou Textile.
- [ ] Os ADRs serão numerados sequencialmente e monotonicamente. Os números não serão reutilizados.
- [ ] Se uma decisão for revertida, manteremos a antiga, mas a marcaremos como substituída. (Ainda é relevante saber que _era_ a decisão, mas _não é mais_ a decisão.)
- [ ] Usaremos um formato com poucas partes, para que cada documento seja de fácil assimilação. O formato tem poucas partes.

Exemplo:

**Título:** Estes documentos têm nomes que são frases nominais curtas. Por exemplo, "ADR 1: Implantação em Ruby on Rails 3.0.10" ou "ADR 9: LDAP para Integração Multilocatário".

**Contexto** Esta seção descreve as forças em jogo, incluindo as tecnológicas, políticas, sociais e as de projeto local. Essas forças provavelmente estão em tensão e devem ser destacadas como tal. A linguagem desta seção é neutra em termos de valores. Ela simplesmente descreve fatos.

**Decisão:** Esta seção descreve nossa resposta a essas forças. Ela é expressa em frases completas, na voz ativa. "Nós iremos..."

**Status:** 
- [ ] Uma decisão pode ser "proposta" se as partes interessadas do projeto ainda não concordaram com ela, ou
- [ ] Uma decisão pode ser "aceita" após o acordo.
- [ ] Se uma ADR posterior alterar ou reverter uma decisão, ela poderá ser marcada como "obsoleta" ou "substituída", com uma referência à sua substituição.

**Consequências:** Esta seção descreve o contexto resultante, após a aplicação da decisão.

- [ ] Todas as consequências devem ser listadas aqui, não apenas as "positivas".
- [ ] Uma decisão específica pode ter consequências positivas, negativas e neutras, mas todas elas afetam a equipe e o projeto no futuro.

O documento inteiro deve ter uma ou duas páginas. Escreveremos cada ADR como se fosse uma conversa com um futuro desenvolvedor. Isso requer um bom estilo de escrita, com frases completas organizadas em parágrafos. Marcadores são aceitáveis ​​apenas para estilo visual, não como desculpa para escrever fragmentos de frases. (Marcadores matam pessoas, até mesmo marcadores de PowerPoint.)

# Status

Aceito.

# Consequências

- [ ] Uma ADR descreve uma decisão significativa para um projeto específico. Deve ser algo que tenha impacto no andamento do restante do projeto.
- [ ] As consequências de uma ADR têm grande probabilidade de se tornarem o contexto para ADRs subsequentes.
- [ ] Isso também se assemelha à ideia de Alexander de uma linguagem de padrões: as respostas em larga escala criam espaços para as de menor escala se encaixarem.
- [ ] Desenvolvedores e partes interessadas do projeto podem ver os ADRs, mesmo que a composição da equipe mude ao longo do tempo.

A motivação por trás de decisões anteriores é visível para todos, presentes e futuros. Ninguém fica coçando a cabeça tentando entender: "O que eles estavam pensando?", e o momento de mudar decisões antigas ficará claro a partir das mudanças no contexto do projeto.

# Relato de Experiência
Você deve ter notado que este post está formatado como um ADR. Temos usado esse formato em alguns dos nossos projetos desde o início de agosto. Não é um tempo muito longo em termos globais, mas o feedback inicial de clientes e desenvolvedores tem sido bastante positivo. Nesse período, tivemos de seis a dez desenvolvedores revezando entre projetos que usam ADRs. Todos eles declararam que apreciam o nível de contexto que receberam ao lê-los.

As ADRs têm sido especialmente úteis para capturar intenções de longo prazo. Temos vários clientes que estão estabilizando seus sistemas atuais, mas vislumbram uma reestruturação maior em um futuro não muito distante. Ao anotar essas intenções, não dificultamos inadvertidamente essas mudanças futuras.

Uma possível objeção é que mantê-los em controle de versão com o código os torna menos acessíveis para gerentes de projeto, partes interessadas do cliente e outros que não estão em controle de versão como a equipe de desenvolvimento. Na prática, quase todos os nossos projetos residem em repositórios privados do GitHub, então podemos trocar links para a versão mais recente no repositório principal. Como o GitHub processa o markdown automaticamente, ele parece tão amigável quanto qualquer página wiki.

Até agora, os ADRs estão se mostrando uma ferramenta útil, então continuaremos a usá-los.

# Mais leitura

Agradeço a Philipe Kruchten por discutir a [importância das decisões de arquitetura](http://www.computer.org/portal/web/csdl/doi/10.1109/MS.2009.52) . Disseram-me que há mais sobre elas em [Documentando Arquiteturas de Software,](http://www.sei.cmu.edu/library/abstracts/books/0321552687.cfm) que está no topo da minha lista de leitura.


![[Pasted image 20250522194215.png]]


![[Pasted image 20250522194242.png]]


![[Pasted image 20250522194254.png]]


![[Pasted image 20250522194305.png]]
