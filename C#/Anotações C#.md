### O que é C#?

Uma linguagem elegante, orientada a objetos fortemente tipada.
A sintaxe orientada a objetos foi baseada no C++ e possui influências de outras linguagens de programação como Object Pascal e Java. 
Suporta os conceitos de encapsulamento, herança e polimorfismo (OO)

Os programas C# são executados no .NET, que inclui:
- CLR (Common Language Runtime);
- Conjunto unificado de biblioteca de classes.

Atualmente o compilador do C# é o Roslyn.

---------------------------

### Como funciona?

O código-fonte escrito em C# é compilado em uma linguagem intermediária (IL)

O código e os recursos de IL são armazenados no disco em um arquivo executável chamado assembly, geralmente com uma extensão .exe ou .dll

Quando o programa C# é executado, o assembly é carregado no CLR

Em seguida o CLR executará a compilação "just in time" (JIT) para converter o código IL em instruções de máquina nativas.

O CLR também fornece outros serviços:
- Garbage Collector (ferramenta que trabalha coletando o lixo, liberando espaço na memório excluindo arquivos que não estão sendo utilizados);
- Exception Handler (receber e controlar as excessões de erros que ocorrem no código);
- Resources Manager (gerenciador de recursos).

![image](https://user-images.githubusercontent.com/86674024/150872210-a0a60af1-651b-4207-afa6-a95d307559c3.png)

Além dos serviços de tempo de execução, o .NET também inclui uma extensa biblioteca com milhares de classes que fornecem uma ampla variedade de funcionalidades úteis, desde entrada e saída de arquivos, manipulação de cadeias de caracteres, análise XML, etc.

# Anotações gerais

Concatenar: ${texto ou código}

i++ = i+1

! = expressão de negativa no código C#

args / args.Length = argumentos

override = sobrescrever (uma classe filha, pode sobrescrever uma classe mãe)

ref = referência um determinado metódo dentro do código, se este metódo sofre alteração, todas as suas referencias serão alteradas.

Para fazer uma classe herdar uma herança: public class _aluno_ : _Pessoa_ (exemplo de classe _aluno_ herdando da classe _Pessoa_)

Quando se trata de propriedade quando tem o sinal de "=" estamos chamando o set (atribuir valor), e sem ele estamos chamando o get (apenas acessar o valor).

---------------------------

# Comandos Úteis

Para comentar um parágrafo inteiro: ctrl + K e depois sem soltar o ctrl, tecle "c".

Carregar a opção de auto completar da extensão: F1 / Digitar OmniSharp: Select Project.

Verificar resolução do erro sublinhado em vermelho: ctrl + ". (ponto)".

Atralho para criar construtores, digite: ctor + tab

Atralho para criar Consoles, digite: cw + tab

---------------------------

# Criar um projeto

Na pasta a onde quer salvar o projeto, vá na barra de pesquisa e digite _cmd_ para abrir o terminal da pasta atual.

Para criar uma solução, digite: dotnet new sln --name (nome da solução) 
Para criar um projeto do tipo console, digite: dotnet new console --name (nome do projeto)
Para adicionar o projeto criado na solução criada, digite: dotnet sln add (nome da solução)/(nome do projeto).csproj
Para abrir o .NET code, digite: code ". (ponto)". 
