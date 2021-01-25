<h1>Instalação limpa do Wordpress com Docker</h1>
<h2>Projeto padrão Wordpress Versão 2</h2>

- O que há de novo? 
- Nesta versão, fiz questão de colocar no docker-compose.yml a chamada da imagem do PHP. Neste caso, você terá a liberdade de usar o Wordpress em outras versões de PHP
- Adicionei também o arquivo de variáveis de ambiente .env para você customizar melhor seus containers. 
- As credenciais de acesso como login e senha do MySQL e do PHPMYADMIN você foram colocadas no .env e você pode alterar como quiser.
- Os nomes dos containers também podem ser alterados no .env
<hr>
<h2>Tecnologias</h2>
- PHP 7+
- MySQL Server
- PHPMYADMIN (Rodando na porta 8080 | http://localhost:8080)
<hr>
<h2>Como usar</h2>
- Acesse a raiz do projeto pelo terminal e digite os seguintes comandos:
- docker-compose build --no-cache
- docker-compose up -d
<hr>
<h3> Pronto! Seu Wordpress estará rodando na porta 80 em http://localhost:80</h3>
<h3>Agora temos um ambiente configurado! Agora basta você instalar o Wordpress e os plugins de acordo com a sua necessidade!</h3>
<hr>
<h2>Caso dê alguma coisa errada e precise remover os contâineres</h2>
- docker-compose stop
- docker-compose down 
- Realize as alterações necessárias no arquivo docker-compose.yml e repita os comandos de como usar

