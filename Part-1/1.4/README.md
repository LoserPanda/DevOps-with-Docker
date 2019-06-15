# Part 1

## 1.4

Below you can find the commands and outputs produced by them:

```
docker run devopsdockeruh/exec_bash_exercise
```

```
docker ps
```

*output*
```
CONTAINER ID        IMAGE                               COMMAND             CREATED             STATUS              PORTS               NAMES
bb407fe32cbf        devopsdockeruh/exec_bash_exercise   "node index"        17 seconds ago      Up 14 seconds                           hungry_villani
```

```
docker exec -it bb407fe32cbf bash
```

```bash
tail -f ./logs.txt
```

*output*
```
"Docker is easy"
Fri, 31 May 2019 18:55:21 GMT
Fri, 31 May 2019 18:55:24 GMT
Fri, 31 May 2019 18:55:27 GMT
Fri, 31 May 2019 18:55:30 GMT
Secret message is:
"Docker is easy"
Fri, 31 May 2019 18:55:36 GMT
Fri, 31 May 2019 18:55:39 GMT
Fri, 31 May 2019 18:55:42 GMT
Fri, 31 May 2019 18:55:45 GMT
Secret message is:
"Docker is easy"
Fri, 31 May 2019 18:55:51 GMT
Fri, 31 May 2019 18:55:54 GMT
Fri, 31 May 2019 18:55:57 GMT
```
