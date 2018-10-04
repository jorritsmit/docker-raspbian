
# docker-raspbian

![Docker Build Status](https://img.shields.io/docker/build/hannseman/raspbian.svg)

This docker image runs QEMU system emulation for Raspbian Stretch Lite. 
It will let you run Raspbian as if it was running on an actual Raspberry PI. 

## Usage

SSH is enabled on port `2222`. The username is `pi` and the password is `raspberry`. 

To run the container:

`docker run -it -p 2222:2222 --privileged hannseman/raspbian`

To connect with SSH:

`ssh -p 2222 -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no pi@localhost`
