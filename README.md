# Docker
Docker com PHP, SQL SERVER e NGINX

# Instalação do docker
https://www.docker.com/

# Orientações gerais

[SQL Server]
1. O Arquivo Dockerfilesql indica a senha para o SA do banco
2. No arquivo docker-compose.yml é criada uma bridge para o seu IP local, desse modo o banco responde por ele na porta padrão
3. No arquivo docker-compose.yml é criado um volume que aponta para pasta /data que deve manter os arquivos do banco de dados 

[NGINX]
1. O arquvio default.conf é referente a configuração do servidor http
2. No arquivo DockerfileNginx é cedida permissão de leitura e gravação na pasta publicada para o usuário do servidor http

[PHP]
1. Algumas extensões são instaladas na docker pelo arquivo DockerfilePhp
2. As bibliotecas necessárias para o SQL Server são instaladas pelo arquivo DockerfilePhp
3. O composer é instalado pelo arquivo DockerfilePhp
