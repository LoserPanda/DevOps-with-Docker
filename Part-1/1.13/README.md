# Part 1

## 1.13

In order to run the *spring-example-project*, which you can find from https://github.com/LoserPanda/spring-example-project/tree/feature/dockerfile, in a Docker container, build the project first locally by running:

```
./mvnw package
```

Then build the Docker image by running:

```
docker build -t spring-example-project .
```

Finally, run the container by running:

```
docker run -p 8080:8080 spring-example-project
```

Now you can navigate to http://localhost:8080 to see the spring app up and running.
