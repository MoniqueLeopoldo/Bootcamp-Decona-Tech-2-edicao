#### Por que armazenar dados?

Um banco de dados é uma forma de guardar informações para serem reutilizadas no futuro, sendo também uma forma de controlar seus negócios.

#### O que são bancos de dados?

São informações (dados) armazenados em algum lugar que poderão ser reaproveitados em determinado momento.

#### Por que armazenar dados?

Um banco de dados é uma forma de guardar informações para serem reutilizadas no futuro.

#### O que são SGBDs?

São Softwares que padronizam os bancos de dados. 
Sua principal característica é lidar com o padrão de dados armazenados e seu uma interface entre o sistema/pessoas e os dados.
Outra característica é poder realizar o cadastramento das pessoas que teram acesso a esses dados e cada usuário teria níveis de permissões diferente a fim de proteger as informações.

#### Tipos de bancos de dados:

_Relacionais_- São para sistemas que precisam de uma alta confiabilidade dos dados:
- SQL Server;
- Oracle;
- MySQL.

_NoSQL_- São voltados para um melhor performace, que armazena uma grande quantidades de dados de forma eficiente (bigdata), tendo ferramentas que facilitam sua utilização:
- MongoDB;
- Neo4j;
- Firebase.

#### Representação banco relacional:

Uma tabela no banco de dados é como uma planilha no excel, com linhas (registros) e colunas (informações daquele registro).

#### Atomicidade:

Controle sobre inicio e fim da transação, é a garantia que todo o bloco de transações foi executado integralmente. 
Consistência: A garantia de que um dado está íntegro durante e após a transação.

#### Consistência dos dados:

Validar é determinar se os dados capturados pelo sistema cumprem as regras lógicas definidas para manter a sua consistência. 
Também é preciso ressaltar que a consistência dos dados influencia diretamente a qualidade do software, interferindo na forma como o usuário interage com a aplicação.
Quando o banco está espelhado (segregado) para agilizar os processor, e receber uma solicitação de consulta só irá mostrar a informação que consta (persiste) em todos os espelhos, ou seja, a informação será mostrada assim que for replicada em todos os espelhos essa é uma diferença entre os bancos relacionais e os demais.  

#### Normalização de dados:

A normalização tem dois objetivos principais: 
- 1) garantir a integridade dos dados, evitando que informações sem sentido sejam inseridas; 
- 2) organizar e dividir as tabelas da forma mais eficiente possível, diminuindo a redundância e permitindo a evolução do banco de dados com o mínimo de efeito colateral.

-----------------------------

#### Comando _join_:

- inner join: retorna os registros que são comuns às duas tabelas. select * from (nome da tabela) inner join (o que quer comparar) on (da tabela 1) = (da tabela 2)
- left join: retorna os registros que estam na tabela à esquerda. select * from (nome da tabela) left join (o que quer comparar) on (da tabela 1) = (da tabela 2)
- right join: retorna os registros que estam na tabela à direira. select * from (nome da tabela) right join (o que quer comparar) on (da tabela 1) = (da tabela 2)

-----------------------------

### Alguns comandos:

Criação de tabela: create table (nome da tabela);

Inserir dados: insert (nome da tabela) values (informações a seres inseridas);

Inserir dados de colunas: insert into (nome da tabela) (informações a seres inseridas [código, nome, TipoPessoa]);

Visualizar os dados da tabela: select * (o * representa que quer selecionar toda a tabela) from (nome da tabela);

Apagar tabela: drop table (nome da tabela);

Atualizar a informações na tabela: Update (nome da tabela) set (informações a seres inseridas).

Deletar dados: delete from (nome da tabela)

Retornar a data e hora da criação da tabela: getdate()

Retornar X valor caso o informação for nula: select isnull(parâmetro, [o que quer retornar se o valor for nulo]) from (noma da tabela)

Conversão: select convert(parâmetro, [o que quer converter]) from (noma da tabela)

Agrupar por: group by (tabela 1), (tabela 2) 

Ordenar por: order by (tabela 1), (tabela 2) 


-----------------------------

### Anotações gerais:

varchar: informações alfa numéricas com limite de 4.000.

char: informações alfa numéricas com um número fixo de 10 caracteres que quando não declaradas são preenchidas com espaços até completar sua quantidade fixa.

int: números inteiros, positivos ou negativos.

bigint: números inteiros maiores.

bit: aceita apenas 0 (falso) ou 1 (verdadeiro).

Após o comando _select_, se selecionar o nome da tabela e dar o comando "alt + F1" irá vizualizar especificações da tabela.

Where: condicional que pode ser usado juntos com os comando de update, select e delete, por exemplo.

In: o que está contido na tabela.

not in: o que não está contido na tabela.

count: recurso que serve para contar determinada informação da tabela 

-----------------------------

#### _Tabela Verdade_:

- And: Para uma informação ser declarada verdadeira, tudo precisar ser verdadeira. Para ser falso, basta uma ser falsa.

- Or: Para uma informação ser declarada verdadeira, basta uma ser verdadeira. Para ser falso, todos precisam ser falsas.

![image](https://user-images.githubusercontent.com/86674024/151688253-27e3de8a-df3b-4d80-a8ea-28ff9df5db62.png)


