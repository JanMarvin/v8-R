FROM archlinux:latest

ENV target v8-r

RUN pacman -Syu --noconfirm && pacman -S base-devel git icu lld python3 rlwrap --noconfirm

RUN useradd -m archie

USER archie

WORKDIR /home/archie

RUN git clone https://github.com/JanMarvin/v8-r 

WORKDIR /home/archie/v8-r

# RUN git checkout testing

RUN git config --global http.postBuffer 524288000

RUN makepkg

RUN sha256sum v8-r-*-x86_64.pkg.tar.zst > v8-r.sha256sum

