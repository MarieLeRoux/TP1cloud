# TP1cloud

Automatisation du déploiement de golang-myip (https://github.com/BastienBalaud/golang-myip) avec Packer et Ansible sur des VM Rocky 8.

********************************

## Installation d'Ansible sur Rocky 8

**toutes les commandes sont effectuées en root**

dnf update -y
reboot
dnf install -y epel-release
dnf install ansible -y

**vérification de l'installation**

ansible --version

source : https://www.linuxtechi.com/how-to-install-ansible-on-rocky-linux/

********************************

## Utilisation de Packer

packer build <nom du fichier>
dans notre cas: packer build packer.pkr.hcl

*********************************

## Description du playbook

sources :
https://linuxconfig.org/how-to-create-systemd-service-unit-in-linux
https://www.linuxtricks.fr/wiki/systemd-les-commandes-essentielles
https://ostechnix.com/check-runlevel-linux/
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/file_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html
