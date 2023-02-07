FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=max
ENV MONGODB_PASSWORD=secret1234
ENV MONGODB_URL=mongodb
ENV MONGODB_DATABASE=goals_dev

CMD ["npm", "start"]