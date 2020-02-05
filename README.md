# git-pr-release in GitHub Actions

Sample of [git-pr-release](https://github.com/motemen/git-pr-release) in GitHub Actions.

## Flow
1. Create `release` branch from `develop` branch
1. Push `release` branch to GitHub
1. Automaticary create pull request to `master` branch by GitHub Actions
1. Rename pull request title to be contain release version
1. Merge pull request
1. Automaticary add git tag extacted from pull request title by GitHub Actions

## Specification
[git-flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) based branch management.

Release pull request title must be contain semantic version number.
(ex. `v1.0.0`, `Version 1.0.0`, `Release 1.0.0`)
