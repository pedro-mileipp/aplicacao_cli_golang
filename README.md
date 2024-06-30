
# Aplicação de Linha de Comando em Go (Golang)

## Descrição

Esta é uma aplicação CLI (Command Line Interface) desenvolvida em Go (Golang) que permite buscar endereços IP e nomes de servidores (NS) de um domínio especificado. Utiliza a biblioteca `net` para realizar essas buscas de forma eficiente.

## Funcionalidades

- **Buscar endereços IP**: Através do comando `ip`, a aplicação retorna os endereços IP associados a um domínio.
- **Buscar servidores de nomes**: Através do comando `servers`, a aplicação retorna os servidores de nomes (NS) associados a um domínio.

## Estrutura do Projeto

```
golang-cli-application/
├── main.go
├── app/
│   └── app.go
├── README.md
└── linha-de-comando.exe
```

- `main.go`: Arquivo principal que inicializa e executa a aplicação.
- `app/app.go`: Contém a lógica da aplicação e os comandos CLI.
- `linha-de-comando.exe`: Executável pré-compilado disponível para uso imediato.

## Instalação

### Pré-requisitos

- [Go](https://golang.org/dl/) instalado no seu sistema.

### Passos

1. Clone o repositório:

    ```sh
    git clone https://github.com/pedro-mileipp/golang-cli-application.git
    cd golang-cli-application
    ```

2. Compile o código:

    ```sh
    go build -o linha-de-comando
    ```

3. Execute a aplicação com a flag desejada:

    ```sh
    ./linha-de-comando ip --host <NOME_DO_SITE>
    ./linha-de-comando servers --host <NOME_DO_SITE>
    ```

## Uso do Executável Pré-Compilado

Caso você não queira compilar o código, pode usar o executável pré-compilado disponível no repositório.

### Passos

1. Baixe o executável:

    ```sh
    curl -O https://github.com/pedro-mileipp/golang-cli-application/raw/main/linha-de-comando.exe
    ```

2. Execute o executável com a flag desejada:

    ```sh
    ./linha-de-comando.exe ip --host <NOME_DO_SITE>
    ./linha-de-comando.exe servers --host <NOME_DO_SITE>
    ```

## Exemplos de Uso

- Buscar IPs do domínio `stackoverflow.com`:

    ```sh
    ./linha-de-comando ip --host stackoverflow.com
    ```

    Saída:

    ```
    151.101.193.69
    151.101.1.69
    151.101.65.69
    151.101.129.69
    ```

- Buscar servidores de nomes do domínio `stackoverflow.com`:

    ```sh
    ./linha-de-comando servers --host stackoverflow.com
    ```

    Saída:

    ```
    ns-358.awsdns-44.com.
    ns-cloud-e1.googledomains.com.
    ns-1033.awsdns-01.org.
    ns-cloud-e2.googledomains.com.
    ```
    

Esta documentação fornece uma visão detalhada do projeto, incluindo como ele funciona, como utilizá-lo e exemplos de sua execução.
