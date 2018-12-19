# todoistalfred
A workflow to make API requests Todoist, using alfred

This workflow allows users to make API calls to Todoist, using Alfred. 

# Instructions
### 1. Pre-requesites
1. Alfred for MacOS required Alfred Powerpack required before using: https://www.alfredapp.com/
2. A Todoist Premium license is required before using: https://todoist.com/r/andy_wingrave_errvgl

### 2. Download and install workflow
1. Download the workflow from github
2. Drag and drop it into Alfred workflows

### 3. Get your bearer token from Todoist 
1. Navigate to https://todoist.com/prefs/integrations
2. Scroll down to the bottom for your integration token
3. Copy it to your clipboard

### 4. Insert your bearer token into your workflow
1. Within the workflow, navigate to [x] in the top right - Environment Variable
2. Create an environment variable with the name "bearer" 
3. Insert the value in your clipboard as the corresponding value

### 5. Grab a list of your projects [IMPORTANT]
1. Using your alfred shortcut type "projectstodo"
2. This will copy all of your projects to your clipboard - you will need these to create your own bespoke workflows

### 6. Grab a list of your lables [OPTIONAL]
1. Using your alfred shortcut type "labelstodo"
2. This will copy all of your lables to your clipboard - If you use lables, you might want to consider this 

## Configure your first project keyword - Example

1. In your list of project IDs, navigate to the top - where you'll see the project ID for "Inbox" - Copy it
2. Navigate to the "vars" utility in the workflow - Double click it. This is where we will configure the default behaviour for your Inbox
3. Configure your variables

### There are 6 configurable varibles:

1. content: Leave this as '{query}' - This will be the To Do item content
2. due_lang: Two letter language code - Default is English: https://en.wikipedia.org/wiki/ISO_639-1
3. due_string: Human Defined due string - Default is "today at 5pm" https://get.todoist.help/hc/en-us/articles/205325931-Dates-and-Times
4. label1: Default is blank, but if you'd like to add a labels, you can get a list of the ones you use by typing "labelstodo"
5. priority: Task priority from 1 (normal) to 4 (urgent).
6. project_id: Enter your copied project id from step 1, above

You should now be able to create your first Todoist task using Alfred by launching Alfred and writing 
"todo" followed by your query




