# SAMPLE

This is a sample only

## `Pre-requisite`

```
* AWS Account
* Azure Subscriptionm
```

### `How the do`

Only main branch should exist on the repo, in order to make changes a feature/bugfix needs to be checked out from the main branch.

The updates made to the feature/bugfix branch will trigger API calls to the dev workspace from the dev stage in terraform enterprise by deafault. Once you are satisfied with your code and its tested on the dev environment, raise a MR to main branch.

Once the MR is approved and is merged to main branch it automatically triggers a run of test stage which will make API calls to the tst worksapce in terraform enterprise.

The deployment in prd is a manual trigger.


Important notes
```
* No direct pushes to main branch
* checked out branch name should always start with feature or bugfix
```

### `How to use`

Create a project in your own application/project space and use this project's content.
