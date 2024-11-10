# yt6801_CentOS_9
Esse driver foi editado e corrigido para compilar no CentOS Stream 9
O ideal é que tudo seja feito com permissões root.

Instalar os pacotes abaixo e suas dependências:
yum install kernel-devel make gcc

Para descompactar:
tar -xjf yt6801.tar.bz2

Entre no diretório:
cd yt6801

Instale (se der erro no certificado ou no SSL não se preocupe):
./yt_nic_install.sh

Verificar se o módulo já subiu:
lsmod | grep yt6801

Reinicie:
reboot

Configure a placa de rede (pacote NetworkManager):
nmtui
