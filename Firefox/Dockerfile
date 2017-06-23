FROM alpine

#MAINTAINER Zach Deibert<zachdeibert@gmail.com>
#MAINTAINER Daniel Guerra <daniel.guerra69@gmail.com>
MAINTAINER Mathias Stadler<stadler-mathias@web.de>



ENTRYPOINT ["/launch.sh"]
CMD [":0"]

RUN apk --update --no-cache add bash \
 firefox-esr \
                    libcanberra-gtk3 \
                    dbus-x11 \
                    libstdc++ \
                    libgcc \
                    musl \
                    ttf-dejavu \
                    su-exec  \
    && rm -rf /tmp/* /var/cache/apk/*

 
ADD launch.sh /launch.sh
