FROM alpine

RUN apk add --update curl && \
    rm -rf /var/cache/apk/*

WORKDIR /teamcity

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2022.04.5.tar.gz && \
    mkdir 2022.04 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2022.04 && \
    rm TeamCity.tar.gz

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2022.10.4.tar.gz && \
    mkdir 2022.10 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2022.10 && \
    rm TeamCity.tar.gz

RUN curl -SL --output TeamCity.tar.gz https://download.jetbrains.com/teamcity/TeamCity-2023.05.2.tar.gz && \
    mkdir 2023.05 && \
    tar -xzf TeamCity.tar.gz -C /teamcity/2023.05 && \
    rm TeamCity.tar.gz