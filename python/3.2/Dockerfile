FROM dockershelf/debian:wheezy
MAINTAINER Luis Alejandro Martínez Faneyth <luis@huntingbears.com.ve>

ARG BUILD_DATE
ARG VCS_REF
ARG VERSION

LABEL org.label-schema.build-date=${BUILD_DATE} \
      org.label-schema.name="python3.2" \
      org.label-schema.description="A Python 3.2 image based on Debian Sid." \
      org.label-schema.url="https://github.com/LuisAlejandro/dockershelf" \
      org.label-schema.vcs-ref=${VCS_REF} \
      org.label-schema.vcs-url="https://github.com/LuisAlejandro/dockershelf" \
      org.label-schema.vendor="Luis Alejandro Martínez Faneyth" \
      org.label-schema.version=${VERSION} \
      org.label-schema.schema-version="1.0.0-rc.1"

ENV PY_VER_NUM="3.2" PY_DEBIAN_SUITE="wheezy" PYTHONIOENCODING="UTF-8"

COPY *.sh /usr/share/dockershelf/python/
RUN bash /usr/share/dockershelf/python/build-image.sh

CMD ["/bin/bash"]