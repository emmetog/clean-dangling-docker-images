Intro
=====
This container removes any "dangling" docker images.  Run it every now and
again on your development machine to reclaim disk space.

Dangling images are created when you build and rebuild images. If you're
building and rebuilding images often you might find yourself running out
of disk space. This container removes all the old images that are dangling.

It won't remove any images that are currently in use, even if they're dangling.

Usage
=====

```
$ docker run --rm -v /var/run/docker.sock:/var/run/docker.sock emmetog/clean-dangling-docker-images
```