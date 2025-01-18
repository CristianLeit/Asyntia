# Usando a imagem oficial do Node.js para React
FROM node:16-alpine

# Diretório de trabalho dentro do container
WORKDIR /app

# Copiar arquivos do package.json e instalar dependências
COPY package*.json ./
RUN npm install

# Copiar o código para o container
COPY . .

# Build do frontend para produção
RUN npm run build

# Expor a porta usada pelo frontend
EXPOSE 3000

# Comando para rodar a aplicação
CMD ["npm", "start"]
