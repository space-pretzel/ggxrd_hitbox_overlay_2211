# build the image with
# docker build . -t xrd-hitbox-overlay
# docker run -t -v ..:/ggxrd_hitbox_overlay_2211 --name build-mod

# and get the compiler output with:
# docker exec -t build-mod ./build.py

# if you get an error that the container is not running
# docker start build-mod


FROM ubuntu:24.04

ENV CHOST=i686-w64-mingw32
WORKDIR /ggxrd_hitbox_overlay_2211/ggxrd_hitbox_overlay

RUN apt-get update && apt-get install -qq \
    gcc \
    gcc-mingw-w64-i686 \
    g++-mingw-w64-i686 \
    git \ 
    make \
    cmake \
    python3
