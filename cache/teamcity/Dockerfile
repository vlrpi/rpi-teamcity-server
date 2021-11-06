FROM alpine

RUN apk add --update curl && \
    rm -rf /var/cache/apk/*

WORKDIR /teamcity

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2020.2.4.tar.gz && \
    mkdir 2020.2 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2020.2 && \
    rm TeamCity.tar.gz

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2021.1.4.tar.gz && \
    mkdir 2021.1 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2021.1 && \
    rm TeamCity.tar.gz

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2021.2.tar.gz && \
    mkdir 2021.2 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2021.2 && \
    rm TeamCity.tar.gz