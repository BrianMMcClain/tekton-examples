# Tekton Examples

## Configuring Your Secret

`kubectl create secret docker-registry regcred --docker-server=https://index.docker.io/v1/ --docker-username=DOCKER_USERNAME --docker-password=DOCKER_PASSWORD --docker-email DOCKER_EMAIL`

## Examples

- **[hello-task](https://github.com/BrianMMcClain/tekton-examples/blob/master/hello-task.yml):** A bare-bones task that echos "Hello World" to the output logs
- **[kaniko-task](https://github.com/BrianMMcClain/tekton-examples/blob/master/kaniko-task.yml):** Build the [Sinatra Hello World Demo](https://github.com/BrianMMcClain/sinatra-hello-world) using [Kaniko](https://github.com/GoogleContainerTools/kaniko)
- **[cnb-spring-api-demo.yml](https://github.com/BrianMMcClain/tekton-examples/blob/master/cnb-spring-api-demo.yml):** Build the [Spring Boot REST API Demo](https://github.com/BrianMMcClain/spring-boot-api-demo) using [Cloud Native Buildpacks](https://buildpacks.io/) and push it to Docker Hub. Requires the [Buildpack Task](https://github.com/tektoncd/catalog/tree/master/buildpacks) to be to be applied.