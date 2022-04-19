Start a Postgres with Docker database

```bash
docker run --name ignite-challenge-database-queries -e POSTGRES_DB=queries_challenge -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
```





docker -v
docker ps                                                   => Verifica os containers que estão rodando
docker ps -a                                                => Lista Todos os containers


docker build -t [nomeDaImagemASerCriada] [caminhoDoDockerfile]    => Criar img do docker
docker build -t rentx .                                           => Exemplo

docker start [idContainer]                                  => Inicia container
docker stop [idContainer]                                   => Parar container
docker rm [idcontainer]                                     => Remover container

docker run -p 3333:3333 rentx


docker exec -t rentx /bin/bash                              => Acessa o folder do container e pode executar comandos


------------------------------------------------------



docker-compose up                           => Subir o docker, Na raiz que estiver o arquivo docker-compose.yml
docker-compose up -d                        => Sobe em background

docker-compose start                        => Inicia os containers
docker-compose stop                         => Para o docker-compose

docker-compose down                         => Remove tudo que foi criado

docker logs rentx                           => Últimos logs
docker logs rentx -f                        => Acompanhar os logs


-------------------------------------------------------

yarn typeorm migration:create -n CreateCategories

yarn typeorm migration:run

yarn typeorm migration:revert

