FROM amd64/node:16-alpine

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret
ENV MONGODB_URL=mongodb
ENV MONGODB_NAME=goals

CMD ["npm", "start"]