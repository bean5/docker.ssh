# docker_ssh

A docker wrapper that maps your `~/.ssh` folder to a an alpine-based SSH container. It mounts to a corresponding `~/.ssh/` to the container as read-only. Previously it that was copied, permissions were modified, but with docker-compose, now it can be mounted directly.

## Warning

Although this is mounted as read-only, it is not recommended that you mount your actual `.ssh` folder. You should be mounting one that makes sense for your project.

## Requirements

* docker
* docker-compose

## Use

`docker compose up -d ssh`

Then use ssh as you normally would. Enjoy!
