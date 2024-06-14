FROM golang:1.22.1 as builder

ENV GO111MODULE=on

WORKDIR /app

COPY . .

RUN CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build .

FROM alpine:latest
COPY --from=builder /app/spot .

EXPOSE 50051

ENTRYPOINT ["/spot"]