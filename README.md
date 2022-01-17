# deploy-workflow

Workflow for deploying Docker Images to Google Cloud Run.

Will update the Terraform repo with the deployed version and notify Slack regarding the deploy status.


# Tagging

### Create the tag:

`git tag {version}`. Example `git tag v1`

### Push the tag:

`git push origin {version}`. Example `git push origin v1`

### Deleting a tag

`git push origin --delete {version}`. Example `git push origin --delete v1`
