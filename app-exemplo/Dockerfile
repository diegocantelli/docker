FROM node:14

# define o diretorio atual dentro do container
WORKDIR /app-node 

# copia o conteúdo do diretório em que se encontra o dockerfile e cola no diretório atual do container(app-node)
COPY . .
RUN npm install

# assim que as dependências do comando acima forem executadas, será executado o comando npmo start para subir a aplicação
ENTRYPOINT npm start