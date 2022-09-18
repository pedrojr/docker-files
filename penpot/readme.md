
Start Penpot
```
docker compose -p penpot -f docker-compose.yml up -d
```

Url
```
http://localhost:9001
```

---

SMTP
```
docker exec -ti penpot-penpot-backend-1 ./manage.sh create-profile
```

Update Penpot
```
docker-compose -f docker-compose.yml pull
```
