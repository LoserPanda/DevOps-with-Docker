# Part 1

## 1.11

To run the backend application presented in https://github.com/LoserPanda/backend-example-docker/tree/feature/dockerfile run the following from the project root:

```
docker build -t backend-example-docker .
```

```
docker run -v c:/logs/logs.txt:/usr/app/logs.txt -p 8000:8000 backend-example-docker
```

After running the commands, visit http://localhost:8000 to verify the application successfully runs on Docker container.
