Docker Compose: pgAdmin4 e PostgreSQL
---
Este repositório contém um exemplo simples de como usar o Docker Compose para executar o pgAdmin4 e o PostgreSQL em contêineres Docker separados. Isso é útil para desenvolvimento local, testes e ambientes de demonstração.

Pré-requisitos

Certifique-se de ter o Docker e o Docker Compose instalados em seu sistema. 

Você pode encontrar instruções de instalação aqui:

Docker Installation Guide

Docker Compose Installation Guide

Uso:

Clone este repositório para o seu sistema local:

git clone https://github.com/Carloshenriquepere/aula3.git

Navegue até o diretório do projeto:

cd docker-pgadmin4-postgresql

Inicie os contêineres usando o Docker Compose:

docker-compose up -d

Acesse o pgAdmin4 no navegador da web:

URL: http://localhost:5050

Credenciais padrão:

E-mail: admin@example.com

Senha: admin

No pgAdmin4, adicione um servidor PostgreSQL:

Host: postgres

Porta: 5432

Nome do usuário: postgres

Senha: password

Agora você pode gerenciar o servidor PostgreSQL usando o pgAdmin4.

Quando terminar, você pode parar os contêineres usando:

docker-compose down

Configuração
O arquivo docker-compose.yml define os serviços de contêineres para o pgAdmin4 e o PostgreSQL, juntamente com suas configurações.
Você pode ajustar as configurações do PostgreSQL (como nome de usuário, senha, banco de dados padrão etc.) no arquivo docker-compose.yml.
Certifique-se de não usar senhas padrão em ambientes de produção.

Notas
Este é um ambiente de desenvolvimento e demonstração. Não é adequado para produção sem modificações adequadas.
Certifique-se de fazer backup dos dados importantes, especialmente se estiver usando este ambiente para desenvolvimento ou teste.
Sinta-se à vontade para adicionar mais informações ou personalizar o README conforme necessário!
