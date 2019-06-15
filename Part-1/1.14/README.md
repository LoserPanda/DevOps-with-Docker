# Part 1

## 1.14

To run the *rails-example-project*, clone the project first from

* https://github.com/LoserPanda/rails-example-project/tree/feature/dockerfile

Now, in the project root run these two commands:


```
docker build -t rails-example-project .
```

```
docker run -p 3000:3000 rails-example-project
```

As soon as the application is up and running, navigate to http://localhost:3000 and verify the application works by clicking the *Press* button.

In order to make the *rails-example-project* work with Docker, the *Gemfile* of the project was modified so that the ruby version number became '2.6.3'.
