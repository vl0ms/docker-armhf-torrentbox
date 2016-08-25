# docker-armhf-torrentbox
Docker image with nginx + php5-fpm + rtorrent + rutorrent(web ui) started with supervisord

# usage
docker pull vl0ms/armhf-torrentbox

docker run -dt --name torrentbox -p 80:80 -p 443:443 -p 49160:49160/udp -p 49161:49161 --restart=always -v /mnt/mydata:/rtorrent -e NEW_USER=myuser -e NEW_PASS=mypass -e TZ=Europe/Moscow vl0ms/armhf-torrentbox
