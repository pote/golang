FROM golang:1.3.3

RUN mkdir -p /go/src/app/.godeps
ENV GOPATH /go/src/app/.godeps:/go/src/app
WORKDIR /go/src/app

ONBUILD COPY . /go/src/app
ONBUILD RUN gpm install
ONBUILD RUN go build
