# Part 1

## 1.10

To run the frontend application presented in [https://github.com/LoserPanda/frontend-example-docker/tree/feature/dockerfile] run the following from the project root:

```
docker build -t frontend-example-docker .
```

```
docker run -p 5000:5000 frontend-example-docker
```

After running the commands, visit [localhost:5000] to verify the web application successfully runs on Docker container.
