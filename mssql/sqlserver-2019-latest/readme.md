
SQL Server 2019 Express
```
Host: localhost
Port: 1433
Username: sa
Password: qwe@1234
```

Attach
```
CREATE DATABASE db ON
  (FILENAME = '/var/opt/mssql/db.mdf'),
  (FILENAME = '/var/opt/mssql/db_Log.ldf')
FOR ATTACH;
```

Sobe container(s)
```
docker-compose up -d
```
