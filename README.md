# [Alpine Google Cloud CLI Docker Images](https://hub.docker.com/r/jamespedwards42/alpine-cloud-sdk/) [![](https://images.microbadger.com/badges/image/jamespedwards42/alpine-cloud-sdk.svg)](https://microbadger.com/images/jamespedwards42/alpine-cloud-sdk "microbadger.com")

## Supported Tags

* [`latest`](https://github.com/jamespedwards42/alpine-cloud-sdk/blob/master/Dockerfile) FROM openjdk:7-jre-alpine

## Docker Run

```sh
docker run -i -t --rm \
  -v $HOME/.config/gcloud:/.config/gcloud\
  -v $PWD:/data \
  -w /data \
  jamespedwards42/alpine-cloud-sdk:latest
```

## Shell Alias

```sh
alias gcloud="docker run -i -t --rm\
  -v $HOME/.config/gcloud:/.config/gcloud\
  -v $PWD:/data\
  -w /data\
  jamespedwards42/alpine-cloud-sdk:latest "
```
