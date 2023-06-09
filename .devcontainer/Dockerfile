FROM mcr.microsoft.com/devcontainers/universal:2-linux AS base
FROM ubuntu:focal

ENV LANG="C.UTF-8" \
    SHELL=/usr/bin/zsh \
    DOCKER_BUILDKIT=1

COPY --from=base / /

VOLUME [ "/var/lib/docker" ]
ENTRYPOINT [ "/usr/local/share/docker-init.sh", "/usr/local/share/ssh-init.sh"]
CMD [ "sleep", "infinity" ]