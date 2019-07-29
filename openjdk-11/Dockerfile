FROM openjdk:11.0.4-jre-slim

LABEL maintainer="gs-w_eto_eb_federal_employees@usgs.gov"

ENV USER=java
ENV HOME=/home/$USER

RUN adduser --disabled-password --gecos "" -u 1000 $USER

WORKDIR $HOME

COPY --chown=1000:1000 docker-entrypoint.sh docker-entrypoint.sh

RUN chmod +x docker-entrypoint.sh

ENTRYPOINT ["./docker-entrypoint.sh"]
