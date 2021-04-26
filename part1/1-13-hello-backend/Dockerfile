FROM golang:1.16-alpine3.13

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN go build

# default port is 8080
CMD ./server