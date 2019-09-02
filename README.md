# workshop-dev-jcasc
JCasC for Workshop Team Masters.

## Unique JCasC Yaml Per Team Master
While the majority of Team Masters for workshops will utilize the same JCasC configuration there will be some long running and/or example Team Masters that require slightly different configuration. There is currently no inheritance mechanism built into JCasc ([see this issue for some details](https://github.com/jenkinsci/configuration-as-code-plugin/issues/10). 

The current recommendation is to manage a based/default JCasC in a shared repo and have individual Teams that need modified/addtional config create a custom branch from the default branch, and then update the Team Master to get its JCasC config from their Team specific branch. To get upstream changes, you will just need to merge the default branch with the Team specific branch.

>NOTE: The branch name needs to be the same name as the Team Master name.
