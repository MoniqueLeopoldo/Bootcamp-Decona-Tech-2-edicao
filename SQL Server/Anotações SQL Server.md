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


