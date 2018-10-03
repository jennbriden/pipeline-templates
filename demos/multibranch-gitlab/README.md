# CloudBees Pipeline Templates Example
## Multibranch Pipeline Authentication for Github.com

This example shows how to add authentication to your Gitlab.com repository. The developer will supply the value for the ${repoName} parameter when they create their pipeline job in CloudBees Core.

````
type: MULTIBRANCH
...

multibranch:
  branchSource:
    gitlab:
      serverUrl: http://www.gitlab.com 
      repoOwner: myCompany
      repository: ${repoName}
      scanCredentialsId: my-team-github-credentials
````