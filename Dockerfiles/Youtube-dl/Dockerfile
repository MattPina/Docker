# Uses yt-dlp, the maintained fork of youtube-dl.
# docker container run \
#   --name yt-dlp \
#   -it \
#   --restart unless-stopped \ (optional)
#   -v C:\Users\username\Youtube-dl:/youtube-dl \ (Windows)
#   -v /home/username/Youtube-dl:/youtube-dl \ (Linux)
#   yt-dlp:latest (For use after the Dockerfile creation)

FROM alpine
RUN apk add --no-cache yt-dlp ffmpeg
WORKDIR /youtube-dl
