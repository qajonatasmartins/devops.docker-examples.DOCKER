FROM node:18-alpine
WORKDIR /app

# RUN addgroup dev && adduser -S -G jonatas
# USER jonatas

# fazer um copy para otimizar a geração do build.
# copio primeiro o package.json e se houver uma alteração das dependencias, ai sim eu instalo novamente todos os itens.
# Se não eu uso o chache feito pelo docker
COPY package.json .
RUN yarn install --production
# Comando que roda depois da aplicação ser criada
CMD ["node", "src/index.js"]

# Copiando todos os arquivos para o diretorio principal definido no workdir
COPY . . 

# Porta que sera exposta a aplicação
EXPOSE 3000