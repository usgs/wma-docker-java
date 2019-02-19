# USGS Water Mission Area Java Docker Base Images

This Docker Image may be extended by USGS WMA Java Docker Images requiring a Java Run-time Environment (JRE).

## Usage
### Extending the Base Image
This image is not intended to be run on its own, rather other images should inherit from this image in order to utilize its functionality. 

#### The Entrypoint Script
This docker image includes an entrypoint script that configures the environment variables for the application. Additionally, this entrypoint allows for your application to be launched via an additional script. The entrypoint script is added to the docker image as `/docker-entrypoint.sh`. 

#### Environment Variables and Secrets
If required, environment variables and secrets are read from up to two directories. These directories should be mounted when running the containers.

1. **COMMON_DATA_DIRECTORY**: Files in this directory are shared across the containers in the cluster.

2. **APPLICATION_DATA_DIRECTORY**: Files in this directory are specific to the application in this container.

#### Executing your Application
The entrypoint script added by this docker image expects your application to add a `/launch-app.sh` script for running the application.
