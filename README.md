# starting with docker-compose

This demo sets up a mysql database and a python image.
The python image will connect to the mysql image.

test the setup by running:

```
$ docker-compose up
```

After it has started you can access the web page : http://0.0.0.0:5000/

or use curl.

and you can access the database:

```
$ mysql --host=127.0.0.1 --port=32000 -u root -p
```

then do a ``` show databases; ``` and then ``` use knights; ``` 
you can then see the content by:

```
select * from favorite_colors;
```


Reference: [Dockerizing a Flask-MySQL app with docker-compose](https://stavshamir.github.io/python/2018/05/08/dockerizing-a-flask-mysql-app-with-docker-compose.html)