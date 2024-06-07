## Diretórios

- /lib
- /media
```
Um pendrive, por exemplo, vai ser montado aqui
```
- /proc
```
Informações de hardware da máquina
```
- /srv
- /usr
- /var
```
var é um dos mais utilizados:

diretório de arquivos variáveis/dinâmicos;

arquivos de logs, por exemplo ficam aqui, pois são arquivos dinâmicos, que cresce com o tempo.
```
- /tmp
```
tmp é um dos mais utilizados:

diretório de arquivos temporários;

costumamos utilizar para arquivos temporários, que queremos manter até mover para um local específico ou excluir;
```
- /mnt
```
Muito utilizado, pois podemos montar as mídias externas nele;
```
- /opt
```
Muito utilizado para softwares complementares;

Geralmente são instalados em /opt, softwares que não são nativos
```
- /etc
```
Principal pasta do linux;

Todos os arqruivos de configuração, inclusive de softwares instalados, fica dentro do diretório /etc
```
- /bin
```
Diretório onde ficam os binários do linux, assim com o /sbin;

Obs.: Todo comando excutado no linux é um binário, então fica dentro de /bin ou de /sbin

Obs. 2: A diferença entre elas é que comandos que qualquer um possa utilizar fica dentro do /bin e comandos que só pode ser executado  com privilégio, fica dentro de /sbin

Exemplo:
pwd -> dentro de /bin

apt -> dentro de /sbin
```
- /sbin : comandos, ver acima
- /boot
```
Arquivos de configuração de boot
```
- /dev
```
Os dispositivos ficam neste diretório, ou seja, colocou um pendrive no pc, ele vai para /dev

assim como hd, etc
```
- /home
```
Diretório dos usuários;
```
- /root
```
Diretório "home" do usuário root, que fica nesse diretório específico
```