# Utility Images
Unless otherwise stated, these images are built at a minimum with ubi8.

These containerfiles can be used to create an image with utilities built in like ansible, some
ansible collections and a few other pip libraries (listed within each repo) to be used to execute
playbooks for openshift deployments and day 2 operations.

| Image | Purpose |
| ----- | ------- |
| ansible | only provides ansible and ansible collections |
| cspUtility | provides ansible, ansible collections, terraform, azure-cli and awscli |