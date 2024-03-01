1. start and build

`docker compose up`

2. access the console

`docker exec -it mongodb mongo -u admin -p mongo`

2. select a db

`use banana`

3. create a new user for it

```
db.createUser(
  {
    user: 'vini',
    pwd: 'supersecret',
    roles: [ { role: 'root', db: 'admin' } ]
  }
);
```

4. exit
