Intro
=====
This container removes any "dangling" docker images.

Usage
=====

```
$ docker run --rm -v /var/run/docker.sock:/var/run/docker.sock docker-registry.nimblewarestudios.com/clean-dangling-docker-images
```