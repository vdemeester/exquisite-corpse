# Exquisite Corpse - Docker edition

See https://en.wikipedia.org/wiki/Exquisite_corpse

## Setup

```
docker-compose build
```

## Start

```
docker stack deploy --compose-file docker-compose.yml demo
```

Open a browser on `http://localhost`. Refresh. It should always be the same random sentence.

## Scale the backend

```
docker service scale exquisite-corpse_back=20
```

Open a browser on `http://localhost`. Refresh. It should be a new random sentence each time.
