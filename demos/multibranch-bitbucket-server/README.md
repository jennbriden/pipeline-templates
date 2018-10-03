# CloudBees Pipeline Templates Example
## Multibranch Pipeline Authentication for Bitbucket.org

This example shows how to add authentication to your Bitbucket.org server. The developer will supply the value for the ${repoName} parameter when they create their pipeline job in CloudBees Core.

````
type: MULTIBRANCH
...

multibranch:
  branchSource:
    bitBucketServer:
      serverUrl: https://bitbucket.beescloud.com
      repoOwner: myCompany
      repository: ${repoName}
      scanCredentialsId: my-team-bitbucket-org-credentials
````