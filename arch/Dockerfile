FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S base-devel python2 python3 git sudo rlwrap --noconfirm

RUN useradd -m archie

USER archie

WORKDIR /home/archie

RUN git clone https://github.com/JanMarvin/v8-r 

WORKDIR /home/archie/v8-r

RUN makepkg

