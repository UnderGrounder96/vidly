FROM node:14.16.0-alpine3.13

ENV NODE_ENV="development" PORT="3000"
EXPOSE ${PORT}

RUN addgroup app && adduser -SG app app
WORKDIR /app
RUN chown app /app && ls -lh /app
USER app

COPY package*.json ./
RUN npm install
COPY . .

CMD ["npm", "start"]
