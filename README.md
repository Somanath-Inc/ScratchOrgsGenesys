# Scratch Org Deployment

## Enable Dev Hub in your org.
    To enable go to Setup > Dev Hub > Enable Dev Hub
    Once enabled you cannot disable it
## Authorise DevHub in VS Code
Run:

     sf org login web -d -a DevHub
 
 Allow Prompt to access SF CLI

## Create Scratch Org
Run:

      sf org create scratch --definition-file config/project-scratch-def.json --no-namespace --duration-days 30 --alias MyScratchOrg --set-default --target-dev-hub ScratchOrg
 
 Successfully created scratch org: \<orgId\>, username: uname@example.com

 ## Open the Scratch Org
 Run:
 
     sf org open -u uname@example.com

## Get password for the scratch Org
Run:

    sf org generate password --target-org <username-or-alias>

 Successfully set the password "*********" for user \<username\>.

 You can see the password again by running `sf org display user -o <username>`
