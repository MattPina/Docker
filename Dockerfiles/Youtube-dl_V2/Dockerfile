# Uses yt-dlp, the maintained fork of youtube-dl, downloaded straight from its latest release.
# docker container run \
#   --name yt-dlp \
#   -it \
#   --restart unless-stopped \ (optional)
#   -v C:\Users\username\Youtube-dl:/youtube-dl \ (Windows)
#   -v /home/username/Youtube-dl:/youtube-dl \ (Linux)
#   yt-dlp:latest (For use after the Dockerfile creation)

FROM alpine
RUN apk add --no-cache curl python3 ffmpeg
RUN curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp \
	&& chmod a+rx /usr/local/bin/yt-dlp
WORKDIR /youtube-dl
