# Instalação limpa do Wordpress com Docker
Projeto padrão Wordpress

# Tecnologias
## MySQL Server
## PHPMYADMIN (Rodando na porta 8080 | http://localhost:8080)

## Como usar
### Acesse a raiz do projeto pelo terminal e digite os seguintes comandos:
### docker-compose build --no-cache
### docker-compose up -d

## Pronto!
### Agora temos um ambiente configurado! Agora basta você instalar o Wordpress e os plugins de acordo com a sua necessidade!

## Caso dê alguma coisa errada e precise remover os contâineres
### docker-compose stop
### docker-compose down 
### Realize as alterações necessárias no arquivo docker-compose.yml e repita os comandos de como usar

# Credenciais de banco de dados e PHPMYADMIN:
###  Nome do banco MySQL: wordpress
###  Usuário do banco MySQL: wordpress
###  Senha do banco MySQL: wordpres