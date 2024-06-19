## Criação de scripts no linux

- Script linux nada mais é que umaa sequência de comandos, que será executado um após o outro quando o arquivo .sh for executado

- Como boa prática, é sempre bom iniciar um script com o seguinte comentário:
```
#!/bin/bash
```

- Como exemplo, vamos criar um script que baixe o pacote vim:

```
cd ~

editor de texto "nome_do_script"

gedit instala-vim.sh

conteúdo:
#!/bin/bash

apt update

apt install vim

# salva o arquivo

# depois dar permissão de executar ele

sudo chmod -X ou 111 ou 777 instala-vim.sh

# para rodar:

./instala-vim.sh
```

#### Usando variáveis

- Há ainda como automatizar o script deixando o nome do pacote, por exemplo como uma vaariável, que o usuário pode escolher o que quer baixar:

- obs.: para usar variável, usamos o $nome_da_variável

```
cd ~

vim instala-pacote.sh

#!/bin/bash

apt update

apt install $1
```

- Dessa forma acima, o valor da variável será passado no momento de executar o script:

```
./instala-pacote.sh nginx
```

#### usando echo para mostrar mensagens

```
vim instala-pacote.sh

#!/bin/bash

echo "instalando pacote $1"

apt update

apt install $1
```

```
./instala-pacote.sh nginx
```

- Ao chamar o script acima, ele vai mostrar o nome que foi passado para a variável no momento de chamar o script

#### melhorando o script anterior para pedir o valor da variável durante a execução

```
vim instala-pacote.sh

#!/bin/bash

echo "Informe o nome do pacote"

read nome_pacote

echo "instalando pacote $nome_pacote"

apt update

apt install $nome_pacote
```

- para melhorar ainda mais, podemos usar o `read` sem precisar do echo para pedir a informação, bastando passar a flag `-p` e uma mensagem:

```
vim instala-pacote.sh

#!/bin/bash

read -p "Informe o nome do pacote" nome_pacote

echo "instalando pacote $nome_pacote"

apt update

apt install $nome_pacote
```