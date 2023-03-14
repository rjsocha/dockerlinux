# dockerlinux (working name)

PoC/research project - build docker (container) image based on packages

Starting example
```
# syntax=docker/dockerfile:1.5
FROM wyga/dockerlinux-base:latest
COPY --link --from=wyga/dockerlinux-busybox:latest / /
COPY --link --from=wyga/dockerlinux-busybox-system:latest / /
```
