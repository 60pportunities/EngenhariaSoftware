**Object Calisthenics** foi introduzido por [**Jeff Bay**](http://www.xpteam.com/jeff/) e publicado no seu livro chamado [**Thought Works Anthology**](https://pragprog.com/book/twa/thoughtworks-anthology)
https://github.com/ghas-bootcamp/ghas-bootcamp?tab=readme-ov-file

https://github.com/advanced-security
https://github.com/advanced-security/codeql-sap-js


A principal motivação para o **Object Calisthenics** é aplicar alguns princípios do **SOLID.** 

Basicamente são um conjunto de boas práticas e regras de programação para aumentar a qualidade do seu código.

São 9 regras básicas do **Object Calisthenics**:

1. **Only One Level Of Indentation Per Method**
2. **Don’t Use The ELSE Keyword**
3. **Wrap All Primitives And Strings**
4. **First Class Collections**
5. **One Dot Per Line**
6. **Don’t Abbreviate**
7. **Keep All Entities Small**
8. **No Classes With More Than Two Instance Variables**
9. **No Getters/Setters/Properties**

Um método deve ter apenas um nível de indentação. Se um método tiver mais de um nível de indentação, é sinal de que ele está fazendo mais do que deveria. Para resolver esse problema, o método deve ser dividido em vários métodos menores, cada um com uma única responsabilidade.




1 - Use apenas um nível de indentação por método



Um método deve ter apenas um nível de indentação. Se um método tiver mais de um nível de indentação, é sinal de que ele está fazendo mais do que deveria. Para resolver esse problema, o método deve ser dividido em vários métodos menores, cada um com uma única responsabilidade.



2 - Não use else



O uso de else torna o código mais difícil de entender e manter. Em vez disso, devemos usar polimorfismo e estruturas de controle que não precisam de else para evitar a repetição de código.



3 - Envolva todas as estruturas primitivas e Strings em classes



O uso de tipos primitivos e Strings torna o código mais difícil de entender e manter. Em vez disso, devemos criar classes para representar esses tipos e encapsular a lógica relacionada a eles. Isso torna o código mais legível e reduz a quantidade de código duplicado.



4 - Envolva suas collections em classes



Um conjunto de elementos e quiser manipulá-los, é necessário criar uma classe dedicada collection apenas para este conjunto. Assim, ao atualizar aquele valor, com certeza será em sua collection.



5 - Use apenas uma classe por arquivo



Cada arquivo deve conter apenas uma classe. Isso torna o código mais fácil de encontrar e entender. Além disso, ajuda a evitar a dependência desnecessária de outras classes.



6 - Não abrevie nomes



Nomes de variáveis, métodos e classes devem ser claros e descritivos. Abreviações podem tornar o código mais difícil de entender e manter. Portanto, é importante usar nomes completos e descritivos.



7 - Mantenha todas as entidades pequenas



Cada classe, método e bloco de código deve ser pequeno e fazer apenas uma coisa. Isso torna o código mais fácil de entender, testar e manter. Além disso, ajuda a evitar a repetição de código e a aumentar a coesão do código.



8 - Não use getters e setters



Getters e setters violam o princípio de encapsulamento e tornam o código mais difícil de entender e manter. Em vez disso, devemos criar métodos que representem as ações que desejamos executar em nossos objetos.



9 - Use apenas uma instância de ponto por linha



O uso de várias instâncias de ponto em uma linha torna o código mais difícil de entender e manter. Em vez disso, devemos usar apenas uma instância de ponto por linha para melhorar a legibilidade do código.



Princípios do Object Calisthenics:



Encapsulamento



O encapsulamento é o princípio de ocultar o estado interno de um objeto e fornecer uma interface para interagir com ele. Isso torna o código mais fácil de entender e manter, pois as mudanças no estado interno do objeto não afetam a maneira como ele é usado.



Coesão



A coesão é o princípio de manter as entidades relacionadas juntas em uma única unidade. Isso significa que cada classe deve ter uma única responsabilidade e fazer apenas uma coisa. Quando as entidades estão altamente coesas, o código é mais fácil de entender, testar e manter.



Baixo acoplamento



O baixo acoplamento é o princípio de minimizar as dependências entre as entidades. Isso significa que uma classe deve depender apenas do que é necessário para cumprir sua responsabilidade e não deve depender de outras classes ou módulos desnecessariamente. Quando as entidades têm baixo acoplamento, o código é mais flexível e fácil de evoluir.



Abstração



A abstração é o princípio de representar as entidades do mundo real em um nível mais alto de generalidade. Isso significa que uma classe deve representar um conceito abstrato e não uma implementação concreta. Isso torna o código mais flexível e fácil de evoluir, pois as mudanças na implementação não afetam a interface da classe.



Composição sobre herança



A composição sobre herança é o princípio de que as classes devem ser construídas por meio da composição de objetos existentes, em vez de herdar comportamentos de outras classes. Isso torna o código mais flexível e fácil de evoluir, pois as mudanças na implementação não afetam a interface da classe.



Aplicação prática do Object Calisthenics:



Para aplicar o Object Calisthenics na prática, é necessário seguir as regras e princípios descritos acima. Isso significa que devemos:



Dividir métodos grandes em métodos menores e mais simples



Evitar o uso de else e usar polimorfismo e estruturas de controle que não precisam de else



Criar classes para representar tipos primitivos e encapsular a lógica relacionada a eles



Criar classes para as collections



Criar apenas uma classe por arquivo



Usar nomes descritivos para variáveis, métodos e classes



Manter todas as entidades pequenas e altamente coesas



Evitar o uso de getters e setters e criar métodos que representem as ações que desejamos executar em nossos objetos



Usar apenas uma instância de ponto por linha



Além disso, devemos aplicar os princípios do Object Calisthenics, como encapsulamento, coesão, baixo acoplamento, abstração e composição sobre herança, para tornar nosso código mais flexível, fácil de entender e evoluir.
