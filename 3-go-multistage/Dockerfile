FROM golang:1.21-alpine AS builder

WORKDIR /app

COPY . .

RUN go build -o /app/main ./main.go

EXPOSE 8080

CMD ["/app/main"]


FROM scratch
WORKDIR /app
COPY --from=builder /app/main .
EXPOSE 8080
CMD ["/app/main"]
