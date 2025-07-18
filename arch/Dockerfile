# FROM archlinux:latest
FROM ghcr.io/archlinux/archlinux:latest

ENV target=v8-r

RUN pacman -Syu --noconfirm && pacman -S base-devel clang procps-ng git icu lld llvm python3 rlwrap --noconfirm

RUN useradd -m archie

USER archie

WORKDIR /home/archie

RUN git clone -b clang https://github.com/JanMarvin/v8-r 

WORKDIR /home/archie/v8-r

RUN git config --global http.postBuffer 524288000

RUN makepkg

RUN sha256sum v8-r-*-x86_64.pkg.tar.zst > v8-r.sha256sum

