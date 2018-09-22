## Containerized

This is a collection of the various dockerfiles that I use in my system.
Containerizing your application has multiple advantages: Possibility to limiting resources per application, prevent polluting of your filesystem, adds some level of weak security, ..

## Install

Add the bin folder to your PATH
```
export PATH=$PATH:$(readlink -f bin)
```

## Build

The docker images will automaticly be build on the first time you run one of the commands.
That requires DOCKER_HOME_DIR to be defined.
```
export DOCKER_HOME_DIR=$(readlink -f containerized/)
```

### Credit

Inspired by Jess Frazelle
