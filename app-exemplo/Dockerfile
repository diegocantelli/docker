FROM node:14

# define o diretorio atual dentro do container
WORKDIR /app-node 

# A instrução ARG carrega variáveis apenas no momento de build da imagem,
ARG PORT_BUILD=6000

# a instrução ENV carrega variáveis que serão utilizadas no container.
ENV PORT=$PORT_BUILD

# expoem a porta do container na qual o app ira rodar
EXPOSE $PORT_BUILD

# copia o conteúdo do diretório em que se encontra o dockerfile e cola no diretório atual do container(app-node)
COPY . .
RUN npm install

# assim que as dependências do comando acima forem executadas, será executado o comando npmo start para subir a aplicação
ENTRYPOINT npm start