### FROM 

http://www.jianshu.com/p/58a999ccb32e

### RUN 

```
bash get-data.sh
```

```
docker-compose run --rm initdb
```

edit `app.conf`

change:

    site.url=https://note.mydomain.com

to your domain

```
docker-compose up -d leanote
```

