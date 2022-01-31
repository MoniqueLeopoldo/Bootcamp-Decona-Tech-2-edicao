## Introdução Arrays

O array é uma estrutura de dados que armazena valores do mesmo tipo, com um tamanho fixo. Um array também é conhecido como retorno, matriz ou arranjo.
É como se fosse uma variável e dentro desta variável irá armazenar diversos itens do mesmo tipo e pode acessá-lo através de uma posição (índice) de onde o elemento se encontra.

- int[] arrayInteiros = new int[4]; - (inteiro que aceitará apenas quatro elementos);
- int[] array = new int[] { 42, 75, 74, 61 }; - (não tem limite, mas tem 4 valores declarados, então ele só aceitará 4 elementos);
- string[] nomes = { "Jan", "Fev" };

Depois que a capacidade do array é salvo na memória não é possível alterar sua capacidade para mais ou menos, sendo necessário declarar outro array com a capacidade desejada ou implementar o anterior caso queira aumentar sua capacidade. 

-----------------------------

#### Disposição do Array

Índice: É a posição de um determinado valor de um array, sempre começando com zero.

![image](https://user-images.githubusercontent.com/86674024/151741941-2e545227-14e1-48d8-9f8b-5802d4f76ed0.png)

- var elemento = array[0]
- array[0] = 43 (caso queira alterar o valor do elemento, chame sua posição e depois o novo valor)

-----------------------------

#### Array Multidimensional (muito utilizado para representar matriz)

O array pode possuir mais de uma dimensão:

- int[,] array = new int[4, 2];

4 = Número de linhas

2 = Número de colunas

- Acessar um valor: array[1, 1]

-----------------------------

#### Ordenando Arrays

Para ordenar um array, existem diversos algoritmos de ordenação, diferentes técnicas e casos a serem considerados.

-----------------------------

#### Classe Array

A classe Array é uma classe do C# que nos oferece diversos métodos que nos auxiliam a trabalhar com arrays.

Array.Sort(array)

Array.Copy(array, arrayDestino, array.length) - (o array.length está solicitando que tudo seja copiado)

Array.Exists (saber se o que está pesquisando existe)

Array.TrueForAll (Determina se cada elemento na matriz corresponde às condições definidas pelo predicado especificado)

Array.Find (Pesquisa um elemento que corresponde às condições definidas pelo predicado especificado e retorna a primeira ocorrência em toda a Array)

Array.IndexOf (Pesquisa o objeto especificado e retorna o índice da sua primeira ocorrência em uma matriz unidimensional ou em um intervalo de elementos na matriz)

Array.Resize (redimensionar a capacidade do array, com os mesmos elementos)

Array.ConvertAll (Converte uma matriz de um tipo para uma matriz de outro tipo, converter de String para inteiro, por exemplo) 

-----------------------------

#### Coleção genérica

No C#, existem classes de coleções que agrupam valores, e essas classes são padronizadas para as operações mais comuns, como:

- Ordenação;
- Obter valor por índice;
- Obter valor com expressões;
- Trabalhar com tamanhos dinâmicos.

Uma lista não precisa se preocupar com o tamanho dela como no array, mas trabalha com internamente com o array e caso exceda a capacidade desse array ela automáticamente altera sua capacidade. Ela é genêrica e também é possível acessá-la através de índice e ordená-la. Ela não precisa ser declara com valores na sua criação.

(nome da lista).AddRange (adicionar elemento a lista)

(nome da lista).Insert (1, "RJ") - (adicionar o elemento por índice)

(nome da lista).Remove (nome do elemento) - (adicionar o elemento por índice)

-----------------------------

#### Coleção específica

As coleções específicas implementam regras para sua ordem de acesso e manipulação de seus elementos, são elas:

- Queue (Fila): Obedece a ordem FIFO (First In First Out);

Queue<string> fila = new Queue<string>();
  
(nome da pilha).Enqueue(o que quer inserir) - Inserir elementos na pilha
  
Peek (retorna quem é o primeiro da fila)
  
Dequeue (retorna quem é o primeiro da fila e o remove)

  
- Stack (Pilha): Obedece a ordem LIFO (Last In First Out).

Stack<string> pilha = new Stack<string>;
  
(nome da pilha).Push(o que quer inserir) - Inserir elementos na pilha
  
Peek (retorna quem é o último da pilha)
  
Pop (retorna o elemento do topo da pilha e o removendo)
  
-----------------------------  
  
#### Dicionários

Um dicionário é uma coleção de chave e valor, permitindo que você recupere rapidamente seus itens baseado em sua chave. Não pode duplicar a chave, mas pode repetir o valor.

O dicionário armazena a sua chave em hash.

Criação de um dicionário:
  
Dictionary<string, string> estados = new Dictionary<string,string>()
  
Para percorrer o dicionário utilizamos o comando foreach.

Para atualizar a chave basta colocar o valor de igual após o nome da mesma e em seguida seu novo valor.
  
Para remover a chave: (nome da classe).Remove(nome da chave).
  
Para acessar de maneira segura utilizar o comando TryGetValue.
  
-----------------------------  
  
#### LINQ

O Language-Integrated Query (LINQ) é uma maneira de você utilizar uma sintaxe de consulta padronizada para coleções de objetos.
  
![image](https://user-images.githubusercontent.com/86674024/151754881-ca263854-47c0-44e1-a46a-c87a7b9fbfbf.png)
  
Min() - Retorna os valores mínimos
  
Max() - Retorna os valores máximos
  
Average() - - Retorna os valores médios (É do tipo double)
  
Sum - Soma todos os elementos presentes no array e retorna o novo valor que é o resultado de sua soma.
  
Distinct - Retorna uma nova coleção com valores úncios, retorna valores distintos de uma sequência.
  
-----------------------------

## Anotações Gerais

for (int i = 0, i < arrayInteiros.Length; i++), (o Length, ele percorre todo o array)
                                         
foreach (int _item_ in _collection_) (outro método de percorrer o array) 

