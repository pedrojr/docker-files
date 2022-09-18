
Conectar no mysql: 
```
mysql -u root -p
```

Selecionar o banco: 
```
USE mysql;
```

Configurar native password: 
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```

---

Remover validate password: 
```
uninstall plugin validate_password;
alter user 'root'@'localhost' identified by 'root';
flush privileges;
```

---

Alterar senha: 
```
SET GLOBAL validate_password_policy=LOW;
use mysql;
update user set authentication_string=password('password') where user='root';
flush privileges;
```
