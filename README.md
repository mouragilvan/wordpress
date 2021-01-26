# Ambiente Wordpress com Docker
## Projeto padrão Wordpress Versão 2

- O que há de novo? 
- Nesta versão, fiz questão de colocar no docker-compose.yml a chamada da imagem do PHP. Neste caso, você terá a liberdade de usar o Wordpress em outras versões de PHP
- Adicionei também o arquivo de variáveis de ambiente .env para você customizar melhor seus containers. 
- As credenciais de acesso como login e senha do MySQL e do PHPMYADMIN você foram colocadas no .env e você pode alterar como quiser.
- Os nomes dos containers também podem ser alterados no .env

## Tecnologias
- PHP 7+
- MySQL Server
- PHPMYADMIN (Rodando na porta 8080 | http://localhost:8080)

## Como usar

### Passo 1
#### Acesse o arquivo .env na raiz do projeto e informe/altere as credenciais de acesso:
```
WEB_CONTAINER_NAME=nome-do-seu-container-web
DB_CONTAINER_NAME=nome-do-seu-container-db
PMA_CONTAINER_NAME=nome-do-seu-container-phpmyadmin

DB_USER=nome-do-usuario-do-banco
DB_PASS=senha-do-usuario-do-banco
DB_DATABASE=nome-do-banco-de-dados
```
### Passo 2
#### Altere as credenciais de acesso ao banco no arquivo wp-config.php de acordo com seu .env
```
// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define( 'DB_NAME', 'nome-do-banco-de-dados');

/** MySQL database username */
define( 'DB_USER', 'nome-do-usuario-do-banco');

/** MySQL database password */
define( 'DB_PASSWORD', 'senha-do-usuario-do-banco');
```

### Passo 3
#### Acesse a raiz do projeto pelo terminal e digite os seguintes comandos:

``` 
docker-compose build --no-cache
```

```
docker-compose up -d
```
### Pronto! Seu Wordpress estará rodando na porta 80 em http://localhost:80
### Agora temos um ambiente configurado! Agora basta você instalar o Wordpress e os plugins de acordo com a sua necessidade!

## Caso dê alguma coisa errada e precise remover os contâineres
- docker-compose stop
- docker-compose down 
- Realize as alterações necessárias no arquivo docker-compose.yml e repita os comandos de como usar

