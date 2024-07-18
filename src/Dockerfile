# Usar a imagem oficial do Node.js como base
FROM node:18

# Criar e definir o diretório de trabalho da aplicação no container
WORKDIR /app

# Copiar os arquivos de dependências package.json e package-lock.json
COPY package*.json ./

# Instalar as dependências da aplicação
RUN npm install

# Copiar o código da aplicação para o diretório de trabalho no container
COPY . .

# Expor a porta em que a aplicação estará rodando
EXPOSE 3000

# Comando para iniciar a aplicação
CMD ["node", "server.js"]