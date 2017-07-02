FROM splunk/splunk:latest
MAINTAINER vince.sesto@gmail.com

# Set up environment variables
ENV SPLUNK_START_ARGS --accept-license
ENV SPLUNK_USER root

# Copy ui_login to stop the first time login screen
COPY .ui_login /opt/splunk/etc/.ui_login

# Creating a new app
COPY mood_radiator/ /opt/splunk/etc/apps/mood_radiator/

# In case we need it
RUN apt-get update && apt-get install -y vim
