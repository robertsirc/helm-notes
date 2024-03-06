# Helm Notes

## Introductions

This is a repo on the notes I am taking to contribute to the helm/helm project.

## Development Environment

Adding a line in the helm/helm .gitignore to ignore `.devcontainer/` so I can run my go in a container.

The `devcontainer/devcontainer.json` file should look like this:

``` json
{
    "name": "golang:1.21",
    "image": "registry.suse.com/bci/golang:1.21",
    "forwardPorts": [ 3000 ],
    "customizations": {
        "vscode": {
          "settings": {},
          "extensions": ["golang.Go", "766b.go-outliner","premparihar.gotestexplorer"]
        }
      }
}
```
