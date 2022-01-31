## Introdução Arrays

O array é uma estrutura de dados que armazena valores do mesmo tipo, com um tamanho fixo. Um array também é conhecido como retorno, matriz ou arranjo.
É como se fosse uma variável e dentro desta variável irá armazenar diversos itens do mesmo tipo e pode acessá-lo através de uma posição (índice) de onde o elemento se encontra.

- int[] array = new int[4]; - (inteiro que aceitará apenas quatro elementos);
- int[] array = new int[] { 42, 75, 74, 61 }; - (não tem limite, mas tem valores declarados);
- string[] nomes = { "Jan", "Fev" };

-----------------------------

#### Disposição do Array

Índice: É a posição de um determinado valor de um array, sempre começando com zero.

- var elemento = array[0]
- array[0] = 42

-----------------------------

#### Array Multidimensional

O array pode possuir mais de uma dimensão:

- int[,] array = new int[4, 2];

4 = Número de linhas

2 = Número de colunas

- Acessar um valor: array[1, 1]

