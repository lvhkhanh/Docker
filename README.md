# Docker

* [THAT Conference '19: The Absolute Beginner's Guide to Docker](https://app.pluralsight.com/library/courses/that-conference-2019-session-33/table-of-contents)
* [docker-kubernetes-big-picture](https://app.pluralsight.com/library/courses/docker-kubernetes-big-picture)
* [summer-of-skills](https://www.pluralsight.com/offer/2019/summer-of-skills) - [@KhanhLVH](https://app.pluralsight.com/profile/KhanhLVH)
* [Play with Docker classroom](https://training.play-with-docker.com/)

Turn on docker experimental
![](https://snipboard.io/ncemTz.jpg)


```
git clone https://github.com/docker/doodle.git
```

[New to git? Install it here.](https://help.github.com/en/articles/set-up-git)

```
cd doodle\cheers2019 ; docker build -t khanhlvh/cheers2019 .
docker run -it --rm khanhlvh/cheers2019
docker login ; docker push khanhlvh/cheers2019
```

```
# build a image
docker image build -t <repo_name>:<tag_id> .
# list out an image
docker image ls <repo_name>:<tag_id>
# register image
docker image push <repo_name>:<tag_id>
```

```
# list out all image
docker image ls
REPOSITORY          TAG       IMAGE ID      CREATED       SIZE
<repo_name>         <tag_id>
# run a forward port 
docker run -d --name web -p 8080:8080 <repo_name>:<tag_id>
docker stop web 
docker container start web
```
```
docker ps
docker ps -a
docker rm <at least 3 chars start of id>
docker stop <at least 3 chars start of id>
docker run --rm <name>
docker run --rm nginx
```
```
# mapping volume from current directory to code folder inside container 
docker run -rm -it -v ${PWD}:/code python
```
