Freshrss + mariadb docker
---

Here are the steps to get a working Freshrss install:

- First clone this repo

```sh
$ git clone https://github.com/lovenunu/docker-freshrss-mariadb
```

- Then change the mariadb root password in `docker-compose.yml` (replace `%your_db_password%` with a faceroll over your keyboard)

- Start the containers

```sh
$ docker-compose up -d
```

Finally on Freshrss configuration (first access to the application), when asked to configure mysql, provide these informations:
- Host: `db`
- User: `root` (Security FIRST)
- Password: _The password you configured_
- Database: `freshrss`
