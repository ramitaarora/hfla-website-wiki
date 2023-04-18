Each environment will host a different version of the website. We use GitHub pages as our host, which means that it is impossible for us to host multiple sites off of one repository. Instead, we will use two repositories: a dev repo and a production repo.

## Repositories

### Production: hackforla/website-prod 
- This repo will be a production environment, meaning code here is for a website made specifically with external clients in mind
- Changes will only be moved to this repo after they are viewed on the UAT site and approved

### Development: hackforla/website-dev 
- This environment will have 2 primary branches (UAT and main)
- The main branch will work like our current environment, but instead of updating the site every time a pull request is merged, the changes will only be visible on the UAT website after they are moved to the UAT branch
- The UAT site will be built from the UAT branch so that it is easy for the whole team to review before changes are pushed to production

## Moving changes between environments

### Updating UAT
- A github action can be manually triggered to merge all changes from the main branch into UAT
- The changes can be viewed on the site and if they are approved, can then be sent to production
- [GitHub Action: Merge Branch](https://github.com/marketplace/actions/merge-branch)

### Updating Production
- Once changes to the UAT site have been approved, a github action can be manually triggered to move the changes to the production repo
- This action is triggered from the dev repo
- [GitHub Action: Git Sync](https://github.com/marketplace/actions/git-sync-action)

### How to manually trigger the actions

- Go to the Actions tab in the dev repo
- Under workflows, click on the action you want to run
- Select the `Run workflow` dropdown
- Keep the branch set to main, then click `Run workflow`
- Click `All workflows` to see the status of the action
- It will take a few minutes for the website to update after the action runs

<img width="850" alt="gh-action" src="https://user-images.githubusercontent.com/62186905/136641170-cc1c0abf-1311-492f-a90e-45cfd4ee77fe.png">