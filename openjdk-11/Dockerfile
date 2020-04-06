FROM openjdk:11.0.6-jre-slim

LABEL maintainer="gs-w_eto_eb_federal_employees@usgs.gov"

ENV USER=java
ENV HOME=/home/$USER

RUN adduser --disabled-password --gecos "" -u 1000 $USER

WORKDIR $HOME
