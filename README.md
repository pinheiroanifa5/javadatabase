# javadatabase
Criar base dados conectados no java 

criar duas tabelas relacionais para armazenar informaçoes de clientes e trasações em um sistema java. Para isso, foi desenvolvida uma solução que envolve duas classes: User e trasações.
A classe User tem informaçoes sobre o cliente, incluindo nome, endereço e id do cliente, o valor a transferir.
Para criar a relação entre as tabelas, foram utilizadas chaves primarias e estrangeiras. A tabela users possui uma chave primaria "id", que referencia na tabela transação como chave estrangeira "user_id", assim cada transação fica vinculada a um cliente especifico.
A solução foi implementada em java, as informções dos clientes e transações podem ser armazenadas em banco de dados(mysql).
Portanto, a solução desenvolvida tem como objetivo criar duas tabelas que armazenam informações de clientes e transações em sistema java.
Foi criado uma tabela no banco de dados usando o comando CREATE TABLE, especificando as colunas a utelizar, para se comunicar com o banco de dados MySQL em no código Java, utilizei  a API JDBC (Java Database Connectivity), que nos permitiu estabelecer uma conexão com o banco de dados e executar comandos SQL.
Para inserir dados em na tabela MySQL a partir do código Java, usei um objeto PreparedStatement para preparar uma instrução SQL com espaços reservados para os valores a serem inseridos. Em seguida, usei métodos set para fornecer os valores dos espaços reservados, e executeUpdate para executar a instrução. Para recuperar dados da tabela My_SQL a partir do código Java, usei um objeto Statement para criar uma instrução SQL simples. Em seguida, o método executeQuery para executar a instrução e recuperar um objeto ResultSet, que contém os resultados da consulta.
Para lidar com transações em nosso código Java, foi utelizado o métodos setAutoCommit(false) e commit() para desativar o modo autocommit e confirmar a transação. 

