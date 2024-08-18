to run the web listed hosts in 01-ping.yaml and inventory.yaml command
```
ansible -i inventory.yaml --web-hosts
```
to run the all listed hosts in 01-ping.yaml and inventory.yaml command
```
ansible -i inventory.yaml --all-hosts
```

to run the unlisted hosts in 01-ping.yaml and inventory.yaml command

```
ansible -i inventory.yaml --unlisted-hosts
```

to run the playbook in 01-ping.yaml and inventory.yaml command

```
ansible-playbook -i inventory.yaml -e ansible_username=ec2-user -e ansible_password=DevOps321 01-ping.yaml
```



For 03 multiplaybook commands

install ansible by these command
```
sudo dnf install ansible -y
```

run multiplay by using this command
```
ansible_playbook -i inventory.ini -e ansible_username=ec2-user -e ansible_password=DevOps321 03-multiplay.yaml
```

14-filter

if user doesnt difine the any varible then you can give in deafault value in the filter inself

 name: default value
  hosts: localhost
  tasks:
  - name: print default value
    ansible.builtin.debug:
      msg: "Hello {{course | default('Ansible') }}"


ansible is defined value 

