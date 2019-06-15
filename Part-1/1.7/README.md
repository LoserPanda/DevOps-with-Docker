# Part 1

## 1.7

From this directory you will find a *Dockerfile* that starts an *Ubuntu* container instance with *curl* installed in it. When running the build you get an interactive app that asks you a website and then outputs the value of the curl get of that url.

To build the image from a Dockerfile run:

```
docker build -t curler .
```

Then, to run the container run the following command:

```cmd
docker run --rm -it curler
```

The output of the run with an input of *helsinki.fi* should look like this:

```hmtl
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```
