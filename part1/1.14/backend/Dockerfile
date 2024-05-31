FROM golang:1.16-alpine
WORKDIR /usr/src/app
EXPOSE 8000
COPY . .
ENV REQUEST_ORIGIN=http://localhost:5000
RUN apk add build-base
RUN go build
RUN go test ./...
ENTRYPOINT ./server
