# ARM Linux Alpine base image for Docker

This repository will be place where to build and test an ARM base image for Linux Alpine.

Actual URL is : https://registry.hub.docker.com/u/dduportal/rpi-alpine/ 

## Content

This image is build with the Docker's [mkimage-alpine.sh](https://github.com/docker/docker/blob/master/contrib/mkimage-alpine.sh), from original Alpine Linux distribution, in order to limit the potential unknown things in the userland.

## Thoughts and TODOs

Idea came from [progrium](https://github.com/progrium/) and it's [x64 Linux Alpine base image](https://github.com/gliderlabs/docker-alpine) aimed to replace busybox one.

Goal is to auto-build this image and test it using thoses things :
* CirleCI or TravisCI for public build using quemu emulation : http://www.tomaz.me/2013/12/02/running-travis-ci-tests-on-arm.html
* Some bats testing as usual
