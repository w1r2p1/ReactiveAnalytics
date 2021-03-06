# Build Reactive Analytics locally with docker containers

The following information shows how to run Reactive Analytics with Docker.

## Pre-requisites

- [Docker (Including Docker-Compose)](https://docs.docker.com/install/)

## Before starting:

The module "native" is not supported yet in this project to dockerize.

## Build

Server and client code have their own specific Dockerfiles. It is built by using a single docker-compose file that each creates each image.

**(1) Building and running the project**

Go to a terminal and change your current context to the root of the project. You will notice that you are in the root of the project when you can see the "docker-compose.yml" file.

Run `docker-compose up`

This will build the image if not built and run the application. If there are no issues, you will see a stack of messages like the following:

```
reactive-analytics-localbuild | @adaptive-insights/server: published MARKET_UPDATE.DIA with price 254.26
reactive-analytics-localbuild | @adaptive-insights/server: published MARKET_UPDATE.SPY with price 281.56
reactive-analytics-localbuild | @adaptive-insights/server: published MARKET_UPDATE.IWM with price 165.58
```

**(2) Browsing the application**

By default, the client is running in port 3000. To browse the application, open your preferred browser and type:

`localhost:3000`

You should see now Reactive Analytics running.
