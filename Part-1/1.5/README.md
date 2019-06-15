# Part 1

## 1.5

Below is the command used to start the process required:

```cmd
docker run --rm -it ubuntu:16.04 sh -c "apt-get update; apt-get install curl -y; echo 'Input website: '; read website; echo 'Searching...'; sleep 1; curl http://$website;"
```

If you input *helsinki.fi*, you'll get the following output:

```html
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```

It took a while to come up with this solution. For instance, running the command on Windows' Command Prompt caused trouble with the quotes. Also, it was important to run *apt-get update* before installing curl.
