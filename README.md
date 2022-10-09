# devops.docker-examples.DOCKER

## docker hub

Onde existe uma diversa variedade de imagens docker [docker hub](https://hub.docker.com/)

## [Comandos](https://docs.docker.com/engine/reference/run/)

### docker run nome_container

Executa um container

### 'docker ps' ou 'docker container ls'

Retorna quais containers estão em execução.

### 'docker ps -a' ou 'docker container ls -a'

Retorna todos os containers.

### docker stop nome_imagem_ou_id

Para a execução da imagem docker

### docker start nome_imagem_ou_id

Inicia a execução da imagem docker

### docker exec -ti nome_imagem_ou_id bash

Execute um comando em um contêiner em execução.

### docker run -d -p 8080:80 docker/getting-started

o comando `-d -p 8080:80` no comando acima levanta a imagem `docker/getting-started` na porta 8080 da sua maquina.

Abra no navegador `http://localhost:8080/`

### docker unpause nome_imagem_ou_id

Iniciar um container pausado.

### 'docker images' ou 'docker images ls'

Iniciar um container pausado.

### docker inspect nome_imagem_ou_id

### docker history nome_imagem_ou_id

## imagens

É um conjunto de camadas empilhadas para formar um container.

- Quando temos a nossa imagem, ela é read only. Isso significa que não conseguimos modificar as camadas dessa imagem depois que ela foi criada.
- Se ela é bloqueada para escrita como é que o container consegue escrever informação dentro dela? Porque no fim das contas, quando criamos o container, o container nada mais é do que uma imagem com uma camada adicional de read-write, de leitura e escrita.