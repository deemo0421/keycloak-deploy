# keycloak deploy

> An auth system deploy for 2023/6  master's students [color=#3b75c6]
> To use docker compose, need install [docker](https://docs.docker.com/get-docker/) frist

### Step 1 Installation
Clone this [repo](https://github.com/jennyhuoh/try-keycloakify)  made by jennyhuoh 
```
git clone https://github.com/jennyhuoh/try-keycloakify
```

### Step 2: mount theme
In `docker-compose.yaml`, to mount theme into the container，you need to replace the directory in `source` under keycloak configuration. 
e.g. `C:\Users\wuret\Desktop\try-keycloakify\theme`
```
volumes:
      - type: bind
        source: you need to replace
        target: /opt/jboss/keycloak/themes/serendipity
```
### Step 3: launch container
then you can run `docker compose up -d`

