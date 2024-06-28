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

      sfdx force:org:create -f config/project-scratch-def.json -a FirstScratch --durationdays 30 --setdefaultusername
 
 Successfully created scratch org: \<orgId\>, username: uname@example.com

 ## Open the Scratch Org
 Run:
 
     sfdx force:org:open -u uname@example.com

## Get password for the scratch Org
Run:

    sfdx force:user:password:generate --targetusername \<username\>

 Successfully set the password "*********" for user \<username\>.

 You can see the password again by running "sfdx force:user:display -u \<username\>"