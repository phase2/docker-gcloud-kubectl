# Phase2 gcloud-kubectl

> Docker image for using gcloud auth with kubectl. Extends from [Google's alpine image](https://cloud.google.com/sdk/docs/downloads-docker).

This Docker image adds the gke-gcloud-auth-plugin and kubectl to the base `google-cloud-cli:alpine` image.

## Image generation

* To generate new images for the latest google-cloud-cli version:
* * Go to [Google's container registry](https://console.cloud.google.com/gcr/images/google.com:cloudsdktool/global/google-cloud-cli) and find the latest version.
* * Update the `src/Dockerfile` and set the docker image tag to the latest version number: ex `399.0.0-alpine`
* * Commit and tag the main branch with `v` followed by the version number: ex `v399.0.0`
* * Push the udpates and tag upstream.

## Security Reports

Please email outrigger@phase2technology.com with security concerns.

## Maintainers

[![Phase2 Logo](https://s3.amazonaws.com/phase2.public/logos/phase2-logo.png)](https://www.phase2technology.com)