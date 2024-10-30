# Run mongo in replica in docker compose

It is convenient to launch it to check and work with replicas on the local machine

## Install

need install docker and docker compose

## Config key

```
echo "yourSecretKey" > mongo-keyfile
chmod 600 mongo-keyfile
```

## Run

```
docker compose up -d
```

check replica

```
docker exec -it mongo1 mongo
rs.status()
```
