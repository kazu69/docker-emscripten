alpine base Docker with emscripten container
====================

[![Build Status](https://travis-ci.org/kazu69/docker-emscripten.svg?branch=master)](https://travis-ci.org/kazu69/docker-emscripten)

> You can create the docker image you need to develop in the Alpine Linux

Installation
-----

The easiest way to do this is to get from Docker registry

```sh
$ docker pull kazu69/emscripten
```

Also possible to use or from github to get

```sh
$ git clone https://github.com/kazu69/docker-emscripten.git
$ cd docker-emscripten
$ docker build -t kazu69/docker-emscripten .
```

build
----

example

```sh
$ docker run -v $(pwd)/example:/tmp -it kazu69/docker-emscripten /bin/bash

bash-4.3# cd /tmp && ./build hello.c hello.html
# build
bash-4.3# ls example
build          hello.c        hello.html     hello.html.mem hello.js
```
