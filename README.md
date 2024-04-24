# Hello World

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
