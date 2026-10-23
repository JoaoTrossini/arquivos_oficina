Sistema de Gestão de Oficina Mecânica
1. Sobre o projeto
O Sistema de Gestão de Oficina Mecânica é uma aplicação web desenvolvida em Python, com o objetivo de facilitar a organização e o gerenciamento das atividades de uma oficina mecânica. O sistema permite administrar clientes, veículos e agendamentos de serviços, utilizando um banco de dados MySQL para armazenar as informações.
2. Funcionalidades
- Autenticação: permite que os usuários acessem o sistema por meio de login e senha.
- Gerenciamento de clientes: permite cadastrar, listar, editar e excluir clientes.
- Gerenciamento de veículos: permite cadastrar veículos, vinculá-los aos seus proprietários, consultar informações, editar registros e excluir veículos.
- Agendamentos: permite cadastrar, consultar, editar e excluir agendamentos de serviços.
- Serviços: permite consultar os serviços disponíveis para os agendamentos.
- Validação de dados: verifica as informações fornecidas para evitar cadastros inválidos.
- Banco de dados: armazena as informações de clientes, veículos, usuários, serviços e agendamentos.
3. Tecnologias utilizadas
- Python
- Flask
- MySQL
- HTML
- CSS
- JavaScript
- Biblioteca mysql-connector-python
- Biblioteca bcrypt
4. Estrutura do projeto
O projeto está organizado nos seguintes arquivos e pastas:
- app.py: responsável por iniciar a aplicação.
- rotas.py: define as rotas e os endpoints do sistema.
- autenticacao.py: responsável pelo processo de autenticação dos usuários.
- clientes.py: contém as funções relacionadas ao gerenciamento de clientes.
- veiculos.py: contém as funções relacionadas ao gerenciamento de veículos.
- agendamento.py: contém as funções relacionadas aos agendamentos.
- db.py: responsável pela conexão e pelas operações com o banco de dados.
- requirements.txt: lista as dependências necessárias para executar o projeto.
- saep_db.sql: contém o script SQL para criação e configuração inicial do banco de dados.
- testar_conexao.py: permite verificar se a conexão com o banco de dados está funcionando.
- templates/: armazena os arquivos HTML das páginas do sistema.
- static/: armazena os arquivos CSS e JavaScript utilizados na interface.
5. Instalação e configuração
Para executar o sistema, é necessário ter o Python e o MySQL instalados no computador.

Passo 1 — Instalar as dependências

Abra o terminal na pasta do projeto e execute:
python -m pip install -r requirements.txt


Passo 2 — Configurar o banco de dados

Abra o MySQL Workbench ou outra ferramenta de gerenciamento do MySQL e execute o script saep_db.sql para criar e configurar as tabelas necessárias.

Passo 3 — Verificar a conexão

Execute o arquivo de teste:
python testar_conexao.py


Se a conexão estiver funcionando, o programa deverá informar que o banco de dados foi conectado corretamente.

Passo 4 — Iniciar o sistema

Execute o seguinte comando no terminal:
python app.py


Depois, abra o navegador e acesse:

http://127.0.0.1:5000
6. Banco de dados
O sistema utiliza o MySQL para armazenar e organizar as informações. Entre as principais tabelas estão:
- usuarios: armazena os dados dos usuários que acessam o sistema.
- clientes: armazena os dados dos clientes da oficina.
- veiculos: registra os veículos cadastrados e seus respectivos proprietários.
- servicos: armazena os serviços disponíveis.
- agendamentos: registra os agendamentos realizados, relacionando veículos e serviços.
O relacionamento entre as tabelas permite manter as informações organizadas e garantir a integridade dos dados.
7. Segurança
O sistema possui recursos voltados à segurança, como autenticação de usuários, validação de dados e consultas parametrizadas ao banco de dados. A biblioteca bcrypt é utilizada para verificar senhas armazenadas em formato de hash.

Em uma implantação real, também é necessário configurar adequadamente as credenciais do banco de dados, a chave secreta da aplicação e desativar o modo de depuração.
8. Objetivo do trabalho
O objetivo deste projeto é desenvolver uma aplicação que facilite o gerenciamento de uma oficina mecânica, reduzindo a necessidade de controles manuais e tornando o acesso às informações mais organizado e eficiente.

Além disso, o trabalho permite aplicar conhecimentos de programação em Python, desenvolvimento web, integração com banco de dados, autenticação e operações CRUD (criar, consultar, atualizar e excluir registros).
9. Considerações finais
O desenvolvimento do Sistema de Gestão de Oficina Mecânica proporciona uma solução para organizar as principais atividades administrativas de uma oficina. A integração entre Python, Flask e MySQL permite gerenciar informações de maneira estruturada, facilitando o controle de clientes, veículos e agendamentos.

O projeto também serve como oportunidade para aplicar, na prática, conceitos de desenvolvimento de software, banco de dados e segurança da informação.
