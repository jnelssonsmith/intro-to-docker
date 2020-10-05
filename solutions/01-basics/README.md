# Docker basics

## Install Docker

## Running a container

Lets start by just jumping into a docker container, for this example we're going to use `ubuntu LTS Bionic (v18)`

Install docker and run:
`docker run -it --rm --init ubuntu:bionic`

Don't worry too much about what the above means just yet.
We are within ubuntu, you can have a look around and can confirm you are not being tricked via:

`cat /etc/issue` which should output `Ubuntu 18.04.5 LTS`

You can make files, folders and do all the usual linux stuff here

To exit the container type `exit` and you will be returned to your host environment
