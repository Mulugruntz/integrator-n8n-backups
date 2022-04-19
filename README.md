# n8n backups #

In our [n8n](https://n8n.io/) (container), there’s a workflow that creates backups, commit and pushes them.
This is the repository that is used for these backups.

And when you build a new image, it pulls from this repo to import workflows into the n8n docker image.

### Where is our n8n setup? ###

It can be found in [our GitHub repository](https://github.com/Mulugruntz/integrator-n8n).

### What base workflow do we have?

#### In `1.json`: Backup workflows & credentials | [FILE](workflows/1.json)

A workflow that backs up all other workflows and credentials. It includes itself.

### Who maintains this repository? ###

The lifecycle of this repository is supposed to be fully automated. 

Only our bot [@Mulugruntz](https://github.com/Mulugruntz) maintains this repository.
