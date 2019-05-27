You have 4 services:


1. rocketchat1
download image 
restart if it is stopped
map uploads folder /app/uploads to ./uploads

2.rocketchat2
download image
restart if it is stopped
map uploads folder /app/uploads to ./uploads

3.mongo
download image
restart if it is stopped
map ./data/runtime/db folders to /data/db
map /data/dump folders to /dump

4.haproxy
download image
restart if it is stopped
map ./haproxy.conf folders to /usr/local/etc/haproxy/haproxy.cfg:ro


and you have haproxy.conf file for config.


For start containers, run this command :
docker-compose up
