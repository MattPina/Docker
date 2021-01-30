# docker container run \
#   --name youtube-dl \
#   -it \
#   --restart unless-stopped \ (optional)
#   -v C:\Users\username\Youtube-dl:/youtube-dl \ (Windows)
#   -v /home/username/Youtube-dl:/youtube-dl \ (Linux)
#   youtube-dl:latest (For use after the Dockerfile creation)

FROM alpine
ENV ALPINE_FRONTEND=noninteractive
RUN apk update
#RUN apk add youtube-dl
RUN apk add curl python2 python3
RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
RUN chmod a+rx /usr/local/bin/youtube-dl
WORKDIR /youtube-dl
