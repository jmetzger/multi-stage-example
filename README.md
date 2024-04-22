# Multi Stage Docker build example
`Dockerfile` contains various stages which are tagged by a name using `as`.

## Commands used

```
# Variante 1 
# alles bauen  
docker build . -t multi-stage-example:v1
docker run -p 8080:8080 multi-stage-example:v1 
```

## Debuggen 

```
# So könnte ich debuggen, 2. Teil wird nicht gebaut 
# build bis zum target / dort davor stoppen 
docker build . -t multi-stage-example:v1 --target=builder
```


## Reference:

  * https://docs.docker.com/build/building/multi-stage/
