# CloudBees Pipeline Templates Example
## Multibranch Pipeline Authentication for a Git Server

This example shows how to add authentication to your Git server repository. The developer will supply the value for the ${repoName} parameter when they create their pipeline job in CloudBees Core.

````
type: MULTIBRANCH
...

multibranch:
  branchSource:
    git:
      repoOwner: myCompany
      repository: ${repoName}
      scanCredentialsId: my-team-github-credentials
````