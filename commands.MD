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


