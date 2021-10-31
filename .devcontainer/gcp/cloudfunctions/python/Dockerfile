# Base Image
FROM python:3.9-buster

# labels
LABEL version="1.0"

# latest environment
RUN apt-get update

WORKDIR /usr

# setting launch.json
RUN mkdir .vscode
COPY  ./gcp/cloudfunctions/python/_.vscode .vscode

# installing liblaries
RUN pip3 install \
    google-auth \
    google-cloud-core \
    google-cloud-firestore \
    google-cloud-logging \
    google-cloud-pubsub \
    google-cloud-storage \
    functions-framework \
    flask