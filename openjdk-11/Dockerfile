FROM ubuntu:18.04
LABEL maintainer="gs-w_eto_eb_federal_employees@usgs.gov"

RUN apt update && apt -y upgrade
RUN apt install -y openjdk-11-jdk
RUN adduser --disabled-password --gecos "" -u 1000 java
