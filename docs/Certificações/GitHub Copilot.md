O GitHub Copilot representa uma mudança monumental na forma como o código é escrito, oferecendo a você um parceiro excepcional em sua jornada de codificação.

O GitHub Copilot é um assistente de programação baseado em IA desenvolvido pelo GitHub em parceria com a OpenAI.

O GitHub Copilot não é apenas uma ferramenta; ele está transformando o conceito de programação em pares.
A engenharia de prompts é a prática de estruturar comandos ou instruções para obter os melhores resultados possíveis de modelos de IA generativa.
A qualidade das sugestões geradas pelo GitHub Copilot depende diretamente da clareza dos prompts fornecidos.
Prompts bem elaborados ajudam a IA a entender melhor o contexto do problema, resultando em saídas mais úteis e precisas.

| Ideia da IA                | Entenda                                                               |
| -------------------------- | --------------------------------------------------------------------- |
| Imparcialidade             | Os sistemas de IA devem tratar todas as pessoas de maneira imparcial. |
| Confiabilidade e segurança | O desempenho dos sistemas de IA deve ser confiável e seguro.          |
| Privacidade e segurança    | Os sistemas de IA devem ser seguros e respeitar a privacidade.        |
| Inclusão                   | Os sistemas de IA devem capacitar a todos e engajar as pessoas.       |
| Transparência              | Os sistemas de IA devem ser compreensíveis.                           |
| Responsabilidade           | As pessoas devem ser responsáveis pelos sistemas de IA.               |

| Modelo/Produto                       | Fornecedor         | Finalidade Principal                                                              | Público-Alvo                         | Principais Recursos                                                                | Integração                                 | Casos de Uso Comuns                                                          |
| ------------------------------------ | ------------------ | --------------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------------------------- | ------------------------------------------ | ---------------------------------------------------------------------------- |
| **Serviços de IA do Azure**          | Microsoft          | Oferecer APIs e serviços de IA prontos para uso (visão, linguagem, voz, decisão)  | Desenvolvedores, empresas            | APIs pré-treinadas, personalização, escalabilidade                                 | Azure, REST APIs, SDKs                     | Chatbots, análise de imagens, tradução automática, reconhecimento de fala    |
| **Portal da Fábrica de IA do Azure** | Microsoft          | Interface para criar, implantar e gerenciar soluções de IA                        | Engenheiros de IA, cientistas        | Modelos pré-construídos, pipelines de dados, monitoramento                         | Azure Machine Learning, Power BI           | Desenvolvimento de modelos personalizados, automação de fluxos de trabalho   |
| **AI Builder**                       | Microsoft          | Criar modelos de IA sem código para automação de processos                        | Usuários de negócios, Power Platform | Modelos pré-treinados (formulários, previsões), integração com Power Apps/Automate | Power Apps, Power Automate, Dynamics 365   | Extração de dados de documentos, automação de tarefas repetitivas            |
| **Copilot Studio**                   | Microsoft          | Criar e personalizar copilots (assistentes de IA) para interações conversacionais | Desenvolvedores, equipes de TI       | Interface low-code, conectores a dados externos, GPT-4 integrado                   | Microsoft 365, Teams, Power Platform       | Chatbots empresariais, suporte ao cliente automatizado                       |
| **SDK do Semantic Kernel**           | Microsoft          | Integrar modelos de IA (como LLMs) em aplicativos com orquestração de tarefas     | Desenvolvedores avançados            | Composição de habilidades, plugins, planejamento de tarefas                        | Azure OpenAI, ChatGPT, APIs personalizadas | Aplicativos com raciocínio contextual, automação complexa                    |
| **Visual Studio IntelliCode**        | Microsoft          | Auxiliar na escrita de código com sugestões baseadas em IA                        | Desenvolvedores                      | Autocompletar contextual, recomendações de padrões                                 | Visual Studio, VS Code                     | Aceleração de desenvolvimento, redução de erros                              |
| **ChatGPT**                          | OpenAI             | Gerar texto, responder perguntas e realizar tarefas de linguagem natural          | Público geral, desenvolvedores       | Conversação natural, suporte a múltiplos idiomas, customização via prompts         | API OpenAI, aplicativos personalizados     | Suporte virtual, criação de conteúdo, tutoriais interativos                  |
| **GitHub Copilot**                   | Microsoft (GitHub) | Sugerir código em tempo real com base em contexto                                 | Desenvolvedores                      | Autocompletar código, suporte a múltiplas linguagens, integração com editores      | VS Code, Visual Studio, JetBrains          | Aceleração de codificação, redução de bugs, aprendizado de novas tecnologias |




- [x] https://learn.microsoft.com/pt-br/training/modules/get-started-github-copilot/?wt.mc_id=1reg_24497_webpage_reactor

- [x] https://www.builder.io/blog/cursor-vs-github-copilot

- [x] https://learn.microsoft.com/pt-br/training/modules/github-copilot-across-environments/?wt.mc_id=1reg_24497_webpage_reactor

- [x] https://developer.microsoft.com/pt-br/reactor/series/S-1447/?wt.mc_id=seriespg_S-1447_webpage_reactor

- [x] https://learn.microsoft.com/pt-br/training/paths/copilot/?wt.mc_id=github_inproduct_copilotfoundations_mslearn_ghcertregistration

Hi everyone.
My name is Henry.
Thank you so much for taking this course.
I promise we will get right away into learning about GitHub Copilot and all of its great features.
But before we do that, we need to understand what GitHub Copilot is.
Simply put, GitHub Copilot is an AI coding assistant that is proven.
That's right.
Proven to improve developer productivity and happiness.
Productivity is simple.

You can get more stuff done in the same amount of time.

Happiness is something where I really like because it allows you to focus on more high level problem

solving tasks rather than mundane, uh, manual work that many developers have to do.

Now, in terms of the idea behind GitHub Copilot and the mechanism, we'll learn a little bit about

that more, but it's basically the idea or the amalgamation of three separate things.

Okay.

First is generative AI.

We know how we can use it for many different use cases like writing code, reviewing code, understanding

code.

And it goes beyond code as well as anything related to any sort of text generation or synthesis.

You then have your code base.

This is your canvas.

This is where you create code.

This is where you push code, maybe into a git repository or something like that.

This is your product.

And then you have your IDE.

This is how you actually create your product.

This is your paintbrush.

Okay, now GitHub Copilot is really the amalgamation of these three things okay.

It allows you to run generative AI tasks given your code base as context and available to you right

in your IDE.

Okay, right where you work.

So it's generative AI with your code as context and it's available to you right where you work.

That's really the sum of what GitHub Copilot strives to accomplish.

Okay.

Now it's been proven to really, really sorry, really, really improve developer productivity and happiness.

There's been many studies on it.

Um, you know, it's very common to say and it's almost cringey at this point that AI will replace you.

Someone using AI will.

But after looking at all of these studies, it has never been truer.

Okay, so these are just some studies that I found.

You know, 88% of developers said that they are more productive.

And I'll be honest, when I do GitHub copilot trainings, only about 10% of developers actually use

GitHub Copilot efficiently.

So when the survey was taken, it's really targeting those people that really use GitHub Copilot efficiently,

which is why I wanted to create this course to make sure everyone hits that 88% productivity level.

Everyone feels that they are faster completion, everyone feels that they are less frustrated when coding,

so on and so forth.

In fact, there was a great study that was done that basically gave two sets of developers the same

task.

One set of group were very proficient with GitHub Copilot and the other group was not.

And you can see in terms of the finished rate, the people who were familiar with GitHub copilot definitely

finished more.

But also take a look at how much shorter time they took.

Okay.

It took them about 55% less time to complete the same task.

And that is again a control study if you think about it.

Right.

Because it's the same task to two different sets of developers.

Okay.

GitHub Copilot is a productivity machine, but only if you know how to use it, right?

All right.

We'll move on to the next video where we'll learn more about the features of GitHub copilot.

We'll go through the course roadmap.

We'll learn about how to succeed in this course.

And then we'll get into the future sections where we'll actually learn and get our hands dirty and learn

about all the great features of GitHub copilot.

All right.

Awesome.

Rolagem automática

[](https://www.udemy.com/terms/terms-of-use/#tou_gen-ai-terms)

[](https://survey.alchemer.com/s3/8155525/AIA-Feedback-Survey-product-marketplace)

## Conteúdo do curso

## Visão geral

## Perguntas e respostasPerguntas e respostas

## Observações

## Anúncios

## Avaliações

## Ferramentas de aprendizado

-
