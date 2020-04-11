# nginx-rtmp-docker

A docker image running NGINX with the [nginx-http-flv-module](https://github.com/winshining/nginx-http-flv-module) (which includes the [nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module)).

**Git repository:** [https://github.com/ngrie/nginx-rtmp-docker](https://github.com/ngrie/nginx-rtmp-docker)\
**Docker image:** [https://hub.docker.com/r/ngrie/nginx-rtmp](https://hub.docker.com/r/ngrie/nginx-rtmp)

## Usage

```
docker run -d -p 1935:1935 ngrie/nginx-rtmp
```

### Use a custom NGINX configuration

The (basic) default configuration can be found [here](nginx.conf). It can be overridden like this:

```
docker run -d -p 1935:1935 -v /path/to/nginx.conf:/etc/nginx/nginx.conf ngrie/nginx-rtmp
```
