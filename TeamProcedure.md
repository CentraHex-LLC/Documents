# Overview

Modifying the code in a shared repository requires several steps to be followed. The goal of this workflow is to make more team members aware of significant changes, reduce the chance of bugs being introduced into the repository, and to increase the transparency of progress on various tasks.

## Workflow

The standard workflow is as follows.

1. A task is created within the teams management tool (clickup, azure, github, etc.).
2. A branch is created with the same name ('Some Task' becomes 'Some-Task') from the relevant branch (usually main).
3. Change are made to the branch and commited roughly daily.
4. Once the branch has completed the task, a pull request is made with at least 1 reviewer.
5. Following review approval, the code is merged into the main branch.
6. Finally, the branch is deleted.

### Branches

Branches should be named after the task they are meant to solve. Changes unrelated to the task at hand should be avoided, but minor bug fixes will be inevitable. Finally, branches should not live past the end of a task; otherwise, branches can accumulate and be a mild nuisence.

### Commits

As we will use the squash merge strategy commit names and contents are not critical. However, it is extremely helpful for reviewers to package commits logically and with names that quickly describe their purpose. The most important aspect of commits is that the code is checked in regularly (daily), so that no code sits in local memory for too long. This habit also makes it easy for other team members to spot changes.

### Pull Requests

Pull requests can be created at any point during the lifetime of a branch. The primary purpose of a pull request is to create a forum for developers to review and comment on code changes as they occur. Once a pull request has reached a state that is statisfactory for all reviwers, it can be merged into main. Generally, the squashed commit mode is prefered, and the merge should have a very useful/descriptive commit name. This is to allow the pull request's merge to have a meaningful name and content while regular commits are held to a lower standard (encouraging frequent commits).
