FROM alpine:latest

RUN apk update
RUN apk add curl git fish gcc

RUN curl –proto ‘=https’ –tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
SHELL ["/usr/bin/fish", "-c"]
RUN fish_add_path $HOME/.cargo/bin/

ENV SHELL /usr/bin/fish
