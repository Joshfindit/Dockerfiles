# nmap in a container:
# [ docker run -it --rm networkstatic/nmap --help ]
# Scan for open ssh (tcp/22) ports on a range of IPs
# [ docker run -it --rm networkstatic/nmap -sT 192.168.1.1-100 -p 22 ]
FROM alpine:latest

MAINTAINER Brent Salisbury <brent.salisbury@gmail.com>

# install binary without cache
RUN apk --no-cache add \
	nmap

ENTRYPOINT ["nmap"]
