
### docker commands
https://docs.docker.com/engine/reference/commandline/cli/


```bash
# Exibe informações do docker
docker info

# Lista todos os contêineres
docker ps -a

# Exibe estatísticas de uso de recursos nos contêineres
docker stats

# Retorna informações de baixo nível sobre objetos do Docker
docker inspect INSTANCE_ID

# Exibe o histórico de uma imagem
docker history IMAGE

# Exibir logs de um contêiner
docker logs -n20 CONTAINER_ID

# Lista espaço utilizado por contêiner
docker ps --size -a

# Exibe uso de disco do docker
docker system df -v

# Gerar uma imagem de um Dockerfile
docker build -t IMAGE .

# Executa um contêiner usando env-file
docker run -d -80:80 --env-file dockerfile.env IMAGE

# Executa um comando em um contêiner em execução
docker exec -it -d CONTAINER /bin/bash

# Remove imagens de dados não utilizadas
docker system prune -a -f

# Remove volumes de dados não utilizados
docker system prune -a --volumes

# Remove todos os contêineres parados
docker container prune -f

# Remove todos os volumes locais não utilizados
docker volume prune -f

# Remove imagens não utilizadas
docker image prune -ff
```
