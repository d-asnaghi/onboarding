# `git`

## Workflow

`git` is a powerful version control tool that will be used to keep track of collaborative changes to the project.

The following diagram shows how git can be used to develop code following a branching model.

![git workflow](../resources/images/git-workflow.svg)

In the diagram above, there is a `master` branch that always contains clean, ready to ship code.

This branch is fed changes from the `develop` branch, where any feature implementation will live.

A developer will work on the `develop` branch, creating individual `feature` branches where any contributions will be made.

Once the `feature` branch is ready, it will be merged to `develop` trough a **pull request** (which involves a code review)

Once several features have been merged to develop and tested together, the can finally be merged back to the `master` branch to create user facing release.

## Contributions

- Downloading a repo
    `git clone <repo url>`

- Moving to the `develop` branch
    `git checkout develop`

- Creating a `feature` branch
    `git checkout -b <my-feature-brach>`

- Uploading a `feature` branch to the remote
    `git push -u origin <my-feature-branch>`

- Downloading the latest changes for a branch
    `git pull`


## Additional resources
- [Atlassian git workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)