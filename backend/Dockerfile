FROM node:14.16.0-alpine3.13

ENV NODE_ENV="development" PORT="3001"
EXPOSE ${PORT}

WORKDIR /app

COPY package*.json ./
RUN npm install
COPY . .

CMD ["npm", "start"]
