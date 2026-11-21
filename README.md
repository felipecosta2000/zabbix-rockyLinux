Rocky Linux 9.8 na instalção via pacotes com o Zabbix 8.0 LTS. Nosso ambiente está assim:

➔ Zabbix 8.0 LTS
➔ Sistema Rocky Linux 9.8


Atualize o seu sistema:

# dnf update
# dnf upgrade

Desabilite o SELinux, editando o arquivo /etc/selinux/config:

# vim /etc/selinux/config

SELINUX=disabled

Stop e desabilitar o firewall:

# systemctl stop firewalld ; systemctl disable firewalld
