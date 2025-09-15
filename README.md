# desafio-docker-fullcycle
> 📌 **Desafio 1 (Módulo Docker):** Criar uma imagem Docker em Go que tenha no máximo **2MB** de tamanho.
Aplicação Go que expõe um servidor web simples e imprime uma mensagem no console. O projeto usa Docker para compilar o binário da aplicação e empacotá-lo em uma imagem Docker otimizada com multi-stage build, resultando em um contêiner leve e eficiente. Ideal para demonstrações de Go e Docker.

# 🚀 1 — Go Initial

Nessa parte criei meu primeiro código em Go e compilei ele em binário.  

## 📥 Instalação do Go
- Acessei o site oficial: [https://go.dev/](https://go.dev/)  
- Consultei a documentação e instalei o Go no meu computador.  

## 👨‍💻 Primeiro código
- Segui o exemplo de **Hello World** da documentação.
- Criei o arquivo `main.go` com a frase do desafio (e algumas alterações).
- Em ambos os casos, ao executar a aplicação, é possível acessá-la pelo navegador, através do endereço: [https://localhost:8080](https://localhost:8080)

## ▶️ Executando o código
Rodei o comando abaixo para executar diretamente o `main.go`:

```bash
go run main.go
```

## ▶️ Compilando o código
Rodei o comando abaixo para compilar o `main.go`:

```bash
go build main.go
```

## ▶️ Executando o binário
Rodei o comando abaixo para executar o binário construído:

```bash
./main
```



# 🚀 2 — Go

Nessa segunda parte usarei o docker, portanto não é necessária a instalação do go na máquina física.  

## 👨‍💻 Estrutura
- Aproveitei o main.go que já havia criado anteriormente.
- Criei o arquivo `Dockerfile`, usando a imagem mais leve que encontrei, alpine.
- Nesse exemplo, ao executar o container, a aplicação pode ser acessada no navegador em: [http://localhost:8080](http://localhost:8080)

## ▶️ Buildando e executando a imagem
Na raiz do diretório 2-go, rodei os seguintes comandos:

```bash
docker build -t 2-go .
docker run -p 8080:8080 2-go
```
