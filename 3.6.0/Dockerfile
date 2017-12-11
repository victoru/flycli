FROM alpine:3.6 as builder

RUN apk --no-cache add openssl ca-certificates

ENV FLY_VERSION 3.6.0
RUN wget -O /usr/local/bin/fly https://github.com/concourse/concourse/releases/download/v${FLY_VERSION}/fly_linux_amd64 \
	&& chmod +x /usr/local/bin/fly

ENTRYPOINT /usr/local/bin/fly
