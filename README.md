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

## Quick Start (ASTRA-Sim)
```
$ cd astra-sim
$ ./build.sh
$ docker run -it astra-sim
# cd astra-sim
# ./build/astra_analytical/build.sh -c
# examples/run_allreduce.sh -n analytical
```

## Quick Start (GitHub Pages)
```
$ cd astra-sim.github.io
$ ./build.sh
$ docker run -it astra-sim-github-io
# cd astra-sim.github.io
# docker run -p 4000:4000 -it astra-sim-pages
# cd astra-sim.github.io
# bundle install
# bundle exec jekyll serve --host=0.0.0.0
```
