FROM node:15.14.0-alpine3.10

EXPOSE 5000

WORKDIR /usr/src/app

COPY . .

RUN npm install && npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]
