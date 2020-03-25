# FAHclient
Dockerizing folding@home (FAH) client

### Build
Place yourself into the same directory where the `Dockerfile` is located and run:
```
$ docker build -t <user>/<repo>:<tag> .
```

### Run
```
docker run \
    --rm \
    -d \
    -p 7396:7396 \
    --name fahclient \
    <user>/<repo>:<tag> \
    --user=CarmeloC --team=0 --gpu=false --smp=true --power=light
```

### Web Control
The web control page can be displayed at `http://127.0.0.1:7369/`

