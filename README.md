# deploy-workflow

Workflow for deploying Docker Images to Google Cloud Run.

Will update the Terraform repo with the deployed version and notify Slack regarding the deploy status.

## Development

### Releasing

#### Create release

Each release has its own Git *tag*. Do these steps to create a new release:

1. Create the tag: `git tag <version>`
1. Push the tag to origin: `git push origin <version>`


#### Update release

Because the release now is tagged to a specific commit, if you want to update the release, the tag has to be destroyed and re-created:

1. Delete the tag: `git push origin --delete <version>`
1. Delete the local tag `git tag -d <version>`
3. Create the tag again: `git tag <version>`
4. Push the tag to origin: `git push origin <version>`
