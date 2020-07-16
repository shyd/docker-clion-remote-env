# docker-clion-remote-env

CLion remote docker environment based on <https://blog.jetbrains.com/clion/2020/01/using-docker-with-clion/>

## How to run

```
docker run -d --rm --cap-add sys_ptrace -p127.0.0.1:2222:22 --name clion_remote_env shyd/clion-remote-env
ssh-keygen -f "$HOME/.ssh/known_hosts" -R "[localhost]:2222"
```

Or use the supplied `docker-compose.yml`.

ssh credentials (test user) `user@password`
