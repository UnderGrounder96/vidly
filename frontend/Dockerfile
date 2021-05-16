FROM node:14.16.0-alpine3.13

ENV NODE_ENV="development" PORT="3000"
EXPOSE ${PORT}

WORKDIR /app
# RUN addgroup app && adduser -SG app app
# USER app

COPY package*.json ./
RUN npm install
COPY . .

CMD ["npm", "start"]
