# zmirror-docker

1. To obtain a ssl from https://www.letsencrypt.org/ and stored it in the default folder
A good instruction is here https://github.com/vimagick/dockerfiles/tree/master/certbot
get dns ready deployed before ssl script run
2. To Run a google mirror by this docker 
for ipv6 support, consider add external domain *.1e100.net to config.py
`docker run -d --name somezmirror -p 80:80 -p 443:443 -e DOMAIN=yourdomain.example.com -v /etc/letsencrypt:/etc/letsencrypt yumin9822/zmirror

`
Please remember to change the DOMAIN setting.
