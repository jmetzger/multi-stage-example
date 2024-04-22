# Multi Stage Docker build example
`Dockerfile` contains various stages which are tagged by a name using `as`.

## Commands used

```
# build bis zum target / dort davor stoppen 
docker build . -t multi-stage-example:v1 --target=builder
# alles bauen  
docker build . -t multi-stage-example:v1
docker run -p 8080 multi-stage-example:v1 -p 8080:8080
```

## Reference:

  * https://docs.docker.com/build/building/multi-stage/
