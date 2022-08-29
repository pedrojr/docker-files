
Create or edit daemon.json file

Linux: 
```
/etc/docker/daemon.json
```

Windows: 
```
$Env:USERPROFILE\.docker\daemon.json
```

Add content to file (pay attention to commas):
```
	"log-driver": "json-file",
	"log-opts": {
		"max-size": "5m",
		"max-file": "3"
	}
```
