FROM alpine:latest

LABEL maintaner=andrzej.pokrywko@gmail.com

RUN apk --update add git git-lfs openssh-client less tree && \
    rm -rf /var/lib/apt/lists/* && \
    rm -rf /var/cache/apk/*

VOLUME /git
WORKDIR /git

ENTRYPOINT ["git"]
CMD ["--help"]
