# Tekton Examples

## Configuring Your Secret

`kubectl create secret docker-registry regcred --docker-server=https://index.docker.io/v1/ --docker-username=DOCKER_USERNAME --docker-password=DOCKER_PASSWORD --docker-email DOCKER_EMAIL`

## Examples

**[build-spring-api.yml](build-spring-api.yml):** Build the [Spring Boot REST API Demo](https://github.com/BrianMMcClain/spring-boot-api-demo) using [Cloud Native Buildpacks](https://buildpacks.io/) and push it to Docker Hub. Requires the [Buildpack Task](https://github.com/tektoncd/catalog/tree/master/buildpacks) to be to be applied.