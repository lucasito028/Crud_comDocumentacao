#  Fazendo Apenas Backend de Manter Pessoa

- [1. Introdução ](#1-Introdução)
- [2. Classes ](#2-Classes)


## 1. Introdução

  Fazendo o requisito de manter Pessoa:<br>
* cadastrar <br>
* alterar <br>
* deletar  <br>
* selecionar<br>

## 2. Classes
  As classes são usando usando 3 pilares de OOP: Herança. Abstração e Encapsulamento:<br>

* Keys - Seria a chave para acessar o banco de dados<br>
Atributos: <br>
host = "localhost";<br>
user = "root";<br>
db = "itospet";<br>
senha = "";<br>
port = 3306;<br>
object $conn;<br>

* MysqlDatabase - Classe abstrata - Responsável pela conexão do banco de dados na qual suas classes filhas pudesse conectar<br>
Metodos: connect();<br>
select()<br>
create()<br>
Update()<br>
delete()<br>

* Pessoa - Classe filha de "MysqlDatabase" na qual seria responsável por fazer as operações do CRUD da tabela Pessoa e pode ser instanciada a objeto<br>
Metodos: connect()<br>
select()<br>
create()<br>
update()<br>
delete()<br>

* BancoDeDados - Interface - na qual seria implementada pela classe MysqlDatabase ter uma função para conectar o banco de dados<br>
Metodos: connect()<br>



