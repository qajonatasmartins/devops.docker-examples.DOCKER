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

### docker build -t nome_projeto_no_docker .

docker build para chamar o arquivo dockerfile e fazer o build do projeto.
o -t para nomear o 'nome do projeto' e o '.' para definir que é o diretório atual. 

### docker stop $(docker container ls -q)

para todos os containers

### docker volume create meu-volume

Cria um volume no docker

### docker volume ls

lista todos os volumes

## imagens

É um conjunto de camadas empilhadas para formar um container.

- Quando temos a nossa imagem, ela é read only. Isso significa que não conseguimos modificar as camadas dessa imagem depois que ela foi criada.
- Se ela é bloqueada para escrita como é que o container consegue escrever informação dentro dela? Porque no fim das contas, quando criamos o container, o container nada mais é do que uma imagem com uma camada adicional de read-write, de leitura e escrita.


## [DOCKERFILE](https://docs.docker.com/engine/reference/builder/#usage)

### ARG 

A instrução define uma variável que os usuários podem passar em tempo de compilação para o construtor com o comando usando o sinalizador. Se um usuário especificar um argumento de compilação que não foi definido no Arquivo Docker, a compilação produz um aviso

### ENV

A instrução define a variável ambiente ao valor . Este valor estará no ambiente para todas as instruções subsequentes na fase de construção e pode ser substituído em muitas também. O valor será interpretado para outras variáveis ambientais, de modo que os caracteres de citação serão removidos se eles não forem escapados. Como a análise da linha de comando, as cotações e as barras traseiras podem ser usadas para incluir espaços dentro dos valores.

ENV MY_NAME="John Doe"
ENV PORT=6000
