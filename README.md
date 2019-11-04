# DevOps Challenge 2019 Q4

## End-to-end challenge using Actions

1.  Prepare the Challenge DevOps project (from a template)
    1.  Grant other users permissions to the project
    1.  Review the work items and plan
    
1.  Prepare an Azure subscription
    1.  Create a resource group for the challenge in an existing subscription
    1.  Setup appropriate team permissions for the resource group
    1.  Create an Azure Web App for Linux using the Node.JS 10 runtime
    1.  TODO: Other resources?
    
1.  Prepare a challenge GitHub repo
    1.  Create a public repo on GitHub
    1.  Grant appropriate permissions to your team
    1.  Connect the GitHub repo to the Azure DevOps challenge project
    1.  Setup branch protections to require PRs and at least on reviewer
    1.  Have two other team members (not the repo owner) test the access and branch protections by updating the README.md file
    
1.  Create a continuous integration workflow using GitHub Actions to verify PRs
    1.  TODO: Provide install/test/... guidance
    1.  Update the GitHub Branch Protection on Master to require this workflow

1.  Secure the application
    1.  Enable security alerts
    1.  Review security alerts (may take a few minutes?)
    1.  Enable automatic security fixes
    1.  Review and implement recommended fixes

1.  Create an Action workflow to provision Azure resources
    1.  Create Infrastructure-As-Code to provision the Azure resources described above. Use your choice of Ansible, ARM templates, Terraform or Pulumi. Commit the files into the deployment folder. 
    1.  Setup Azure security stuff as appropriate and store the key in GitHub secrets
    1.  Set the trigger to filter on changes to the deployment folder

1.  Dockerize the app
    1.  Create a Dockerfile to package the application
    1.  Provision a new Web App for Linux (Containers) against your exisitng app plan
    1.  Update the infrastructure-as-code for your new Web App and verify it in the existing workflow
    1.  Create a workflow to publish the resulting container to the container registry of your choice (GitHub Package Repository, Azure Container Registry, Dockerhub, ...); following the successful push to the container registry, deploy it to the new Web App

# References
- Azure Actions: https://github.com/azure/actions
- Deploy node to web apps: https://github.com/Azure/actions-workflow-samples/blob/master/node.js-webapp-on-azure.yml
- My sample action to provision an Azure Resource Group (with docs)

