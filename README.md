### Nesses dias estava estudando vps então subi o projeto em uma vm da google : [FRONT-END LIVRARIA](http://34.95.247.32:8000)
## Projeto final do modulo de docker
#### INSTRUÇÕES:
    Passos
    1. Fazer o clone desse projeto
    2. Configurar o .env 
        exemplo {
            FRONTEND_PORT=8000
            BACKEND_PORT=4444

            MYSQL_PORT=3306
            MYSQL_DATABASE=livraria
            MYSQL_ROOT_PASSWORD=pass123

            PMA_USER=root
            PMA_PASSWORD=pass123
        } Pode ser copiado para agilizar. Quando for tornar público, remover este exemplo...
    3. Acessar a pasta raiz do projeto pelo cmd, pasta onde se encontra o docker-compose.yml
    4. No terminal, rodar o comando "docker compose up"
    5. Se tudo estiver certo, o front-end do servidor estará rodando...
       

#### Rotas
- [FRONT-END LIVRARIA](http://localhost:8000)
- [INTERFACE BANCO DE DADOS](http://localhost:8080)

#### Projetos originais:
Eu removi o .git de todos os repositorios para facilitar na hora de fazer o clone deste, entao vou deixar o link aqui dos projetos originais que utilizei
- [Webacademy-livros-backend](https://github.com/jocelinnik/webacademy-livros-backend)
- [Webacademy-livros-frontend](https://github.com/jocelinnik/webacademy-livros-frontend)
- [Webacademy-livros-config](https://github.com/jocelinnik/webacademy-livros-config)


#### Obs:
    1. Tentei ao maximo não alterar os arquivos do professor. 
    2. Os logs serão sincronizados na pasta log dentro do backend.
    3. Uso do healthcheck para garantir que o banco ja estava no ar antes de iniciar os serviços que depedem dele.
    4. version do topo do arquivo foi removido por conta do docker indicar que era depreciado.
    5. Aproveitei o arquivo de criação das tabelas e o com as recomendacoes de adições para criar um init.sql, assim o banco ja sobre com algumas informações.
    6. Uso da versao antes do PrismaORM (motivo : Havia alguns problemas quanto ao retorno de erros para o front e travamento do app)
    7. versao com sequelizer no commit anterior.
    
