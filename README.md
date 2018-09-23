# Containerized

This is a collection of the various dockerfiles that I use in my system.
Containerizing standard desktop applications has multiple advantages: 

* Possibility to limite the available resources per application (Looking at you, webbrowsers!)
* Prevent polluting of your filesystem
* Adds some (weak) level of security

## Install

Add the bin folder to your PATH
```
export PATH=$PATH:$(readlink -f containerized/bin)
```

## Build

The docker images will automaticly be build on the first time you run one of the commands.
That requires DOCKER_HOME_DIR to be defined.
```
export DOCKER_HOME_DIR=$(readlink -f containerized/docker)
```

### Credit

Inspired by Jess Frazelle
