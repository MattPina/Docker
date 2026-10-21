# docker container run \
#   --name gallery-dl \
#   -it \
#   --restart unless-stopped \ (optional)
#   -v C:\Users\username\Gallery-dl:/gallery-dl \ (Windows)
#   -v /home/username/Gallery-dl:/gallery-dl \ (Linux)
#   gallery-dl:latest (For use after the Dockerfile creation)

FROM python:3-alpine
RUN pip install --no-cache-dir --upgrade gallery-dl
WORKDIR /gallery-dl
