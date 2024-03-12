# amd64-workstation

```bash
uname -a
```


```bash
docker pull philippecharriere494/hello-go:scratch
docker images | grep hello-go
docker run philippecharriere494/hello-go:scratch
```

```bash
docker pull philippecharriere494/hello-go:multiarch
docker images | grep hello-go
docker run philippecharriere494/hello-go:multiarch
```

docker run \
-p 8080:8080 \
-v $(pwd):/app \
--rm k33g/simplism:0.1.3 \
/simplism listen ./app/index.wasm handle --http-port 8080 --log-level info