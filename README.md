# yt6801_CentOS_9
## Esse driver foi editado e corrigido para compilar no CentOS Stream 9
## O ideal é que tudo seja feito com permissões root.

### Instalar os pacotes abaixo e suas dependências:

```bash
yum install kernel-devel make gcc
```

### Para descompactar:

```bash
tar -xjf yt6801.tar.bz2
```

### Entre no diretório:

```bash
cd yt6801
```

### Instale (se der erro no certificado ou no SSL não se preocupe):

```bash
./yt_nic_install.sh
```

### Verificar se o módulo já subiu:

```bash
lsmod | grep yt6801
```

### Reinicie:

```bash
reboot
```

### Configure a placa de rede (pacote NetworkManager):
```bash
nmtui
```
