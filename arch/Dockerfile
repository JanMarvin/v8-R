FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S base-devel python2 python3 git rlwrap --noconfirm

RUN useradd -m archie

USER archie

WORKDIR /home/archie

RUN git clone https://github.com/JanMarvin/v8-r && cd v8-r && git checkout devel

WORKDIR /home/archie/v8-r

RUN makepkg

RUN sha256sum v8-r-*-x86_64.pkg.tar.zst > v8-r.sha256sum

