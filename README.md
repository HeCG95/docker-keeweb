# docker-keeweb
**Keeweb with Docker Compose** 

Using Docker Compose to create a self-hosting keeweb.

## Prerequisite

+ Install [Docker][1] and [Docker Compose][2] in your testing environment
+ Using docker image of [keeweb][3]

## Start with following steps

+ (1) Start keeweb

```
docker-compose up -d
```

The result is 

```
Creating docker-keeweb_keeweb_1 ... done
```

+ (2) Check the status of keeweb

```
docker-compose ps
```

The result is 

```
         Name                    Command            State                    Ports                  
----------------------------------------------------------------------------------------------------
docker-keeweb_keeweb_1   /opt/entrypoint.sh nginx   Up      0.0.0.0:443->443/tcp, 0.0.0.0:80->80/tcp
```

+ (3) View keeweb web console on : http://hostname:443.


[1]: https://www.docker.com
[2]: https://docs.docker.com/compose/
[3]: https://hub.docker.com/r/antelle/keeweb/

## License

Apache 2.0 license
