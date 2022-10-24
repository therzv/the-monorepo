# Turborepo starter
This is an official Yarn v1 starter turborepo.


### Description of the problem and solution
- This is monorepo and i still dont have any deep experience handling monorepo 

- I create two Jenkinsfile for web service and docs service
- I create two helm chart for web service and docs service
- This Jenkinsfile stage are follows
  * triggered by changes on specific branch for spesific service
  * clone the code repository
  * build the docker image
  * push image to registry
  * deploy the changes to kubernetes cluster by installing helm chart


### The reasoning behind your technical choices, including architecture.
- From my expericence, handling containerized application is better with container orchestaration tools
  in this case, i choose Kubernetes

### Trade-offs you might have made, anything you left out, or what you might do
- The Dockerfile i made is not tested yet, and i believe we still improve that Dockerfile
  (i put Dockerfile inside `web` and `docs` directory)
- The Jenkins pipeline still handle CI/CD. Best practice for this is separating CI and CD process.
  Might be Jenkins for CI and Argo for CD.


### differently if you were to spend additional time on the project.



### Useful Links

Learn more about the power of Turborepo:

- [Pipelines](https://turborepo.org/docs/core-concepts/pipelines)
- [Caching](https://turborepo.org/docs/core-concepts/caching)
- [Remote Caching](https://turborepo.org/docs/core-concepts/remote-caching)
- [Scoped Tasks](https://turborepo.org/docs/core-concepts/scopes)
- [Configuration Options](https://turborepo.org/docs/reference/configuration)
- [CLI Usage](https://turborepo.org/docs/reference/command-line-reference)