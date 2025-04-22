A revisão de código é uma etapa essencial no ciclo de vida de desenvolvimento de software.

A **revisão de código** é uma etapa essencial no ciclo de vida de desenvolvimento de software e serve para garantir esses objetivos, promovendo transparência, qualidade e alinhamento técnico entre os times.

Existem diferentes benefícios de uma revisão de código:

- [ ] Reforçar boas práticas de arquitetura;
- [ ] Promover o aprendizado e a colaboração entre times;
- [ ] Promover a coesão da equipe;
- [ ] Garantir aderência aos padrões de codificação da organização;
- [ ] Verificar cobertura de testes;
- [ ] Avaliar clareza, legibilidade e documentação;

O que você deve procurar em uma revisão de código? 
- [ ] Design: isso se integra bem com o resto do sistema e as interações de diferentes componentes fazem sentido
- [ ] Funcionalidade: isso muda o que o desenvolvedor pretendia
- [ ] Complexidade: este código é mais complexo do que deveria ser;
- [ ] Nomeação: nomear é significativo e claro?
- [ ] Testes: são diferentes tipos de testes usados adequadamente, cobertura de código
- [ ] Estilo: segue as diretrizes de estilo
- [ ] Mensagens: Padronizadas 

Aqui estão algumas boas práticas ao fazer uma revisão de código:

- [ ] Tente revisar seu próprio código primeiro. Antes de enviar um código para seus colegas, tente lê-lo e entendê-lo. Procure partes que possam ser confusas.
- [ ]  Escreva uma breve descrição do que mudou. Isso deve explicar quais mudanças foram em alto nível e por que essas mudanças foram feitas.
- [ ] Automatize o que pode ser automatizado. Deixe para o sistema tudo o que pode ser automatizado, como verificação de compilações bem-sucedidas (CI), mudanças de estilo (linters), testes automatizados e alguns code smell e bugs de código (SonarQube);
- [ ] Tente entender o que mudou - cada linha. Se necessário, leia-o várias vezes, classe por classe.
- [ ] Comente com gentileza. Nunca mencione a pessoa (você), sempre se concentre nas mudanças como perguntas ou sugestões e deixe pelo menos um comentário positivo. Explique o "porquê" em seus comentários e sugira como melhorá-lo.
- [ ] Aprove o PR quando for bom o suficiente. Não se esforce pela perfeição, mas mantenha altos padrões. Não seja um detalhista.
- [ ] Torne as avaliações gerenciáveis em tamanho. Devemos limitar o número de linhas de código para revisão em uma revisão. Nossos cérebros não podem processar tanta informação de uma só vez. 
- [ ] O número ideal de LOC é de 200 a 400 linhas do núcleo de uma só vez, o que geralmente é de 60 a 90 minutos.

#### Exemplo

##### **Criação de Merge Request/Pull Request (MR)**

   - [ ] Desenvolvedor abre um MR/PR em um repositório que pode ser utilizado por múltiplos times.
   - [ ] Inclui descrição clara do propósito, escopo, e contexto técnico das mudanças.
##### **Escolha dos Revisores**

   - [ ] Revisores são preferencialmente:
   - [ ] Membros do time mantenedor do repositório
   - [ ] Pessoas que já contribuíram com partes impactadas
   - [ ] Especialistas em domínios técnicos relevantes

##### **Checklist de Revisão**
    
   - [ ] O código está limpo e legível?
   - [ ] Há testes automatizados cobrindo os novos casos?
   - [ ] O impacto em outras partes do sistema foi considerado?
   - [ ] A mudança é modular e reutilizável?
   - [ ] Há documentação suficiente (código, comentários, ou wiki)?
   - [ ] Segue os padrões do repositório (lint, formatação, convenções)?

##### **Discussões e Feedback**
    
   - [ ] Feedback deve ser construtivo e orientado a aprendizado.
   - [ ] O autor pode responder, discutir ou ajustar conforme necessário.
   - [ ] O objetivo é chegar a um consenso técnico.
##### **Aprovação e Merge**
   - [ ] Após aprovação, o código é mesclado pela pessoa mantenedora ou por automação configurada.

#### Cultura InnerSource Aplicada à Revisão

   - [ ] **Transparência**: Todos os MRs e revisões são públicos para a organização.
   - [ ] **Colaboração Intertimes**: Outros times podem sugerir melhorias, relatar impactos ou contribuir diretamente.
   - [ ] **Mentoria Natural**: Revisões viram oportunidades de mentoria técnica, compartilhamento de padrões e alinhamento entre diferentes áreas.
   - [ ] **Documentação viva**: Discussões nas revisões geram aprendizado reutilizável.
   - [ ] Use linguagem respeitosa e clara nos comentários.
   - [ ] Prefira sugestões e perguntas ao invés de ordens (“Você considerou...?” em vez de “Faça assim.”).
   - [ ] Agradeça contribuições — mesmo aquelas que precisem de ajustes.
   - [ ] Evite **[Lei da Trivialidade](Leis/Paradoxos.md)**: mantenha foco no que é essencial para a qualidade e sustentabilidade do código.