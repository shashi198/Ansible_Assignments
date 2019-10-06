# Hadoop-Install

## Before Install
Use DNS Server or update /etc/hosts for all servers

### Install Hadoop Master 

```
Run Below Shell Command: 

```
ansible-playbook -i hosts/host master.yml
```

### Install Workers

```
Run Below Shell Command: 

```
master_ip:  your hadoop master ip
master_hostname: your hadoop master hostname

above two variables must be same like your real hadoop master

ansible-playbook -i hosts/host workers.yml -e "master_ip=172.31.0.127 master_hostname=hadoop-master"

```
