Estrutura de programa

Programas C# consistem em um ou mais arquivos, sendo que, os programas declaram tipos, que contêm membros e podem ser organizados em namespaces. Classes e interfaces são exemplos  de tipos. Campos, métodos, propriedades e eventos são exemplos de membros.

Os principais conceitos organizacionais em C# são:
- programas;
- namespaces;
- tipos (classes e interfaces);
- membros (campos, métodos, propriedades e evento);
- assemblies.

Programas

Quando os programas C# são compilados, eles são fisicamente empacotados em assemblies. Os assemblies geralmente têm a extensão de arquivo .exe ou .dll, dependendo se são aplicações ou bibliotecas.

Instruções

Ações de um programa são expressadas usando instruções

{
Um bloco que permite que várias instruções sejam escritas em constextos.
}

- Declaração de variáveis e constantes locais;
- if (condicional);
- switch (condicional);
- while (repetição);
- do (repetição);
- for (repetição);
- foreach (repetição).
- breack (auxiliar as outras ferramentas);
- continue (auxiliar as outras ferramentas);
- return (auxiliar as outras ferramentas);
- throw (tratativas de exceção);
- try.. catch.. finally (tratativas de exceção);
- using (importar referências a pacotes e namespaces no projeto);

---------------------------

Namespace

Os namespace são usados para organizar classes dentro do código.
Para usar uma classe de outro namespace, colocamos "using System" no começo do código ou colocando "System." antes da string.
Não pode ter duas classes iguais dentro de uma Namespace.

---------------------------

Tipos

Variáveis de tipos de valor contêm diretamente seus dados. As variáveis têm sua própria cópia dos dados e não é possível que as operações afetem outra variável (exceto no caso das variáveis de paramêtro "ref" e "out".

Numéricos: sbyte, short, int, long, byte, ushort, uint, ulong.

Caracteres Unicode: char.

Pontos flutuantes: float, double, decimal

Booleano: bool

enum, struct e tipos nullable (pode receber valores nulos), (exemplo int?)

Referência

Variáveis de tipos de referência armazenam referências a seus dados. É possível que duas variáveis façam referência ao mesmo objeto e, portanto, que operações em uma variável afetem o objeto referenciado pela outra variável.

Classe

Uma clase pode ter campos, propriedades, metódos e eventos dentro dela que são denominados membros.
Quando uma classe é instanciada, essa instância é chamada de objeto, e nesse objeto podem ser criados os valores de acordo com os campos da classe.
O valor não fica quardado na classe, sendo possível reutilizá-la.
- class, object, string (trabalhar com textos).

Tipos Arrays: int[], int[,], etc...

Delegate

Interface

É como uma classe base que serve de molde para várias classes.
Uma classe que implementa uma interface deve implementar todos os membros.
Ele sempre precisa da lera "I" antes do nome.


Enum

Declara um conjunto de constantes nomeadas que começam do 0 e aumentam de 1 em 1.

---------------------------

Debugging

A depuração pode ser feita colocando um BreakPoint no canto esquerdo do código ou apertando F9 e executando ele.
O código vai parar onde foi colocado o BreakPoint e então o código poderá ser inspecionado.

---------------------------

Variável: posso atribuir diversos valores

Constante: seu valor não pode ser alterado
