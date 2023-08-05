# Simple Docker Webapp

This repository contains a simple Docker web application. Follow the instructions below to build and run the application.

## Instructions

1. **Build the Docker Image**

   In your terminal, navigate to the directory containing the application. Then, build the Docker image using the following command:

```bash
  docker build -t name/repository-name:tag
```

For example:

```bash
  docker build -t kobibell/docker-web:latest
```

2. **Run the Docker Container**

   Run the Docker container with port mapping using the following command:

```bash
  docker run -p 8080:8080 kobibell/docker-web
```

You can then access the application by navigating to `http://localhost:8080/` in your web browser.

3. **Check the Files in the Container**

   To verify that all files are in the `/usr/app` directory, open a new terminal and run the following command:

```bash
docker exec -it [containerid] sh
ls
```

You should see the following output:

```bash
/usr/app # ls
Dockerfile         README.md          index.js           node_modules       package-lock.json  package.json
```

## Author

- [Kobi Bell](https://gitlab.com/kobibell)

## Conclusion

Thank you for checking out this project. If you have any questions or feedback, feel free to open an issue. Happy coding!
