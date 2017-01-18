Image installation
---

`docker build -t th108/wine-winbox https://raw.githubusercontent.com/th108/dockerfiles/master/wine-winbox/Dockerfile`

Running the container
---

`docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=unix$DISPLAY th108/wine-winbox wine winbox.exe`

Gtk: cannot open display: :0
---

`xhost local:root`
source: https://github.com/jessfraz/dockerfiles/issues/4
