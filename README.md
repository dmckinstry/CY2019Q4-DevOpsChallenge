# DevOps Challenge 2019 Q4

## End-to-end challenge using Actions

1.  Prepare the Challenge DevOps project (from a template)
    1.  Grant other users permissions to the project
    1.  Review the work items and plan
1.  Prepare an Azure subscription
    1.  Create a resource group for the challenge in an existing subscription
    1.  Setup appropriate team permissions for the resource group
1.  Prepare a challenge GitHub repo
    1.  Create a public repo on GitHub - *The org/user must have the GitHub Actions preview enabled*
    1.  Grant appropriate permissions to your team
    1.  Connect the GitHub repo to the Azure DevOps challenge project
    1.  Setup branch protections to require PRs and at least on reviewer
    1.  Have two other team members (not the repo owner) test the access and branch protections by updating the README.md file


1.  GitHub security
    1.  Enable security alerts
    1.  Review security alert results
    1.  Enable automatic security fixes
    1.  Review pull requests 

Do we want to force Terraform provisioning of the environment?  Do we have a good starter template?
Should we cause a build action to trigger a deploy action?
Should we do a pipelines with environments?
Should we do deployment slots?
Should we add a CURL test to the deployment?  Other UI tests?
We should probably have a separate manually triggered for deploy to production.
Do we want to do a container push to GPR?

1.  Create an Action workflow to provision Azure
    1. Setup Azure security stuff as appropriate
    1. Figure out security key stuff needed for CLI - need reference
    1. Store key as a GithUB secret in the forked repo
