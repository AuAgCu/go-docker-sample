FROM golang:1.19.0-alpine3.16

# ENV GOPATH=

RUN apk update \
    && apk add git \
    && apk add curl \
    && go install github.com/cosmtrek/air@latest \
    && go get github.com/dgrijalva/jwt-go
    
WORKDIR /go

EXPOSE ${BACKEND_PORT}