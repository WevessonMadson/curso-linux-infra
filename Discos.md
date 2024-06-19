## Gerenciamento de discos no linux

- Comandos de gerenciamento de discos e partições devem ser executados com usuário root, pois deve se ter permissões elevadas;

- Para listar os discos basta usar o ` fdisk -l `

```
Exemplo:

fdisk -l
```

##### reconhecendo discos

- Os discos são montados em ` /dev/ `
- hds e pendrives aparecem como ` sd `
- o primeiro dispositivo de armazenamento é o  `sda`
- o segundo é o `sdb`
- o terceiro é o `sdc`, e assim por diante

##### partições

- Para partições, ele usa a identificação, como acima, mais números para informar que é uma partição do hd, por exemplo:

- `sda1` é uma partição do disco `sda`


#### Gerenciando discos

- O comando `fdisk /dev/"disco"` é usado para gerenciar o disco informado ao final do comando

- com o comando acima é aberto um wizard para fazermos os comandos de gerenciamento, bastando segui-los para cada alteração que se deseja fazer


#### Formatando um novo hd

```
fdisk "caminho do hd"

# exemplo: fdisk /dev/sdb

# seguir a sequência abaixo:

p -> ver as partições
n -> nova partição
w -> salvar alterações
q -> sair do wizard do fdisk

# após sair, formatar a partição com o:
mkfs.xfs "caminho da partição"

exemplo: mkfs.xfs /dev/sdb1

# após isso, a partição pode ser montada:

mount /dev/sdb1 /mnt
```