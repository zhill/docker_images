FROM alpine:latest

# Add some fake secrets
COPY ssh /root/.ssh
COPY aws /root/.aws

RUN apk update -y && \ 
	apk add curl wget

# Modify the wget binary to change the digest
RUN echo 1 >> /usr/bin/wget

