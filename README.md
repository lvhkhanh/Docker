# Docker

* [docker-kubernetes-big-picture](https://app.pluralsight.com/library/courses/docker-kubernetes-big-picture)
* [summer-of-skills](https://www.pluralsight.com/offer/2019/summer-of-skills) - [@KhanhLVH](https://app.pluralsight.com/profile/KhanhLVH)
* [Play with Docker classroom](https://training.play-with-docker.com/)


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

