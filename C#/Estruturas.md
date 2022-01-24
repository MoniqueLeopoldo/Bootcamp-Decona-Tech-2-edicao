Estrutura de programa

Programas C# consistem em um ou mais arquivos, sendo que, os programas declaram tipos, que contêm membros e podem ser organizados em namespaces. Classes e interfaces são exemplos  de tipos. Campos, métodos, propriedades e eventos são exemplos de membros.

Os principais conceitos organizacionais em C# são:
- programas;
- namespaces;
- tipos (classes e interfaces);
- membros (campos, métodos, propriedades e evento);
- assemblies.

Quando os programas C# são compilados, eles são fisicamente empacotados em assemblies. Os assemblies geralmente têm a extensão de arquivo .exe ou .dll, dependendo se são aplicações ou bibliotecas.









Namespace

Os namespace são usados para organizar classes dentro do código.
Para usar uma classe de outro namespace, colocamos "using System" no começo do código ou colocando "System." antes da string.
Não pode ter duas classes iguais dentro de uma Namespace.


Classe

Uma clase pode ter campos, propriedades, metódos e eventos dentro dela que são denominados membros.
Quando uma classe é instanciada, essa instância é chamada de objeto, e nesse objeto podem ser criados os valores de acordo com os campos da classe.
O valor não fica quardado na classe, sendo possível reutilizá-la.


Interface

É como uma classe base que serve de molde para várias classes.
Uma classe que implementa uma interface deve implementar todos os membros.
Ele sempre precisa da lera "I" antes do nome.


Enum

Declara um conjunto de constantes nomeadas que começam do 0 e aumentam de 1 em 1.


Debugging

A depuração pode ser feita colocando um BreakPoint no canto esquerdo do código ou apertando F9 e executando ele.
O código vai parar onde foi colocado o BreakPoint e então o código poderá ser inspecionado.
