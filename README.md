Dependabot Yarn v4 Dependabot Failure Reproduction
==================================================

The purpose of this repo is to show, with a minimum repo, that Dependabot is running fine on Github, but not with the TingleSoftware Azure Devops Dependabot pipeline.

# Prerequisites

1. `nodejs` (LTS Preferred?)
2. `corepack` enabled
```bash
enable corepack
```
3. latest yarn installed
```bash
yarn set version berry
```

# Usage

## Github

Just pay attention to the Dependabot runner.

## Azure Devops

1. Create Repo in your org in Azure devops
2. In [dependabot-azure-devops.yml](./dependabot-azure-devops.yml), please set `gitHubConnection` correctly
3. create a new pipeline using [dependabot-azure-devops.yml](./dependabot-azure-devops.yml)
4. Run your new pipeline in Azure Devops