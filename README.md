# Hello World

``` json
{
  "dockerComposeFile": "docker-compose.yml",
  "service": "devcontainer",
  "workspaceFolder": "/workspaces/${localWorkspaceFolderBasename}",
  "features": {
    "ghcr.io/devcontainers/features/sshd:1": {},
    "ghcr.io/devcontainers/features/php:1": {},
    "ghcr.io/devcontainers/features/python:1": {}
    "ghcr.io/devcontainers/features/node:1": {}
  }
}
```

``` json
{
  "image": "mcr.microsoft.com/devcontainers/base:alpine",
  "features": {
    "ghcr.io/devcontainers/features/sshd:1": {
      "version": "latest"
    }
  }
}
```

``` json
{
  "build": { "dockerfile": "Dockerfile" },
  "features": {
    "ghcr.io/devcontainers/features/sshd:1": {
      "version": "latest"
    }
  }
}
```
