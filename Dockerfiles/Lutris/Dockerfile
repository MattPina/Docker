#Incomplete
FROM ubuntu
ENV DEBIAN_FRONTEND=noninteractive
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
	--no-install-recommends \
	wine \
	software-properties-common \
	&& rm -rf /var/lib/apt/lists/
RUN add-apt-repository ppa:lutris-team/lutris
RUN apt update
RUN apt install -y lutris
RUN useradd -ms /bin/bash user
WORKDIR /home/user
USER user
CMD ["/usr/games/lutris"]
