# Rodando uma aplicação na sua maquina

## Baixando o docker sample application

- [Baixe aqui](https://docs.docker.com/get-started/02_our_app/)
- Criar o arquivo Dockerfile
  - `FROM`: O FROM instrução inicializa um novo estágio de construção e define o Imagem base para instruções subsequentes.
  - `WORKDIR`: Diretório principal da aplicação
  - `COPY`: adiciona arquivos do diretório atual do seu cliente Docker. O COPY instrução copia novos arquivos ou diretórios de <src> e os adiciona ao sistema de arquivos do contêiner no caminho <dest>.
  - `ADD`: O ADD instrução copia novos arquivos, diretórios ou URLs de arquivos remotos de <src> e os adiciona ao sistema de arquivos da imagem no caminho <dest>.
  - `RUN`: Rode a aplicação/cria seu aplicativo. O RUN instrução executará quaisquer comandos em uma nova camada sobre imagem atual e confirme os resultados.
  - `ENV`: O ENV instrução define a variável de ambiente <key> para o valor <value>.
  - `EXPOSE`: Porta que vai rodar a aplicação. O EXPOSE instrução informa Docker que o contêiner ouve no portas de rede especificadas em tempo de execução. Você pode especificar se a porta escuta TCP ou UDP, e o padrão é TCP se o protocolo não for especificado.
  - `USER`:
  - `CMD`: especifica qual comando executar dentro do contêiner. Só pode haver um CMD instrução em um Dockerfile. Se você listar mais de um CMD então apenas o último CMD entrará em vigor.
  - `ENTRYPOINT`:
- Fazer o build `docker build -t app .`
- Executar em modo iterativo no shell `docker run -it app sh`
- Rodando a aplicação depois de todas alterações no dockerfile `docker run -dp 3000:3000 app`