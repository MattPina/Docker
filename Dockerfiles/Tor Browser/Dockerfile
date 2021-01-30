# docker container run -v /tmp/.X11-unix:/tmp/.X11-unix \
#	-v /home/'user':/home/user \ (change for your own information)
#	--device /dev/snd \
#	--device /dev/dri \
#	-v /dev/shm:/dev/shm \
#	-e DISPLAY=unix$DISPLAY \
#	Image name
#	/home/user/.local/share/torbrowser/tbb/x86_64/tor-browser_en-US/Browser/start-tor-browser

FROM ubuntu
ENV UBUNTU_FRONTEND=noninteractive
RUN apt update && apt install -y \
	ca-certificates \
	curl \
	dirmngr \
	gnupg \
	libasound2 \
	libdbus-glib-1-2 \
	libgtk-3-0 \
	libxrender1 \
	libx11-xcb-dev \
	libx11-xcb1 \
	libxt6 \
	xz-utils \
	file \
	torbrowser-launcher \
	dirmngr \
	gnupg \
	apulse \
	ffmpeg \
	libgl1-mesa-dri \
	libgl1-mesa-glx \
	libpulse0 \	
	--no-install-recommends 
RUN rm -rf /var/lib/apt/lists/*
RUN useradd -ms /bin/bash user
WORKDIR /home/user
USER user
CMD ["torbrowser-launcher"]
