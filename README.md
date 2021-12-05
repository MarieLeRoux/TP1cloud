# TP1cloud

Automatisation du déploiement de golang-myip (https://github.com/BastienBalaud/golang-myip) avec Packer et Ansible sur des VM Rocky 8.

********************************

Installation d'Ansible sur Rocky 8

**toutes les commandes sont effectuées en root**

dnf update -y
reboot
dnf install -y epel-release
dnf install ansible -y

**vérification de l'installation**

ansible --version

source : https://www.linuxtechi.com/how-to-install-ansible-on-rocky-linux/
