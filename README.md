# Hello World

``` json
{
  "service": "devcontainer",
  "dockerComposeFile": "docker-compose.yml",
  "workspaceFolder": "/workspaces/${localWorkspaceFolderBasename}",
  "postCreateCommand": "./post-create.sh",
  "forwardPorts": [8000],
  "features": {
    "ghcr.io/devcontainers/features/docker-outside-of-docker:1": {
        "installDockerBuildx": false
    },
    "ghcr.io/devcontainers/features/php:1": {},
    "ghcr.io/devcontainers/features/sshd:1": {},
    "ghcr.io/devcontainers/features/node:1": {},
    "ghcr.io/devcontainers/features/python:1": {}
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

## refs:

- Doesn't seem updated
  - [](https://notes.alexkehayias.com/running-docker-compose-in-codespaces/)
  - [](https://notes.alexkehayias.com/github-codespaces-is-too-slow-and-expensive-to-replace-local-development/)
- [](https://containers.dev/guide/dockerfile)
- [](https://hub.docker.com/_/microsoft-vscode-devcontainers)
- [images](https://github.com/devcontainers/images/tree/main/src)
- [features](https://github.com/devcontainers/features/tree/main/src)
- [sshd](https://github.com/devcontainers/features/blob/main/src/sshd/install.sh)
- [](https://docs.github.com/en/codespaces/developing-in-a-codespace/rebuilding-the-container-in-a-codespace)
- []()
