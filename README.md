# Multi Stage Docker build example
`Dockerfile` contains various stages which are tagged by a name using `as`.

## Commands used

```
# build 
docker build . -t multi-stage-example:v1` - Build image
# use built stuff only 
docker build . -t multi-stage-example:v1 --target=builder
docker run -p 8080 multi-stage-example:v1 -p 8080:8080
```
