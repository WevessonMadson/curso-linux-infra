## Usuários do linux

- Todos os usuários do linux ficam gravados no arquivo: ` /etc/passwd `

```
cat /etc/passwd
```

- Obs.: alguns serviços, quando instalados, criam usam usuários

#### Criando usuários

- Para criar usuário, usamos o comando ` useradd `

- Obs.: o usuário precisa ter permissão para criar outro usuário

```
Exemplo de criação de um usuário chamado "teste"

useradd teste
```

- Obs.: ao criar um usuário, ele é criado sem senha

#### Criando senha para usuário

- Para adicionar uma senha para o usuário, entrar no usuário e executar o comando ` passwd "usuario" `

```
Exemplo para adicionar a senha para o usuário "teste":

# entrar no usuário:

su teste

passwd teste

# basta informar e repetir a senha
```

#### Alterando o bash do usuário

- Um novo usuário criado pode usar o terminal com um bash diferente, e para mudar o bash, podemos editar a linha do usuário no arquivo de usuários:

```
Exemplo:

vi /etc/passwd

# basta alterar a parte do bash na linha do usuário e pronto
```

#### Verificando usuário que está logado no terminal

- Para saber qual usuário você está usando no terminal, basta executar o comando ` whoami `

```
Exemplo:

whoami

# ele retorna o nome do usuário que está logado no terminal no momento
```

#### Mudando de usuário

- Para entrar em outro usuário, basta usar o comando ` su `

```
Exemplos:

su teste  # vai para o usuário "teste"

sudo su   # vai para o usuário root
```

