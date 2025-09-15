FROM golang:1.21-alpine

WORKDIR /app

COPY . .

RUN go build -o /app/main ./main.go

EXPOSE 8080

CMD ["/app/main"]