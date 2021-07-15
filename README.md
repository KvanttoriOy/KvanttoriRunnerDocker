# What's this?
This is a docker-compose file for setting up two runners for both gitlab and github within kvanttori, they're auto restarting and need to only be set up once

# First time setup:
## Gitlab:


Follow the setup by running:
```docker run --rm -it -v kvanttorirunnerdocker_gitlab-runner-config:/etc/gitlab-runner gitlab/gitlab-runner:latest register```

**Instance Url** is `https://gitlab.com`


**Registeration token** must be gotten from an **admin**

**Enter a description** and optionally **tags**

When prompted with **type**, select `docker`

**Default docker image** can be set as `node`

## Github:

Enter creds into .env,

Runner token has to be gotten from an admin

## First time docker run
It's as simple as running ```docker-compose up -d```, this will create the containers and volumes for you

#  Stopping and resuming
```docker-compose stop```

```docker-compose start```

# Removing containers and volumes
```docker-compose down```
