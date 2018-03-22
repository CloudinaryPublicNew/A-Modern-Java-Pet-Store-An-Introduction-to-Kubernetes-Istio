# Step One: Dockerize the Application



I have found a nice recipe for Dockerizing the jPetStore app.

In short I created an account on docker.io — blumareks. I added my image of jpetstore to the repository there, so it can be referenced in the next steps.

Check my github repo for the details:[https://github.com/blumareks/2018-petstore](https://github.com/blumareks/2018-petstore)

I have changed the files responsible for the push to the registry — docker-compose.yml  
After that I was able to build and run my docker image using Docker for Mac:  
```code
$ docker-compose build  
```

```code
$ docker-compose up -d  
```

\* to stop it and remove the images \(rm\) just write:  
```code
docker-compose stop  
docker-compose rm -f
```

When I tested that everything works I was ready to push the images to the Docker repository:  
```code
$ docker-compose push
```

And they are here:[https://cloud.docker.com/app/blumareks/repository/list](https://cloud.docker.com/app/blumareks/repository/list)

Running my image on my local machine even in the cool Docker wasn’t the thing I wanted. I wanted to deploy it on the ☁️ and have it taken care of. So I learned that people are using Kubernetes for that. So I decided to do what is fashionable — the Silicon Valley way 🌁



