# OpenSUSE
## Configuration d'OpenSUSE sur mon PC Lenovo Ideadpad 330-15ARR

### 1. À faire dès la distribution installée
#### a) Ajouter les dépôts communautaires packman & mettre packman comme dépôt principal
##### Première ligne de commande : 
* sudo zypper ar -cfp 90 https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/ packman
##### Seconde ligne de commande : 
* sudo zypper dup --from packman --allow-vendor-change

#### b) Installation driver ethernet (packman doit être installé avant)
* sudo zypper in r8168-kmp-default
* sudo zypper in r8168-blacklist-r8169
