# luzifer / inspircd

# luzifer/dockerproxy Dockerfile

This repository contains **Dockerfile** of [InspIRCd](http://www.inspircd.org/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/luzifer/inspircd/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).

## Base Docker Image

- [debian](https://registry.hub.docker.com/_/debian/)

## Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/luzifer/inspircd/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull luzifer/inspircd`

## Usage

Create a directory containing the configuration for the [InspIRCd](http://www.inspircd.org/) with at least the [inspircd.conf](https://github.com/inspircd/inspircd/blob/master/docs/conf/inspircd.conf.example)

Then launch it with your configuration:

```
docker run -d -p 6667:6667 -v /home/myuser/config:/inspircd/conf luzifer/inspircd
```

Easy!

