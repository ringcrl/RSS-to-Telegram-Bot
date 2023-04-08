# 部署

```sh
# 删除已有 docker container
sudo docker container ls
sudo docker stop CONTAINER_ID
sudo docker rm  CONTAINER_ID

# 安装部署
mkdir rsstt
cd rsstt
wget https://raw.githubusercontent.com/Rongronggg9/RSS-to-Telegram-Bot/dev/docker-compose.yml.sample -O docker-compose.yml
vim docker-compose.yml  # fill in env variables
docker-compose up -d

# 更新
docker-compose down
docker-compose pull
docker-compose up -d
```
