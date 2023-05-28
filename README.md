
# Adicionar Snapper mais suporte impressora de rede

yay -S gvfs-smb a2ps bc bluez-cups colord-sane cups cups-filters cups-pdf foomatic-db foomatic-db-engine foomatic-db-gutenprint-ppds foomatic-db-nonfree foomatic-db-nonfree-ppds foomatic-db-ppds gutenprint ipp-usb libieee1284 liburing net-snmp paper perl-alien-build perl-alien-libxml2 perl-capture-tiny perl-dbi perl-ffi-checklib perl-file-chdir perl-file-which perl-ipc-run perl-parse-yapp perl-path-tiny perl-xml-libxml perl-xml-namespacesupport perl-xml-sax perl-xml-sax-base psutils python-pysmbc qpdf samba sane sane-airscan splix printer-support samba-support scanner-support simple-scan hunspell-pt-br man-pages-pt_br neofetch shotwell stacer snapper snapper-support snapper-tools snap-pac btrfs-assistant btrfs-progs btrfsmaintenance grub-btrfs os-prober-btrfs grub-customizer clementine vlc gimp libreoffice-fresh libreoffice-fresh-pt-br ttf-ms-fonts


# sudo nano ~/.bashrc

cmatrix neofetch

# Reflector

The last step is to enable the reflector timer to run this once a week:

sudo systemctl enable --now reflector.timer

check if it is running:

systemctl status reflector.timer

EndeavourOS mirrors can now be ranked with a terminal command (note: call without sudo!)

eos-rankmirrors

# sudo nano /etc/pacman.conf
ILoveCandy

# Como instalar o yay no Arch Linux
O pacote yay está disponível apenas no Arch User Repository. 
Observe que você pode instalar manualmente os pacotes do AUR sem usar um auxiliar AUR (semelhante a como instalaremos yay abaixo), mas como o nome sugere, um “auxiliar AUR” ajuda você no processo de instalação, tornando mais fácil para você. você instale pacotes com o mínimo de interação do usuário.

Para instalar o yay em seu desktop Arch, primeiro baixe as seguintes dependências:

sudo pacman -S --needed base-devel git

Em seguida, clone o repositório yay usando o comando git clone:

git clone https://aur.archlinux.org/yay.git

Altere seu diretório de trabalho atual para aquele que você acabou de baixarVivapasta usando o comando cd:

cd yay

Finalmente, use o comando makepkg para compilar e instalar yay:

makepkg -si

Se o comando acima lançar o erro “cannot find fakeroot binary”, verifique se você instalou corretamente odesenvolvimento básicopacote e, em seguida, execute o comando novamente.

Além do Arch Linux, esse método também funciona para outras distribuições baseadas no Arch, incluindo Manjaro, EndeavourOS e Garuda Linux.
