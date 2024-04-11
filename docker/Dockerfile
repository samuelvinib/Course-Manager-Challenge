FROM node:latest

WORKDIR /app

COPY package.json yarn.lock ./

RUN yarn install

COPY . .

EXPOSE 3000

RUN yarn global add @nestjs/cli

CMD ["yarn","run", "start:dev"]