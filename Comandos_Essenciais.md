## Comandos essenciais:

- pwd
```
Mostra o diretório atual
```

- cd
```
Acessar um diretório:

cd /home

cd .. : diretorio anterior

cd -  : volta para o diretório que estava anteriormente
```

- ls
```
Lista o conteúdo de um diretório

ls : lista o diretário atual

ls /home  : lista o conteúdo de /home

le -l  : lista o conteúdo com detalhes
```

- mkdir
```
Cria um diretório:

mkdir nome_do_diretorio

Obs.: é possível criar mais de um diretório ao mesmo tempo:

mkdir diretorio-1 diretorio-2 diretorio-3
```

- rmdir
```
Remove um diretório:

rmdir nome_do_diretorio

Obs.: se o diretório não estiver vazio, não deixa remover, sendo necessário passar a flag -r com o comando rm:

rm -r diretorio-1
```

- tree
```
Lista os diretórios e arquivos em forma de árvore:

tree nome_do_diretorio ou tree
```

- touch
```
Altera a data de criação de um arquivo.
obs.: se o arquivo não existir, será criado

touch nome_arquivo.txt

Obs.: é possível criar mais de um arquivo por vez:

touch arquivo-1 arquivo-2 arquivo-3
```

- rm
```
Apaga arquivos:

rm arquivo.txt
```

- mv
```
Mover e Renomear arquivos e diretórios:

mv arquivo.txt /diretorio/arquivo.txt

mv arquivo.txt novo_nome.txt
```

- cp
```
Copiar arquivos e diretórios:

cp arquivo.txt /arquivo.txt
```

- find
```
Procurar arquivos e diretórios no linux

find -name meu-arquivo : diferencia minusculas de maiusculas

find -iname meu-arquivo  : não diferencia minusculas de maiusculas

Obs.: esse comando sempre vai procurar do diretório atual para frente ou pelo diretório especificado no comando

exe:

find diretorio -name meu-arquivo
```

- clear
```
Limpar o terminal
```

- yum / dnf / apt
```
Instalar pacotes no linux

sudo apt install mysql-server
```

- service
```
Gerenciar serviços no linux
(start, stop, status)

service --status-all
```

- tail
```
Exibir as últimas linhas de um arquivo

tail arquivo

obs.: tail -f arquivo, vai ficar mostrando as últimas linhas em tempo real, ou seja, se o arquivo for escrito no momento que tiver aberto, ele vai mostrando as alterações;
```

- cat
```
Visualizar um arquivo

cat arquivo.txt
```

- vi
```
Editor de arquivos nativo;

vi arquivo.txt
```

- man
```
Exibe o manual de um comando:

man ls
```

- du
```
Mostra o tamanho da pasta

du diretorio
```

- df
```
Mostra a utilização das partições

df diretorio
```
- useradd
```
Cria um usuário
```

- passwd
```
Altera a senha de um usuário
```
- userdel
```
Remover um usuário
```

- su
```
Acessar um usuário
```
- sudo
```
Executar comandos com maior nivel de privilégio
```

- data / date
```
Comando para exibir a data e hora do sistema
```
- fdisk
```
Gerenciar disco
```

- mkfs
```
Formatar a partição
```

- mount
```
Montar uma partição
```

- umount
```
Desmontar uma partição
```

- dmesg | grep usb
```
Listar os dispositivos conectados na usb
```