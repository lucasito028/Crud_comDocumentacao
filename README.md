# Crud_comDocumentacao

- [1. Introdução ](#1-Introdução)
- [2. Classes ](#2-Classes)


## 1. Introdução

  Fazendo o requisito de manter Pessoa: 
* cadastrar 
* alterar 
* deletar  
* selecionar

## 2. Classes
  As classes são usando Herança. Abstração e Encapsulamento:

* Keys - Seria a chave para acessar o banco de dados
Atributos: 
host = "localhost";
user = "root";
db = "itospet";
senha = "";
port = 3306;
object $conn;

* MysqlDatabase - Classe abstrata - Responsável pela conexão do banco de dados na qual suas classes filhas pudesse conectar
Metodos: connect();
select()
create()
Update()
delete()

* Pessoa - Classe filha de "MysqlDatabase" na qual seria responsável por fazer as operações do CRUD da tabela Pessoa 
Metodos: connect()
select()
create()
update()
delete()

* BancoDeDados - Interface - na qual seria implementada pela classe MysqlDatabase ter uma função para conectar o banco de dados
Metodos: connect()



