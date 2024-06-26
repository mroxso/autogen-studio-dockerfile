# Autogen Studio Docker Image

This repository contains a dockerfile which can be used to build a docker image for the Autogen Studio. The docker image can be used to run the Autogen Studio in a docker container.

## Quickstart (Pre Built Images)

To quickly get up, run the following command in this repository:

```bash
docker compose up -d
```

or

```bash
docker run -it --rm -p 8081:8081 ghcr.io/mroxso/autogenstudio:latest
```

## Building the docker image

To build the docker image, run the following command in the root of this repository:

```bash
docker build -t autogenstudio .
```

## Running the docker image

To run the docker image, run the following command:

```bash
docker run -it --rm -p 8081:8081 autogenstudio -e "OPENAI_API_KEY=your_openai_api_key"
```

The Autogen Studio will be available at http://localhost:8081.
