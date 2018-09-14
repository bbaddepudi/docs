**NOTE:**
The Docker option to run local clusters is recommended only for advanced Docker users. This is because running stateful apps like YugaByte DB in Docker is more complex and error-prone than the more common stateless app use cases.

## Prerequisites

a) You must have the Docker runtime installed on your localhost. Follow the links below to download and install Docker if you have not done so already.

<i class="fa fa-apple" aria-hidden="true"></i> [Docker for Mac](https://store.docker.com/editions/community/docker-ce-desktop-mac) 

<i class="icon-centos"></i> [Docker for CentOS](https://store.docker.com/editions/community/docker-ce-server-centos) 

<i class="icon-ubuntu"></i> [Docker for Ubuntu](https://store.docker.com/editions/community/docker-ce-server-ubuntu) 

<i class="icon-debian"></i> [Docker for Debian](https://store.docker.com/editions/community/docker-ce-server-debian) 

<i class="fa fa-windows" aria-hidden="true"></i> [Docker for Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows) 

b) Verify that you have python2 installed. Support for python3 is in the works.

```{.sh .copy .separator-dollar}
$ python --version
```
```sh
Python 2.7.10
```

## Download

Download the [yb-docker-ctl](../../admin/yb-docker-ctl/) utility. This utility has a set of pre-built commands to create and thereafter administer a containerized local cluster. 

```{.sh .copy .separator-dollar}
$ mkdir ~/yugabyte && cd ~/yugabyte
```
```{.sh .copy .separator-dollar}
$ wget https://downloads.yugabyte.com/yb-docker-ctl && chmod +x yb-docker-ctl
```

## Install

Confirm that Docker and python are installed correctly.

```{.sh .copy .separator-dollar}
$ docker ps
```
```{.sh .copy .separator-dollar}
$ python --version
```

Pull the YugaByte DB container.

```{.sh .copy .separator-dollar}
$ docker pull yugabytedb/yugabyte
```