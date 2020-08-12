# Quick Review

```
docker-compose up -d --build
```

```
docker-compose exec web python manage.py migrate
```

```
docker-compose exec web python manage.py createsuperuser
```

Here is a short version of the terms and concepts we've covered in this post:

Image: the "definition" of your project
Container: what your project actually runs in (an instance of the image)
Dockerfile: defines what your image looks like
docker-compose.yml: a YAML file that takes the Dockerfile and adds additional instructions for how our Docker container should behave in production.

We use the Dockerfile to tell Docker how to build our image. Then we run our actual project within a container. The docker-compose.yml file provides additional information for how our Docker container should behave in production.
