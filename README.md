# ASTRA-Sim Dockerfile
## Install Docker (if you have root permission)
```
# apt -y update
# apt -y install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common
# curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
# apt-key fingerprint 0EBFCD88
# add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
# apt -y update
# apt -y install docker-ce
```

## Quick Start
```
$ ./build.sh
$ docker run -it astra-sim
# cd astra-sim
# ./build/astra_analytical/build.sh -c
# examples/run_allreduce.sh -n analytical
```
