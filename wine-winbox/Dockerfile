FROM debian:testing-slim
MAINTAINER th108

RUN dpkg --add-architecture i386
RUN apt-get update && apt-get -y install --no-install-recommends wine32 wine && apt-get clean
RUN apt-get -y install wget

# RUN useradd -m winbox
# RUN echo "winbox:winbox" | chpasswd

RUN wget -q -O /winbox.exe http://download2.mikrotik.com/routeros/winbox/3.9/winbox.exe

# VOLUME ["/home/winbox"]

# USER winbox

# CMD ["wine winbox.exe"]
