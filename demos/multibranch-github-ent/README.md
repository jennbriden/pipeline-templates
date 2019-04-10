# CloudBees Pipeline Templates Example
## Multibranch Pipeline Authentication for Github Enterprise

This example shows how to add authentication to Bitbucket.org. The developer will supply the value for the ${repoName} parameter when they create their pipeline job in CloudBees Core, and Pipeline Templates then use the developer's value to replace the placeholder variable in the Jenkinsfile.

````
multibranch:
  branchSource:
    github:
      apiUrl: https://github.beescloud.com/api/v3
      repoOwner: myCompany
      repository: ${repoName}
      scanCredentialsId: my-team-github-credentials
````