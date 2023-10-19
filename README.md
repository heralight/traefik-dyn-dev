# Automated traefik dns resolver with SSL

A fork of [Pyru Gist](https://gist.github.com/pyrou/4f555cd55677331c742742ee6007a73a) with some mods that allow you to have local services accessible by myservice.traefik.me with let's encrypt ssl without any system modification.

[Traefik.me](https://traefik.me/) is a service like https://nip.io/ or https://xip.io/ 

Thanks to [Pyru](https://github.com/pyrou) the source code is accessible at:

https://github.com/pyrou/traefik.me
https://gist.github.com/pyrou/4f555cd55677331c742742ee6007a73a

## What ?

This project allow you to run inside your dev machine a dynamic traefik gateway that will add any services and provide a ssl certificate for any domain under traefik.me. 

You can add your services under the external network 'gtw'.

## Start the gateway

```sh
docker compose up -d
```

## Start others services

Take a look inside the sample directory.

```sh
cd samples/
docker compose up -d
```

check it at https://app1.traefik.me and https://app2.traefik.me

## Traefik Dashboard

Traefik dashboard is accessible at: https://dashboard.traefik.me/





