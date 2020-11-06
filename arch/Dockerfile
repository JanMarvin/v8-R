FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S python2 python3 git icu rlwrap --noconfirm

RUN useradd -r -s /usr/bin/nologin archie

RUN su archie

RUN git clone https://github.com/JanMarvin/v8-r

WORKDIR /v8-r

RUN makepkg
