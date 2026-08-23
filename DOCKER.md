# Docker Setup Guide

This guide explains how to build and run the 9router application using Docker.

## Prerequisites

- Docker installed on your system
- Docker Compose (optional, for multi-container setup)

## Building the Docker Image

```bash
docker build -t 9router:latest .
```

## Running the Container

```bash
docker run -p 3000:3000 --env-file .env 9router:latest
```

## Environment Variables

Create a `.env` file based on `.env.example` with your configuration.

## Docker Compose (Optional)

For a complete stack with database:

```bash
docker-compose up -d
```

## Stopping the Container

```bash
docker stop <container_id>
```

## Viewing Logs

```bash
docker logs <container_id>
```
