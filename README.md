# Simple Docker Webapp

## Instructions

### To run the docker web application, follow these instructions:

- Run the following command in your current working directory of the application:

Build the image with a tag

```bash
  docker build -t name/repository-name:tag
```

e.g.

```bash
  docker build -t kobibell/docker-web:latest
```

Now run the port mapping with the following command:

```bash
  docker run -p 8080:8080 kobibell/docker-web
```

You can check the port mapping is running by going to your local host in your web browser and go to the following link: http://localhost:8080/

Check all the files is in the /usr/app directory by opening a new terminal and running the following command:

```bash
docker exec -it [containerid] sh
ls
```

and you should see the following output:

```bash
/usr/app # ls
Dockerfile         README.md          index.js           node_modules       package-lock.json  package.json
```

## Author

- [Kobi Bell](https://gitlab.com/kobibell)
