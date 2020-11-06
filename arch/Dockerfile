FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S python2 python3 git rlwrap --noconfirm

RUN useradd -m archie

RUN su archie

RUN git clone https://github.com/JanMarvin/v8-r

WORKDIR /v8-r

RUN makepkg
