# Design Patterns

### Alguém já resolveu o seu problema!"

São soluções elegantes, testadas e aprovadas para problemas recorrentes que temos no design e implementação de software.

Surgiram da experimentação e repetição. 

Não é um padrão pronto para ser aplicado no seu código, é uma descrição/template de como resolver o seu problema nas mais diferentes situações.

Os mais utilizados são:
- Adapter;
- Factory;
- Observer;
- Strategy;
- Builder;
- State;
- Singleton.

-------------------------------------

#### GOF - Gang of Four

Criaram a "bíblia" sobre o assunto. Catalogaram 23 patterns divididos em 3 grupos: 
- Creational Pattern;
- StructuralPattern;
- Behavioral Pattern.

-------------------------------------

#### Hands On

_Singleton_

Garante uma única instância da classe e um acesso global para ela, ou seja, centraliza e compartilha recursos.

_Repository_

Faz a abstração ("meio de campo") entre o seu domínio e sua camada de dados, ou seja, contribui para o isolamento da camada de acesso a dados.

_Facade_

Define uma interface que abstrai a complexidade de interface de subsistemas, ou seja, simplifica a utilização de subsistemas complexos.

-------------------------------------

#### Anotações Gerais

Pacote de Instalação: Na aba Browse, instalar _Swashbuckle.AspNetCore_. Para ativar: Botão direito na aplicação... em propriedades... Build... Ticar a opção _XML documentation File_ (facilita na hora de visualizar seu projeto)

Adicionar as seguintes informações em _services.AddControllers()_;

![image](https://user-images.githubusercontent.com/86674024/151639163-275e8077-f4cf-421c-8cf9-1805ded28a55.png)

Adicionar as seguintes informações em _app.UseDeveloperExceptionPage_;

![image](https://user-images.githubusercontent.com/86674024/151639240-b203c2bb-a048-4b26-9435-685451f6537b.png)


Qual Entity Framework instalar: Microsoft.EntityFrameworkCore.InMemory. E para ativalo...

![image](https://user-images.githubusercontent.com/86674024/151685547-2f236720-e2ac-49a5-b4f7-8a7650b51b7a.png)


