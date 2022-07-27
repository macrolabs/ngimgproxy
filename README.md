# NGIMGPROXY

Letsencrypt + NGINX + imgproxy on Docker

# HOW TO USE

- Step 1 : create `.env` file with secret key and salt (see here : https://docs.imgproxy.net/#/configuration?id=url-signature)

```
IMGPROXY_KEY=
IMGPROXY_SALT=
IMGPROXY_PATH_PREFIX=
```

- Step 2: run init-letsencrypt.sh

```
$ sudo init-letsencrypt.sh
```

This requests the initial SSL certs which will later be auto-renewed.

- Step 2 : run docker-compose up

```
$ sudo docker-compose up -d
```

