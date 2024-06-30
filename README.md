# **Aplicação CLI em Go (Golang)**

<br>
<br>

## Olá pessoal,

- Quero compartilhar com vocês uma aplicação CLI incrível desenvolvida como tema do trabalho da matéria de Redes de Computadores em Go (Golang). Esta aplicação é capaz de coletar o endereço IP ou o servidor de um site inserido, dependendo da flag utilizada na execução.

- O Go é uma linguagem de programação de código aberto que se tornou muito popular nos últimos anos devido à sua eficiência e simplicidade. Com ele, é possível criar aplicações poderosas e robustas, capazes de lidar com tarefas complexas e de alto desempenho.

- A aplicação CLI em Go utiliza a biblioteca "net" para coletar informações sobre o site inserido. Através da flag "ip", a aplicação retorna o endereço IP correspondente ao site informado. Já com a flag "servers", a aplicação retorna o servidor utilizado pelo site.

- O processo é muito simples e fácil de executar. Basta baixar o código-fonte da aplicação, compilar e executar com a flag desejada. Com apenas alguns comandos no terminal, é possível obter informações valiosas sobre qualquer site.

- Um abraço a todos!

<br>

## Exemplo de funcionamento
```bash
./linha-de-comando ip --host stackoverflow.com
151.101.193.69
151.101.1.69
151.101.65.69
151.101.129.69
```




```bash
./linha-de-comando servers --host stackoverflow.com
ns-358.awsdns-44.com.
ns-cloud-e1.googledomains.com.
ns-1033.awsdns-01.org.
ns-cloud-e2.googledomains.com.
```
