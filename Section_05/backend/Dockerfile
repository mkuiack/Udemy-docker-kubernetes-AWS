FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

ARG DEFAULT_PORT=80

ENV PORT=$DEFAULT_PORT
ENV MONGODB_USERNAME=root
ENV MONGODB_password=secret

EXPOSE $PORT

COPY . .

CMD ["npm", "start"]