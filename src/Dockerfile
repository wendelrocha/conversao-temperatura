FROM node:18.16.0
WORKDIR /app
## Copiar as dependências do projeto e 
## executar o gerenciador de pacotes,
## antes de copiar todos os arquivos do projeto
## é uma boa prática.
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]