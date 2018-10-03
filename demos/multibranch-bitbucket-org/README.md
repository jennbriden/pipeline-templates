# CloudBees Pipeline Templates Example
## Multibranch Pipeline Authentication for Bitbucket Server

This example shows how to add authentication to your Bitbucket server. The developer will supply the value for the ${repoName} parameter when they create their pipeline job in CloudBees Core.

````
type: MULTIBRANCH
...

multibranch:
  branchSource:
    bitBucketOrg:
      serverUrl: https://bitbucket.org
      repoOwner: myCompany
      repository: ${repoName}
      scanCredentialsId: my-team-bitbucket-org-credentials
````