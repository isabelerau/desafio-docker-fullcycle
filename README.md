# desafio-docker-fullcycle
Aplicação Go que expõe um servidor web simples e imprime uma mensagem no console. O projeto usa Docker para compilar o binário da aplicação e empacotá-lo em uma imagem Docker otimizada com multi-stage build, resultando em um contêiner leve e eficiente. Ideal para demonstrações de Go e Docker.

# 🚀 1 — Go Initial

Nessa parte criei meu primeiro código em Go e compilei ele em binário.  

## 📥 Instalação do Go
- Acessei o site oficial: [https://go.dev/](https://go.dev/)  
- Consultei a documentação e instalei o Go no meu computador.  

## 👨‍💻 Primeiro código
- Segui o exemplo de **Hello World** da documentação.
- Criei o arquivo `main.go` com a frase do desafio (e algumas alterações).  

## ▶️ Executando o código
Rodei o comando abaixo para executar diretamente o `main.go`:

```bash
go run main.go

## ▶️ Compilando o código
Rodei o comando abaixo para compilar o `main.go`:

```bash
go build main.go

## ▶️ Executando
Rodei o comando abaixo para executar o binário construído:

```bash
./main