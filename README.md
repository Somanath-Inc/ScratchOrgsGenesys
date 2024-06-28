# Scratch Org Deployment

## Enable Dev Hub in your org.
    ### To enable go to Setup > Dev Hub > Enable Dev Hub
    ### Once enabled you cannot disable it
## Run the command `sf org login web -d -a DevHub` in terminal
## Allow Prompt to access SF CLI
## Run `sfdx force:org:create -f config/project-scratch-def.json -a FirstScratch`
## Successfully created scratch org: <OrgId>, username: uname@example.com
## Open the Org using `sfdx force:org:open -u uname@example.com`