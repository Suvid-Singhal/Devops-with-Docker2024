FROM golang:1.16-alpine
WORKDIR /usr/src/app
EXPOSE 8080
COPY . .
RUN apk add build-base
RUN go build
RUN go test ./...
ENTRYPOINT ./server
