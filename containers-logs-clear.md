
Listar espaço utilizado por cada container: 
```
$ sudo du -hc --max-depth=1 /var/lib/docker/containers/
```

Limpar logs dos containers: 
```
$ sudo sh -c 'truncate -s 0 /var/lib/docker/containers/*/*-json.log'
```
