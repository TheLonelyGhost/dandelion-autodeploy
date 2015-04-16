Dandelion Autodeployment
========================

This automatic deployment assumes you're using a [git-flow](https://github.com/nvie/gitflow) branching model, with `master`, `release/*`, and `development` branches.

## Installation

Copy the contents of the hooks folder to the hooks folder of your git repo (`$PROJECT_ROOT/.git/hooks`)

Install [dandelion](https://github.com/scttnlsn/dandelion) as per docs specified

Set configuration for each environment with `git config` when inside the repository

```
git config deployment.configs.production '/some/path/to/dandelion-production-*.yml'
git config deployment.configs.staging '/some/other/path/dandelion-staging.yml'
git config deployment.configs.development '/some/final/path/to/dandelion-development.yml'
```
