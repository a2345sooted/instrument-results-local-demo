# Instrument Results – Local Demo

Quick and easy local demo environment for the  
**Instrument Results** application.

It runs the full stack locally using Docker:

- PostgreSQL
- Spring Boot API
- Angular UI

No Java, Node, or database installation is required, **only Docker**.

## Prerequisites

- Docker Desktop (or Docker Engine + Docker Compose)
- Git

## Clone the Repository (Important)

⚠️ **Do not use the GitHub “Download ZIP” or a plain clone button.**  
This repository uses **Git submodules** for the backend and frontend.

Clone it using:

```bash
git clone --recurse-submodules https://github.com/a2345sooted/instrument-results-local-demo.git
```

Change into the dir:

```bash
cd instrument-results-local-demo
```

Create a local env file:

```bash
cp .env.example .env
```

Build and start the full stack:

```bash
docker compose up --build
```

## Access the App

Once everything is running:

- **UI:** http://localhost:4200
- **API:** http://localhost:8080

## Tear Down

```bash
docker compose down
```

If you want to remove data on tear down, use:

```bash
docker compose down -v
```

## What this repo is for:

- Running the full application locally with minimal setup
- Demoing or reviewing the system

Running the full application locally with minimal 

## What this repo is not for:

- Editing backend or frontend code directly
- Managing database migrations manually

Those responsibilities live in the respective submodule repositories.


### Enjoy!

