# Traefik with letsencrypt in docker compose    

Example docker-compose project to run traefik + whoami with ssl certificate easily.


## Edit docker-compose
To run this demo you need to edit cloudflare credentinials and domain name.

```diff
- - "--certificatesresolvers.letsencrypt.acme.email=EMAIL@DOMAIN.com"
+ - "--certificatesresolvers.letsencrypt.acme.email=yusufkaan142@gmail.com"
```

```diff
- - CLOUDFLARE_EMAIL=EMAIL@DOMAIN.com
+ - CLOUDFLARE_DNS_API_TOKEN=yusufkaan142@gmail.com
```

```diff
- - CLOUDFLARE_DNS_API_TOKEN=XXXXXXXXXXX
+ - CLOUDFLARE_DNS_API_TOKEN=Ey78-j123mmdqioqwedqwe54
```
## Run
```
docker-compose up
```

## Urls

After editing and run docker-compose you can check urls

- traefik.DOMAIN.com
- whoami.DOMAIN.com

## Traefik admin panel
Traefik has basic auth middleware, so you need to enter this user password.

| Username | Password |
|----------|----------|
| user     | password |
