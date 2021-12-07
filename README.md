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

********************************

## Utilisation de Packer

packer build <nom du fichier>
dans notre cas: packer build packer.pkr.hcl

*********************************

## Description du playbook

*********************************

## Sources :

**Modules Ansible**
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/file_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/blockinfile_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/uri_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/service_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/shell_module.html

**Création d'un service**
https://linuxconfig.org/how-to-create-systemd-service-unit-in-linux
https://www.linuxtricks.fr/wiki/systemd-les-commandes-essentielles
https://ostechnix.com/check-runlevel-linux/

**Manipulation fichier kickstart**
https://www.golinuxcloud.com/rhel-centos-8-kickstart-example-generator/

**Ajout des clés SSH**
https://linuxize.com/post/curl-command-examples/

**Installation Ansible**
https://www.linuxtechi.com/how-to-install-ansible-on-rocky-linux/
