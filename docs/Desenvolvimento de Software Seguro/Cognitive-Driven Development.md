Cognitive-Driven Development (CDD), ou em português desenvolvimento orientado a cognição, é uma estratégia para reduzir a sobrecarga cognitiva durante o desenvolvimento ao melhorar o design do código.

Cognitive-Driven Development (CDD) é analisar e buscar limitar a complexidade de um código. Para que a gente consiga, de fato, ter uma maneira interessante de limitar a carga intrínseca do código que escrevemos, precisamos seguir alguns passos.

A primeira tarefa do time é decidir qual vai ser a unidade de código que será analisada. Por exemplo, se falamos de uma linguagem orientada a objetos temos algumas possibilidades de definição de unidade de código, como, por:

- [ ] Método dentro de uma classe;
- [ ] Aula;
- [ ] Arquivo

Intrisc Complex Point (ou Ponto de Complexidade Intrínseca) no Cognitive-Driven Development.

Aqui não existe regra, o objetivo do Cognitive-Driven Development (CDD) não é achar uma composição de Ponto de Complexidade Intrínseca (ICP) que forme uma métrica perfeita. 

A ideia é que a equipe, considerando suas características, encontre os ICP que façam sentido para aquele contexto.

E qual o limite de ICP que podemos ter então por unidade de código? Atualmente a nossa sugestão é que você tenha um número que seja o dobro ou maior ao número de ICP escolhidos.

### **Visão prática sobre o Ponto de Complexidade Intrínseca (ICP)**

Definiu que para os projetos em Java que escrevemos, vamos considerar os itens abaixo como ICP:

- [ ] Padrões de branches de código (if, else, loops, when, case do when, try, catch);
- [ ] Funções como argumento;
- [ ] Condicionais;
- [ ] Acoplamento com classes específicas do projeto;
- [ ] Herança de classe abstrata ou concreta (_extends_).

Cada equipe pode definir seu conjunto de ICP e revisitá-lo com frequência. Até porque a combinação de níveis de habilidade da equipe pode influenciar no escopo do projeto e em vários outros fatores que afetam a qualidade e complexidade do código. Outro detalhe bem interessante é que o conjunto de itens influencia diretamente no estilo de código. 

Algumas dicas práticas para escolher e trabalhar melhor com ICPs:

- [ ] Herança foi escolhida como ICP? O recado é: Use com moderação. 
- [ ] Condicional foi escolhida como ICP? O recado é: Não crie if com várias condicionais
- [ ] Função como argumento foi escolhida como ICP? O recado é: Não exagerar em transformação de coleção. 
- [ ] Apenas acoplamento com classe específica foi escolhido como ICP? O recado é: Saiba das tecnologias que sustentam o projeto, vamos usar sem moderação.

A definição do limite de ICP por unidade de código ainda precisa de muita exploração. O importante para o _Cognitive-Driven Development_ (CDD) é que exista um conjunto de itens claros que a equipe considere que dificulta o entendimento, assim como um limite estabelecido.