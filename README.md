## About:

[Docker](http://www.docker.com/) image based on [digitalwonderland/base](https://registry.hub.docker.com/u/digitalwonderland/base/)

## Additional Software:

* [Redis 3](https://github.com/antirez/redis/raw/3.0/00-RELEASENOTES)

## Usage:

Same as [dockerfile/redis](https://registry.hub.docker.com/u/dockerfile/redis/) except:

1. it is based on CentOS 7
2. it contains the latest Redis 3.x builds
3. ```/var/lib/redis``` is used instead of ```/data```

```CMD``` is set to ```["redis-server", "/etc/redis/redis.conf"]``` so you can just use it as you would use the official container, i.e.:

``` 
$ docker run -d --name redis -p 6379:6379 digitalwonderland/redis
```
