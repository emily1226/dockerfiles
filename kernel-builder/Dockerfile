FROM r.j3ss.co/wireguard:install
LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apk add --no-cache \
	bash \
	bc \
	bison \
	ca-certificates \
	curl \
	fakeroot \
	flex \
	git \
	gmp-dev \
	libressl-dev \
	mpc1-dev \
	mpfr-dev \
	ncurses-dev \
	tar

ENV HOME /root
WORKDIR $HOME

ENV JOBS 4

COPY build_kernel /usr/local/bin/build_kernel

ENTRYPOINT [ "bash" ]
