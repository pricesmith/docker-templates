FROM rust:lts-alpine

# install packages specifically related to network troubleshooting
RUN apk add --no-cache \
	-X http://dl-cdn.alpinelinux.org/alpine/edge/main \
	-X http://dl-cdn.alpinelinux.org/alpine/edge/community \
	-X http://dl-cdn.alpinelinux.org/alpine/edge/testing \
	bash \
	bind-tools \
	curl \
	fping \
	hping3 \
	iproute2 \
	iproute2-minimal \
	iproute2-ss \
	mtr \
	openssl \
	traceroute \
	&& :

# Update rust
RUN rustup update

# Install PNPM
RUN curl -fsSL "https://github.com/pnpm/pnpm/releases/latest/download/pnpm-linuxstatic-x64" -o /bin/pnpm; chmod +x /bin/pnpm;



