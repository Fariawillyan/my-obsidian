


O **Strategy** é um padrão de projeto comportamental que permite que você defina uma família de algoritmos, coloque-os em classes separadas, e faça os objetos deles intercambiáveis.

- Usar quando possuir diversos algoritmos.
- Delegar a execução do algoritmo para uma instancia que compõe a classe principal.

##  Prós

-  Você pode trocar algoritmos usados dentro de um objeto durante a execução.
-  Você pode isolar os detalhes de implementação de um algoritmo do código que usa ele.
-  Você pode substituir a herança por composição.
-  Princípio aberto/fechado [[OCP]]. Você pode introduzir novas estratégias sem mudar o contexto.

##  Contra

-  Aumento do número de classes, "uma para cada algoritmo".
-  Se você só tem um par de algoritmos e eles raramente mudam, não há motivo real para deixar o programa mais complicado com novas classes e interfaces que vêm junto com o padrão.
-  Os Clientes devem estar cientes das diferenças entre as estratégias para serem capazes de selecionar a adequada.
-  Muitas linguagens de programação modernas tem suporte do tipo funcional que permite que você implemente diferentes versões de um algoritmo dentro de um conjunto de funções anônimas. Então você poderia usar essas funções exatamente como se estivesse usando objetos estratégia, mas sem inchar seu código com classes e interfaces adicionais.


Referência:
https://refactoring.guru/pt-br/design-patterns/strategy
