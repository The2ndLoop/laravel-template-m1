## When go into a container
When you enter a docker container, you use service name instead of container name.
```shell
docker compose exec <service_name> bash
```

## Log
If you do not set a container name, the log will be a little bit messy like this.

```
docker-laravel-nginx-1  | /docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
```

If you set a container name as nginx, the log will be like this
```
nginx  | /docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
```

You can't use the same name as running container's.
