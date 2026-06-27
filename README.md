🏢 Ouvidoria Connect

---

📌 Sobre o Projeto: 

O Ouvidoria Connect é um sistema de ouvidoria desenvolvido em Python com integração ao MySQL, permitindo o cadastro e gerenciamento de manifestações de forma simples e organizada.

---

🎯 Objetivos
Registrar manifestações dos usuários;
Organizar as informações em um banco de dados;
Permitir a consulta e o gerenciamento dos registros;
Aplicar conceitos de programação, banco de dados e integração entre sistemas.

---

⚙️ Funcionalidades
➕ Inserir uma nova manifestação;
🔢 Exibir a quantidade de comentários cadastrados;
📋 Listar todas as manifestações registradas;
🔍 Pesquisar uma manifestação pelo código;
🏷️ Pesquisar manifestações por categoria;
✏️ Atualizar um comentário pelo código;
🗑️ Excluir uma manifestação pelo código.

---

 Categorias de Manifestação
💡 Sugestão;
⚠️ Reclamação;
❤️ Elogio.

---

🛠️ Tecnologias Utilizadas
Python 3
MySQL
MySQL Connector for Python
PyCharm

---

📁 Estrutura do Projeto

menu.py → Responsável pelo menu principal e interação com o usuário.
operacoesbd.py → Responsável pela conexão e operações com o banco de dados.
Ouvidoria.py → Contém as funcionalidades de cadastro, consulta, atualização e exclusão das manifestações.

---

▶️ Como Utilizar o Sistema
1. Clone o repositório
git clone <link-do-repositorio>
cd Ouvidoria-Connect

2. Instale as dependências

Este projeto utiliza o conector do MySQL para Python.

pip install mysql-connector-python ou py -m pip install mysql-connector-python.

3. Crie o banco de dados

No MySQL Workbench, execute:

CREATE DATABASE ouvidoria;
USE ouvidoria;

Em seguida, crie a tabela utilizada pelo sistema:

CREATE TABLE ouvidoria (
    codigo INT AUTO_INCREMENT PRIMARY KEY,
    categoria VARCHAR(50),
    titulo VARCHAR(100),
    comentario TEXT
);
4. Configure a conexão com o banco de dados

No arquivo operacoesbd.py, verifique se as informações estão corretas:

host = "127.0.0.1"
user = "root"
password = "sua_senha"
database = "ouvidoria"

5. Execute o sistema
python menu.py

Após a execução, um menu interativo será exibido no terminal, permitindo cadastrar, consultar, atualizar e excluir manifestações.

---

👨‍💻 Desenvolvido por:

Projeto acadêmico desenvolvido por alunos da Unifacisa
