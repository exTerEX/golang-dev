# Golang-Docker development container

A Golang development container for [Visual Studio Code](https://code.visualstudio.com/) with [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension. It is a linux environment based on the latest LTS distribution of debian and the image is based on `golang:latest` by Docker. It is installed with [Oh My Bash](https://ohmybash.nntoan.com/).

## Example

To use as development container for your project create, `.devcontainer/devcontainer.json` to project with the content,

```r json
{
    "name": "",
    "image": "exterex/golang-dev",
    "extensions": [
        "golang.go"
    ]
}
```

For configuration of `devcontainer.json` see [code.visualstudio.com](https://code.visualstudio.com/docs/remote/devcontainerjson-reference)

## Build

The image is updated every time the `main` branch of the repository is updated and once a week on a fixed schedule (see [workflows/ci.yml](.github/workflows/ci.yml)).

## License

This repository is distributed under `BSD-3-Clause`. For more information see [LICENSE](LICENSE).
