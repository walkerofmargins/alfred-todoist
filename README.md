# todoist-alfred
A workflow to make API requests to create tasks in Todoist, using alfred

This workflow allows users to make API calls to Todoist, using Alfred, with the primary function being to create new tasks with pre-assigned rules..

For example, for a work project, I might create a workflow that allows me to:

- Type "tdwork" followed by "finish my assignment"
- This workflow will then, using pre-defined rules, create a new task with a pre-defined: priority, language, due date, label and project.
- The outcome could be: "finish my assignment", priority: 3, due date: today at 5pm, project: work, labels: "30 mins"

This allows you to:

- Create an Alfred keyword for each project
- Create an Alfred keyword for each label
- Create an Alfred keyword for each label/project combo
- Create specific language rules for all of the above
- Create due date/time rules for all of the above
- Create priority rules for the above

# Instructions
### 1. Pre-requesites
1. Alfred for MacOS including the Alfred Powerpack required before using: https://www.alfredapp.com/
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

## 7. Configure your first project keyword - Example

In the list filter Configure your projects - There is a placeholder - edit or delete it. 

- Name: Project Name
- Subname: (Whatever you want)
- Arg: Project ID

### There are 6 configurable varibles:

1. content: Leave this as '{query}' - This will be the To Do item content
2. due_lang: Two letter language code - Default is English: https://en.wikipedia.org/wiki/ISO_639-1
3. due_string: Human Defined due string - Default is "today at 5pm" https://get.todoist.help/hc/en-us/articles/205325931-Dates-and-Times
4. label1: Default is blank, but if you'd like to add a labels, you can get a list of the ones you use by typing "labelstodo"
5. priority: Task priority from 1 (normal) to 4 (urgent).
6. project_id: Enter your copied project id from step 1, above

You should now be able to create your first Todoist task using Alfred by launching Alfred and writing 
"todo" followed by your query




