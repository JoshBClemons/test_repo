# TO BUILD: docker build -t test_repo .
# TO TAG: docker tag test_repo jclemons97/test_repo
# TO PUSH: docker push jclemons97/test_repo:latest
# TO RUN: docker run jclemons97/test_repo

# use apt-get with -slim; apk with -alpine
FROM python:3.8.5-alpine

COPY . .

RUN apk update 
RUN \
 apk add --no-cache curl && \
 apk add --no-cache vim

ENTRYPOINT ["python", "client.py"]