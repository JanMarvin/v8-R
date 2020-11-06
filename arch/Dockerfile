FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S python2 python3 git sudo rlwrap --noconfirm

RUN useradd -m archie

RUN sudo -u archie -s && \
    git clone https://github.com/JanMarvin/v8-r && \
    cd v8-r && \
    makepkg

