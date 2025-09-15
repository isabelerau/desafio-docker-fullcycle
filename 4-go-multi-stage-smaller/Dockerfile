FROM golang:1.21-alpine AS builder

WORKDIR /app

COPY . .

RUN go build -ldflags="-s -w" -o /app/main ./main.go

CMD ["/app/main"]

FROM scratch
WORKDIR /app
COPY --from=builder /app/main .
EXPOSE 8080
CMD ["/app/main"]
