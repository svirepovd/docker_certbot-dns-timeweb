# certbot-dns-timeweb docker

Timeweb DNS Authenticator plugin for Certbot wrapped into docker container.

## Buid the container

```sh
docker build -t certbot-dns-timeweb
```

## Issue the certificate

Get Timeweb Cloud [access token](https://timeweb.cloud/my/api-keys) and fill credentials configuration file `certbot/timeweb-creds.ini`.

Change `docker-compose.yml` for your needs.

```sh
docker compose run certbot
```

if successful you would find issued certificate and private key in `./certbot/etc/letsencrypt/live/example.com`

Regards to <https://github.com/artrey/certbot-dns-timeweb>