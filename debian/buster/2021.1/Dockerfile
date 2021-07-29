FROM vlrpi/rpi-jdk11:debian-buster
LABEL maintainer="Vova Lantsov"
LABEL contact_email="contact@vova-lantsov.dev"
LABEL telegram="https://t.me/vova_lantsov"

COPY cache/teamcity/2021.1 .

EXPOSE 8111 9090

ENV TEAMCITY_DATA_PATH /root/BuildServer
ENTRYPOINT ["TeamCity/bin/teamcity-server.sh","run"]