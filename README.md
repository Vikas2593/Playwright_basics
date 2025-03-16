**Playwright Readme to run this project

How to Integrate the GitHub Actions**
1. Create a github Repo
2. Push your all code into it
3. Now create a folder .github/workflows
4. Now create file inside with any name [for ex. playwright.yml]
5. Add the code in the file from [ https://playwright.dev/docs/ci-intro ] , Setting up GitHub Actions
6. Make the changes accordingly in the actions [like in this repo we are running it only a user push the code this will get executed]
   
**How to run this in the current repo**
1. Take a clone of this repo
2. Make any small change
3. Push it in the repo
4. Under "Actions" you will the github action is running all the tests

**How to integrate it with jenkins **
Before Steps
1. Under Manage Jenkins -> Tools -> Add local git.exe path, Add Nodejs path 
2. Under Manage Jenkins -> Plugins -> Install "NodeJs" plugin

Now Configuring Job
1. Configure Jenkins once
2. Now create a new freestyle project
3. In GitHub project provide project Url
4. Under "Source Code Management" provide the git url [ credentials required if it is a private repo ]
5. Under "Build Steps", Select "Execute Windows batch command" and then provide command "npm install playwright && npm install && npm run test"

**How to run the tests on Docket Image in Local**

****How to run it directly on Docker Server**
