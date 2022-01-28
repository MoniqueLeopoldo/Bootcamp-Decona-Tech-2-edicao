Estruturas do Programa
--

Programas C# consistem em um ou mais arquivos, sendo que, os programas declaram tipos, que contêm membros e podem ser organizados em namespaces. Classes e interfaces são exemplos  de tipos. Campos, métodos, propriedades e eventos são exemplos de membros.

Os principais conceitos organizacionais em C# são:
- programas;
- namespaces;
- tipos (classes e interfaces);
- membros (campos, métodos, propriedades e evento);
- assemblies.

---------------------------

### Programas

Quando os programas C# são compilados, eles são fisicamente empacotados em assemblies. Os assemblies geralmente têm a extensão de arquivo .exe ou .dll, dependendo se são aplicações ou bibliotecas.

---------------------------

### O que é a POO (programação orientada a objetos? 

A POO é um paradigama de programação, ou seja, corresponde a uma técnica de programação para um fim específico.

Dentro desta técnica, existem quatro pilares:

- Abstração, abstrair um objeto do mundo real para um contexto específico, considerando apenas os atributos importantes.

- Encapsulamenteo serve para proteger uma classe e definir limites para alterações de suas propriedades. Também serve para ocultar seu comportamento e expor somente o necessário.

![image](https://user-images.githubusercontent.com/86674024/151057191-92ac55bf-762e-4873-b864-1d8ffecc9090.png)


- Herança nos permite reutilizar atributos, métodos e comportamentos de uma classe em outras classes. Serve para agrupar objetos que são do mesmo tipo, porém com características diferentes. 

- Polimorfismo vem do grego e significa "muitas formas". Com o polimorfismo podemos sobrescrever métodos das classes filhas para que se comportem de maneira diferente e ter sua própria implementação.

Polimorfismo em tempo de compilação (Overload/Early Binding);

Criar vários métodos com o mesmo nome, mas cada qual terá seu parâmetro, sendo possível utilizar quaisquer um deles.

Polimorfismo em tempo de execução (Override/Late Binding)

É possível sobrescrever um método de uma classe herdada da seguinte forma: public virtual void ..... (autorizar sobrescrever) / public override void .... (está sobrescrevendo)

---------------------------

### Paradigmas de programação

Uma paradigma é um conjunto regras, técnicas e modelos, ou seja, nada mais é do que um modelo de técnicas, estruturas e formas de solucionar um problema.

Uma linguagem de programação implementas um ou mais paradigmas.

Tipso de paradigmas:
- Programação orientada a objetos POO (se aproxima ao mundo real);
- Programação estruturada;
- Programação imperativa;
- Programação procedural;
- Programação orientada a eventos;
- Programação lógica.
- Etc....

---------------------------

### Instruções

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

### Namespace

Os namespace são usados para organizar classes dentro do código.
Para usar uma classe de outro namespace, colocamos "using System" no começo do código ou colocando "System." antes da string.
Não pode ter duas classes iguais dentro de uma Namespace.

---------------------------

### Tipos

Variáveis de tipos de valor contêm diretamente seus dados. As variáveis têm sua própria cópia dos dados e não é possível que as operações afetem outra variável (exceto no caso das variáveis de paramêtro "ref" e "out".

Numéricos: sbyte, short, int, long, byte, ushort, uint, ulong.

Caracteres Unicode: char.

Pontos flutuantes: float, double, decimal

Booleano: bool

enum, struct e tipos nullable (pode receber valores nulos), (exemplo int?)

---------------------------

### Referência

Variáveis de tipos de referência armazenam referências a seus dados. É possível que duas variáveis façam referência ao mesmo objeto e, portanto, que operações em uma variável afetem o objeto referenciado pela outra variável.

---------------------------

### Classe

São os tipos mais fundamentais de C#, sendo ela uma estrutura de dados que combina estado (campos) e ações (métodos). 

Uma clase pode ter campos, propriedades, metódos e eventos dentro dela que são denominados membros.
Quando uma classe é instanciada, essa instância é chamada de objeto, e nesse objeto podem ser criados os valores de acordo com os campos da classe.
O valor não fica guardado na classe, sendo possível reutilizá-la.

As classes suportam herança e polimorfismo, mecanismos pelos quais as classes derivadas podem entender e especializar as classes base.

- class;
- object;
- string (trabalhar com textos).

Instâncias de classes (objetos) são criadas usando o operador _new_, que aloca memória para uma nova instância, chama um construtor para inicializar a instância e retorna uma referência à instância.

Ponto p1 = new Ponto (0 [X], 0[Y]);

Ponto p2 = new Ponto (10, 20);

A memória ocupada por um objeto é recuperada automaticamente quando o objeto não está mais acessivél. Não é necessário nem possível desalocar explicitamente objetos em C#.

---------------------------

### Classe abstrata

Uma classe abstrata tem como objetivo ser exclusivamente um modelo para ser herdado, portanto não pode ser instanciada. Você pode implementar métodos ou deixá-los a cargo de quem herdar, ou seja, não pode ser alterada diretamente, sendo necessário a sua implementação "sobrescrever".

---------------------------

### Classe selada (class sealed)

Uma classe selada tem como objetivo impedir que outras classes façam uma herança dela, ou seja, nenhuma classe pode ser sua derivada. Também existem métodos e propriedades seladas, que no caso, não permite polimorfismo (que seja sobrescrita).

---------------------------

### Classe object

A classe System.Object é a mãe de todas as classes na hierarquia do .NET. Todas as classes derivam, diretamente ou indiretamente da classe Object, e ela tem como objetivo prover serviços de baixo nível para suas classes filhas.

---------------------------

### Membros

Os membros de uma classe podem ser estáticos ou memebros da instância.

Membros estáticos pertencem a classe e membros de isntância pertencem ao objeto.

Constantes, variáveis, métodos, propriedades, construtores, etc...

---------------------------

### Acessibilidade

Cada membro de uma classe tem uma acessibilidade associada, que controla as regiões do texto do programa que podem acessar o membro.

Pode ser:
- public (pode ser acessada por qualquer classe do código em geral);
- protected (só quem está dentro de seus {} herdará esta condição);
- internal;
- private (só pode ser acessada na classe a qual está este código).

---------------------------

### Herança

Uma declaração de classe pode especificar uma classe base, herdando os membros _public_, _internal_ e _protected_ da classe base.

Omitir uma especificação de classe base é o mesmo  que derivar do tipo _object_.

---------------------------

### Metódos 

Um metódo é um membro que implementa uma computação ou ação que pode ser executada por um objeto ou classe.

Os métodos podem ter uma lista de parâmetros, que representam valores ou referências de variáveis passados para o método, e um tipo de retorno, que especifica o tipo de valor calculado e retornado pelo metódo.

---------------------------

### Tipos Arrays

Um array é uma estrutura de dados que contém um número X de elementos, todos do mesmo tipo que são acessados através de índeces computados.

Arrays são tipos de refência e a declaração de uma variável _array_ simplesmente reserva espaço para uma referência de uma instância de _array_

Ao criar uma array é especificando o tamanho da nova instância, que é fixo durante todo o tempo de vida da instância.

Os índices dos elementos de um array variam de 0 a comprimento do array - 1. 

exemplos de arrays: 
- int[];
- int[,]; etec...

---------------------------

### Interface (ele sempre precisa da lera "I" antes do nome.)

É como uma classe base que serve de molde para várias classes. Uma interface define um contrato que pode ser implementado por classes e _structs_.
Uma classe que implementa uma interface deve implementar todos os membros. Uma interface pode conter métodos, propriedades, eventos e indexadores.

É como se fosse uma classe abstrata, podendo definir métodos abstratos para serem implementados.

Uma interface não fornece implementações dos membros que define - apenas suas "assinaturas".

As interfaces podem empregar herança múltipla, ou seja, obrigando a utilizar o metódo que esta interface usa.

---------------------------

### Structs

Como as classes, as _structs_ são estruturas de dados que podem conter membros de dados e membros de ação, mas diferentemente das classes, as _structs_ são tipos de valor e não requerem alocação de heap (local onde está o dado original da referência).

Uma variável de um tipo de _struct_ armazena diretamente os dados da estrutura, enquanto uma variável de um tipo de classe armazena uma referência a um objeto alocado na memória.

Structs não aceita herança determinada pelo desenvolvedor.

São úteis para pequenas estruturas de dados que possuem semântica de valor: números complexos, pontos em um sistema de coordenadas ou pares de chave-valor em um dicionário são bons exemplos de utilização.

Seu uso em vez de classes para pequenas estruturas de dados podem fazer uma grande diferença no número de alocações de memória.

Constutores de _structs_ são chamados como o operador _new_, semelhante a um construtor de classe, mas em vez de alocar dinamicamente um objeto no _heap_ gerenciado e retornar uma referência a ele, um construtor _structs_ simplemente retorna o próprio valor _structs_ (normalmente em um local temporário na _stack_), e esse valor é copiado conforme necessário.

---------------------------

### Enum

Declara um conjunto de constantes nomeadas que começam do 0 e aumentam de 1 em 1.

Um _enum_ é um tipo de valor distinto com um conjunto de constantes nomeadas.

Você define enumerações quando precisa definir um tipo que pode ter um conjunto de valores discretos. Eles usam um dos tipos de valor integral como armazenamento subjacente. Eles fornecem significado semântico aos valores discretos.

Cada tipo de _enum_ possui um tipo integral correspondente chamado tipo subjacente do tipo de _enum_

Um tipo de enumeração que não declara explicitamente um tipo subjacente tem um tipo subjacente _int_

---------------------------

### Debugging

A depuração pode ser feita colocando um BreakPoint no canto esquerdo do código ou apertando F9 e executando ele.
O código vai parar onde foi colocado o BreakPoint e então o código poderá ser inspecionado.

---------------------------

# Anotações gerais

Diferença entre classe e objeto... A classe é um molde, uma abstração do mundo real a qual eu quero representar e o objeto é a construções dessa classe. Exemplo: Bob (pessoa) é um objeto e suas carecterísticas que o compõem como pessoa são as classes (cor do cabelo, tamanho, peso...) e a ação que ele fará é o método.

Variável: posso atribuir diversos valores

Constante: seu valor não pode ser alterado

Concatenar: ${texto ou código}

i++ = i+1

! = expressão de negativa no código C#

args / args.Length = argumentos

override = sobrescrever (uma classe filha, pode sobrescrever uma classe mãe)

ref = referência um determinado metódo dentro do código, se este metódo sofre alteração, todas as suas referencias serão alteradas.

Para fazer uma classe herdar uma herança: public class _aluno_ : _Pessoa_ (exemplo de classe _aluno_ herdando da classe _Pessoa_)

O que diferencia um metódo do outro são seus parâmetros que no caso são suas assinaturas.

---------------------------

# Comandos Úteis

Para comentar um parágrafo inteiro: ctrl + K e depois sem soltar o ctrl, tecle "c".

Carregar a opção de auto completar da extensão: F1 / Digitar OmniSharp: Select Project.

Verificar resolução do erro sublinhado em vermelho: ctrl + ". (ponto)".
