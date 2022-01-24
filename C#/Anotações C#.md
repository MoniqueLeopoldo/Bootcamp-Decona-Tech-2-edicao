O que é C#?

Uma linguagem elegante, orientada a objetos fortemente tipada.
A sintaxe orientada a objetos foi baseada no C++ e possui influências de outras linguagens de programação como Object Pascal e Java. 
Suporta os conceitos de encapsulamento, herança e polimorfismo (OO)

Os programas C# são executados no .NET, que inclui:
- CLR (Common Language Runtime);
- Conjunto unificado de biblioteca de classes.

Atualmente o compilador do C# é o Roslyn.

---------------------------

Como funciona?

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
