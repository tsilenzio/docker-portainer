# docker-portainer

Creates a portainer instance that will connect and automatically configure seamlessly with our Caddy container

## Setup

Create a `.env` file by cloning from `.env.example`

```
cp .env.example .env
```

Create the nessesary docker volumes

```
docker volume create portainer_data
```

If you haven't created the Caddy container yet then the following volume and network will also need to be created

```
docker volume create caddy_data
docker network create caddy_network
```
