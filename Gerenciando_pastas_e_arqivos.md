## Gerenciamento de pastas e arquivos:

### Desafio 1:

- Criar uma estrutura de pastas no usuário (/home/usuario/) que tenha as seguintes pastas:

- brasil: minas-gerais, bahia, sao-paulo, rio-de-janeiro;

- dentro de cada pasta de estado, criar dois arquivos que representem cidades desses estados;

- Extra: usar o comando `tree` para listar o diretorio brasil em forma de árvore;

```
## RESPOSTA:

mkdir brasil

cd brasil

mkdir minas-gerais rio-de-janeiro sao-paulo bahia

cd minas-gerais

touch belo-horizonte.txt contagem.txt

cd ../bahia

touch porto-seguro.txt salvador.txt

cd ../rio-de-janeiro

touch niteroi.txt rio-de-janeiro.txt

cd ../sao-paulo

touch sao-paulo.txt campinas.txt

cd ../..

tree brasil
```

### Desafio 2:

- copiar arquivo belo-horizonte.txt para o diretório de arquivos temporários: /tmp;

- mover o arquivo contagem.txt para o diretório de arquivos temporários: /tmp;

- copiar o arquivo de contagem.txt, que está em /tmp para o diretório de minas-gerais;

- renomear o arquivo contagem.txt, em minas-gerais, para nova-lima.txt;

```
# RESPOSTAS:

cd brasil/minas-gerais

cp belo-horizonte.txt /tmp

mv contagem.txt /tmp

cp /tmp/contagem.txt /home/pdv/brasil/minas-gerais

mv contagem.txt nova-lima.txt
```

### Desafio 3:

- procure o arquivo salvador.txt pelo nome completo;

- procure o arquivo salvador.txt por parte do nome, exemplo: salvad;

```
find -name salvador.txt

sudo find -iname f "salvad*"
```

### Desafio 4:

- Excluir arquivo niteroi.txt do diretório rio-de-jeneiro;

```
cd /home/pdv/basil/rio-de-janeiro

rm niteroi.txt
```