FROM node:16-alpine

WORKDIR /app
COPY package*.json ./

RUN npm install
COPY . .

RUN npm run build

RUN npm install -g serve
CMD ["serve", "-s", "build", "-l", "3000"]
# port 3000 pour l'application React
EXPOSE 3000
