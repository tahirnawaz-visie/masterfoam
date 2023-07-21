# MasterFoam

## Setup
1. `shopify login --store visie-dev.myshopify.com`

## Development
1. Run
	
	`shopify theme serve --theme cloned-theme-id`

2. Create a feature branch from master
	
	`git checkout -b task/Jira-ticket-no`

3. Develop and test the functionality on “local” (Virtual Clone) theme.
4. Send a PR to base branch staging
5. Once the PR is reviewed, move the code to the LIVE THEME on the Staging store and pass the task for testing to QA Analyst. 
6. Once QA and UAT are done and ready to Deploy, get ready to merge the local branch with master.

    `git checkout master`<br>
    `git pull origin master`<br>
    `git merge feature-branch`

7. Deploy to live theme (Merge the feature branch to master). 

    `git push origin master`

