FROM crops/poky:ubuntu-18.04

USER root

# Add git-lfs from packagecloud
# as recommended by https://git-lfs.github.com/
RUN apt-get update && apt-get install curl
RUN curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash

RUN apt-get update && apt-get install -y vim rpm git zlib1g-dev lib32stdc++-5-dev git-lfs gcc-multilib g++-multilib
RUN rm -rf /var/lib/apt/lists/*
