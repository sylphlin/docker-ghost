# docker-ghost

[![Build Status](https://travis-ci.org/sylphlin/docker-ghost.svg?branch=master)](https://travis-ci.org/sylphlin/docker-ghost)
[![CircleCI](https://circleci.com/gh/sylphlin/docker-ghost.svg?style=svg)](https://circleci.com/gh/sylphlin/docker-ghost)

## Introduction
This docker stack build up two container to run ghost blog system and ngnix as reverse proxy based on the official images. 

## Pre-request
- docker: 1.8.2 or above
- docker-compose: 1.4.2 or above

## Usage
#### 1. Install docker and docker-compose
You need to install the docker and docker-compose before you use it. Refer the offical site for [docker install] (https://docs.docker.com/engine/installation/) and [docker-compose install] (https://docs.docker.com/compose/install/)

#### 2. Modify The Base URL and Certificate
1. Change the `GHOST_BASE_URL` in `docker-compose.yml` to the Real URL.
2. Modify the certificate in `nginx/keys` before launch. The file in this folder is a sample certificate for testing.

#### 3. Launch This Stack
You can simple use docker-compose to launch this stack in the background.
```
# docker-compose up -d
```
