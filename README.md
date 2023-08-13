# Python Flask - Demo Web Application

This is a simple Python Flask web application. The app provides system information and a realtime monitoring screen with dials showing CPU, memory, IO and process information.

The app has been designed with cloud native demos & containers in mind, in order to provide a real working application for deployment, something more than "hello-world" but with the minimum of pre-reqs. It is not intended as a complete example of a fully functioning architecture or complex software design.

Typical uses would be deployment to Kubernetes, demos of Docker, CI/CD (build pipelines are provided), deployment to cloud (Azure) monitoring, auto-scaling

## Screenshot

![screen](https://user-images.githubusercontent.com/14982936/30533171-db17fccc-9c4f-11e7-8862-eb8c148fedea.png)

# Status

![](https://img.shields.io/github/last-commit/benc-uk/python-demoapp) ![](https://img.shields.io/github/release-date/benc-uk/python-demoapp) ![](https://img.shields.io/github/v/release/benc-uk/python-demoapp) ![](https://img.shields.io/github/commit-activity/y/benc-uk/python-demoapp)

Live instances:

[![](https://img.shields.io/website?label=Hosted%3A%20Azure%20App%20Service&up_message=online&url=https%3A%2F%2Fpython-demoapp.azurewebsites.net%2F)](https://python-demoapp.azurewebsites.net/)  
[![](https://img.shields.io/website?label=Hosted%3A%20Kubernetes&up_message=online&url=https%3A%2F%2Fpython-demoapp.kube.benco.io%2F)](https://python-demoapp.kube.benco.io/)

## Building & Running Locally

### Pre-reqs

- Be using Linux, WSL or MacOS, with bash, make etc
- [Python 3.8+](https://www.python.org/downloads/) - for running locally, linting, running tests etc
- [Docker](https://docs.docker.com/get-docker/) - for running as a container, or image build and push

Clone the project to any directory where you do development work

```
git clone https://github.com/erickmpene/python-demoapp.git
```

# Containers

Public container image is [available on Docker Container Registry](https://hub.docker.com/r/erickmpene/webapp)

Run in a container with:

```bash
docker run --rm -it -p 5000:5000 erickmpene/webapp:v3
```
