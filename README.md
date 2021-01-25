# Instalação limpa do Wordpress com Docker
Projeto padrão Wordpress Versão 2

- O que há de novo? 
- Nesta versão, fiz questão de colocar no docker-compose.yml a chamada da imagem do PHP. Neste caso, você terá a liberdade de usar o Wordpress em outras versões de PHP


# Tecnologias
## PHP 7+
## MySQL Server
## PHPMYADMIN (Rodando na porta 8080 | http://localhost:8080)

## Como usar
### Acesse a raiz do projeto pelo terminal e digite os seguintes comandos:
### docker-compose build --no-cache
### docker-compose up -d

## Pronto! Seu Wordpress estará rodando na porta 80 em http://localhost:80
### Agora temos um ambiente configurado! Agora basta você instalar o Wordpress e os plugins de acordo com a sua necessidade!

## Caso dê alguma coisa errada e precise remover os contâineres
### docker-compose stop
### docker-compose down 
### Realize as alterações necessárias no arquivo docker-compose.yml e repita os comandos de como usar

# Credenciais de banco de dados e PHPMYADMIN:
###  Nome do banco MySQL: wordpress
###  Usuário do banco MySQL: wordpress
###  Senha do banco MySQL: wordpres