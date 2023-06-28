# listmonk

## Install / Setup

Create config files.

```sh
cp .env.sample .env # update accordingly
cp config.toml.example config.toml # update accordingly
```

Start the containers.

```sh
docker-compose up -d db
# wait for db to be up and ready
docker-compose run --rm app ./listmonk --install
# after installation
docker-compose up -d app db
```