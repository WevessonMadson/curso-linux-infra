## Visualizando logs:

- Os logs são criados dentro do diretório:  ` /var/log `

- Como exemplo, vamos ver os logs do serviço do nginx:

```
cd /var/log

ls

cd nginx

cat access.log : vai mostrar todo o arquivo

tail -f access.log : vai mostrar o final do arquivo, e o -f vai ficar atualizando caso o arquivo sofra  modificações
```

- Como fazer um filtro para visualizar palavras chave, como ` erro `

```
cat arquivo | grep palavra

Exemplo:

cat error.log | grep sock

obs.: caso ele não encontre a palavra no arquivo, não mostrará nada do arquivo.
```

- O comando anterior pode ser usado de forma generica, para procurar tanto o arquivo como a palavra:

```
grep palavra *

Exemplo:

grep sock *

obs.: ele vai procurar todos os arquivos, dentro do diretório atual, que contenha a palavra sock.
```