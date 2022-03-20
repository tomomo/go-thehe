FROM golang:1.18

RUN apt-get update \
  && apt-get upgrade -y \
  && apt-get autoremove \
  && apt-get autoclean \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /go/src

RUN go install golang.org/x/tools/gopls@latest
RUN go install github.com/cosmtrek/air@latest

COPY go.mod .
COPY go.sum .
RUN go mod download all
# #

# NOTE: 課題。起動も含めてしまいたいが、Webサーバーログが確認できなくなるので、ターミナルでairを実行する方法を取っている。
# CMD ["air", "-c", ".air.toml"]
