# Part 1

## 1.8

Below are commandws to start the container *devopsdockeruh/first_volume_exercise* with a bind mount so that the logs are created to Windows' filesystem:

```powershell
docker run -v c:/logs/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
```

This is the only way I got the container with bind mount working so that the files were created to my local filesystem. The *logs.txt* file had to be created in advance though.
