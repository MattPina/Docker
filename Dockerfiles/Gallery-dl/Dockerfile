# docker container run \
#   --name gallery-dl \
#   -it \
#   --restart unless-stopped \ (optional)
#   -v C:\Users\username\Gallery-dl:/gallery-dl \ (Windows)
#   -v /home/username/Gallery-dl:/gallerry-dl \ (Linux)
#   gallery-dl:latest (For use after the Dockerfile creation)

FROM alpine
ENV ALPINE_FRONTEND=noninteractive
RUN apk update
RUN apk add python3 py3-pip
RUN python3 -m pip install --upgrade gallery-dl
WORKDIR /
