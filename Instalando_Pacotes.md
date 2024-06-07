## Instalação de pacotes:

- Primeiro devemos atualizar o repositório: ` sudo apt update `

- Depois instalar o pacote que queremos: ` sudo apt install pacote `

```
Exemplo:

sudo apt update

sudo apt install nginx
```

## Gerenciando serviços:

- Podemos usar o comando ` service "serviço" status ` para saber se ele está rodando;

```
Exemplo:

service nginx status
```

- Listando todos os serviços:

```
service --status-all
```

- Parando um serviço: ` service "serviço" stop `

```
service mysql stop
```

- Iniciando um serviço: ` service "serviço" start `

```
service mysql start
```

- Reiniciando um serviço: ` service "serviço" restart `

```
service mysql restart
```