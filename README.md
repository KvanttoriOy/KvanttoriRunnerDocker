# First time setup:
## Gitlab:


Follow the setup by running:
```docker run --rm -it -v /srv/gitlab-runner/config:/etc/gitlab-runner gitlab/gitlab-runner register```

**Instance Url** is `https://gitlab.com`


**Registeration token** must be gotten from an **admin**

**Enter a description** and optionally **tags**

When prompted with **type**, select `docker`

**Default docker image** can be set as `node`

## Github:

Enter creds into .env,

Runner token has to be gotten from an admin

# Running
It's as simple as running
```docker-compose up -d```