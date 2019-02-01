FROM openjdk:11-jdk-slim-stretch
LABEL maintainer="gs-w_eto_eb_federal_employees@usgs.gov"

RUN apt update && apt -y upgrade
RUN adduser --disabled-password --gecos "" -u 1000 java
