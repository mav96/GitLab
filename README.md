# GitLab

1. Init docker swarm

```
docker swarm init
```
2. Starting gitlab with registry

```
docker stack deploy -c docker-stack.yml gitlab
```

3. Change certs for https://gitlab.selit.ru
```
docker exec -it  <container_id> bash
vi /etc/gitlab/ssl/gitlab.selit.ru.crt
vi /etc/gitlab/ssl/gitlab.selit.ru.key
```
