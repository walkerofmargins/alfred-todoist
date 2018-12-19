# todoistalfred
A workflow to make API requests Todoist, using alfred

This workflow allows users to make API calls to Todoist, using Alfred. 

# Instructions
## 1. Pre-requesites
Alfred for MacOS required Alfred Powerpack required before using
A Todoist Premium license is required before using

## 2. Download and install workflow
Download the workflow from github
Drag and drop it into Alfred workflows

## 3. Get your bearer token from Todoist 
Navigate to https://todoist.com/prefs/integrations
Scroll down to the bottom for your integration token
Copy it to your clipboard

## 4. Insert your bearer token into your workflow
Within the workflow, navigate to [x] in the top right - Environment Variable
Create an environment variable with the name "bearer" 
Insert the value in your clipboard as the corresponding value

## 5. Grab a list of your projects [IMPORTANT]
Using your alfred shortcut type "projectstodo"
This will copy all of your projects to your clipboard - you will need these to create your own bespoke workflows

## 6. Grab a list of your lables [OPTIONAL]
Using your alfred shortcut type "labelstodo"
This will copy all of your lables to your clipboard - If you use lables, you might want to consider this 

# Configure your first project keyword - Example

1. In your list of project IDs, navigate to the top - where you'll see the project ID for "Inbox" - Copy it
2. Navigate to the "vars" utility in the workflow - Double click it. This is where we will configure the default behaviour for your Inbox
3. Configure your variables

### There are 6 configurable varibles:

content: Leave this as '{query}' - This will be the To Do item content
due_lang: Two letter language code - Default is English: https://en.wikipedia.org/wiki/ISO_639-1
due_string: Human Defined due string - Default is "today at 5pm" https://get.todoist.help/hc/en-us/articles/205325931-Dates-and-Times
label1: Default is blank, but if you'd like to add a labels, you can get a list of the ones you use by typing "labelstodo"
priority: Task priority from 1 (normal) to 4 (urgent).
project_id: Enter your copied project id from step 1, above

You should now be able to create your first Todoist task using Alfred by launching Alfred and writing 
"todo" followed by your query




