Ouvidoria Connect
📌 Sobre o Projeto:


O Ouvidoria Connect é um sistema de ouvidoria desenvolvido em Python com integração ao MySQL.


🎯 Objetivos:

Registrar manifestações dos usuários.
Organizar as informações em um banco de dados.
Permitir a consulta e o gerenciamento dos registros.
Aplicar conceitos de programação, banco de dados e integração entre sistemas.


⚙️ Funcionalidades:


➕ Inserir uma nova manifestação;
🔢 Exibir a quantidade de comentários cadastrados;
📋 Listar todas as manifestações registradas;
🔍 Pesquisar uma manifestação pelo código;
🏷️ Pesquisar manifestações por categoria;
✏️ Atualizar um comentário pelo código;
🗑️ Excluir uma manifestação pelo código.


Categorias de Manifestação:


Sugestão;
Reclamação;
Elogio.


🛠️ Tecnologias Utilizadas:


Python 3
MySQL
MySQL Connector for Python
PyCharm


Estrutura do Projeto: 


menu.py → Menu principal e interação com o usuário.
operacoesbd.py → Responsável pela conexão e operações com o banco de dados.
Ouvidoria.py → Contém as funcionalidades de cadastro, consulta, atualização e exclusão das manifestações.


COMO UTILIZAR O SISTEMA:


1. Clone o repositório: git clone <link-do-repositorio> cd Ouvidoria-Connect;
2. Instale as dependências: Este projeto utiliza o conector do MySQL para Python. Para instalá-lo, execute:

pip install mysql-connector-python ou py -m pip install mysql-connector-python.

3. No MySQL Workbench, crie o banco de dados:

CREATE DATABASE ouvidoria;
USE ouvidoria;

4. Em seguida, crie a tabela utilizada pelo sistema:

CREATE TABLE ouvidoria (
    codigo INT AUTO_INCREMENT PRIMARY KEY,
    categoria VARCHAR(50),
    titulo VARCHAR(100),
    comentario TEXT);

5. No arquivo operacoesbd.py, verifique se os dados de conexão estão corretos:

host = "127.0.0.1"
user = "root"
password = "sua_senha"
database = "ouvidoria" 

6. Execute o sistema!
