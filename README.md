# docker-lnmp

## Registry

```bash
# Nginx
docker pull registry.cn-qingdao.aliyuncs.com/lanseyujie/docker-lnmp-nginx:latest

# PHP
docker pull registry.cn-qingdao.aliyuncs.com/lanseyujie/docker-lnmp-php:latest

# MariaDB
docker pull registry.cn-qingdao.aliyuncs.com/lanseyujie/docker-lnmp-mariadb:latest

# Redis
docker pull registry.cn-qingdao.aliyuncs.com/lanseyujie/docker-lnmp-redis:latest
```

## Usage

```bash
# Clone
git clone https://github.com/lanseyujie/docker-lnmp.git

cd docker-lnmp

# Build & Start
docker-compose up -d

# Stop & Remove
docker-compose down

# Start
docker-compose start

# Restart
docker-compose restart

# Stop
docker-compose stop

# Logs
docker-compose logs
```

## Other

```bash
# PHP Built-in HTTP Server
docker run -it --rm -p 8080:8080 -v $(pwd):/data/ docker-lnmp-php:latest sh -c "php -S 0.0.0.0:8080 -t /data"
```
