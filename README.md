# Maxa AI - Releases

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

## Architecture

This static website is published to our Kubernetes cluster, using Github actions to build the yarn package, the helm chart and the container image.

Argo CD will then serve the helm chart in a specific namespace.

### Local installation

To run a local instance of the website, follow these steps
1. initialize your local yarn with:
```
$ yarn
```

2. build the static website package:
```
$ yarn build
```
This command generates static content into the `build` directory and can be served using any static contents hosting
service.

3. start the yarn server:
```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without
having to restart the server.

## Deployment

As stated above, deployment will be used with ArgoCD and Kubernetes. Github Actions will only perform the build of our different artifacts.
