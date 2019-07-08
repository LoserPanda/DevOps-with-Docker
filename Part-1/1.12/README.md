# Part 1

## 1.12

To run the applications together clone these two forked and edited projects

* https://github.com/LoserPanda/frontend-example-docker/tree/feature/connect-to-backend
* https://github.com/LoserPanda/backend-example-docker/tree/feature/connect-to-frontend

Now, in the *frontend-example-docker* root folder run these commands:

```
docker build -t frontend-example-docker .
```

```
docker run -p 5000:5000 frontend-example-docker
```

Similarly, run these two commands in the *backend-example-docker* root folder:

```
docker build -t backend-example-docker .
```

```
docker run -v c:/logs/logs.txt:/usr/app/logs.txt -p 8000:8000 backend-example-docker
```

As soon as the both applications are up and running, navigate to http://localhost:5000 and click the button for 1.12 and verify the applications work together. The button should turn green.
