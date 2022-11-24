
FROM  ubuntu:18.04

#SHELL ["/bin/bash", "-c"]

RUN  apt-get update && \
     apt-get -y install sudo apt-utils less zsh wget git && \
     useradd -m ubuntu && echo "ubuntu:ubuntu" | chpasswd && adduser ubuntu sudo


USER  ubuntu

WORKDIR /home/ubuntu


RUN sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" | zsh || true

#SHELL ["/bin/bash", "-c"]



#SHELL ["/bin/bash", "--login", "-c"]
#SHELL ["/bin/bash", "-ec"]




CMD  ["tail", "-f", "/dev/null"]

