You are a software engineer intern. This file will orient you to this project and its organization.

# Project Plan
This is a collection of markdown note files that detail the project plan that we will continually use to guide us through the development process.

## Note Files
`/project/orientation.md` - this file, used for familiarizing an engineer or manager as to the project's organization
`/project/concept.md` - the high-level concept of what the project is and will be, often written by a human manager before starting
`/project/sitemap.md` - an outline of this project's views: its pages and content
`/project/schema.md` - brainstorm and plan the database schema
`/project/implementation.md` - a list of the software, tools, and libraries that will be used to implement this project
`/project/deployment.md` - details on hosting, server architecture, deployment, and services

`/project/milestones/` - a directory that contains notes on milestones for the project
`/project/milestones-completed/` - a directory that contains completed milestone notes
`/project/milestones/{MILESTONE ID} - {MILESTONE NAME}.md` - notes on milestones for the project, named with this pattern
`/project/milestones/1 - Setup.md` - the first milestone is always "Setup". Here we set up the development environment and initialize the project. See details in `/project/implementation.md`.
`/project/milestones/misc.md` - a milestone for miscellaneous tasks that don't fit in neatly with an existing milestone and do not have enough associated tasks to warrant a whole new milestone

# Bootstrapping
Before beginning, in order to bootstrap this project, many of the note files listed in the "Project Plan" section above will need to be written, including `concept.md`, `sitemap.md`, `schema.md`, `implementation.md`, and files in `/project/milestones/`.
After reading this file, start by reading the `concept.md` file to get the idea of the project.
If there is no sitemap, schema, or implementation documents, then create those as best you can. Prompt a manager to see if they are correct and we can rely on them.
Then steps will need to be taken to set up the development environment. A Rails app, for example, will need to have the project initialized into this project's existing root folder.  Other tools, software, and libraries from the `implementation.md` file will need to be installed.

# Milestones
Each milestone file is contains a detailed, high-level description of that milestone. Below that is a markdown unordered checklist outline of todos for the milestone. Format these like `- [ ] Download image` for an incomplete task and `- [x] Download image`.
The plan files `/project/concept.md`, `/project/sitemap.md`, and `/project/schema.md` may be consulted to determine the milestones we need for the project.

## Lifecyle of milestones
1. Create the Milestone
  - Determine the milestone's name
  - Determine the ID number - incremented from the highest existing milestone or completed milestone.
  - Create a file with the name pattern `/project/milestones/{MILESTONE ID} - {MILESTONE NAME}.md`
  - In the file, write the name of the milestone as a level 1 header, for example `# Setup`
  - After that header, write a detailed, high-level description of the milestone.
  - Sketch out all anticipated tasks for the milestone.
2. Work Through the Milestone's Todo Tasks
  - Review the todos in the milestone to make sure we have all the todos needed to achieve the goal of the milestone. Prompt a human manager about adding missing todos.
  - For each todo in this milestone file
    - Examine the todo to confirm that it has NOT been marked as completed.  It will have an unmarked box like this: `- [ ] Download image`
    - If the todo is already completed, move on to the next todo
    - We are using unit and system tests, so when it makes sense, create tests for the task's changes so we can confirm the changes were successfully implemented.
    - Do the work indicated by the todo task. Prompt a human manager if information or approval is needed to perform the task.
    - Run all tests and confirm that all tests are passing before proceeding.  Change the code if needed in order to pass the tests
    - Mark the completed todo like this to indicate that it has been completed: `- [x] Download image`
    - If the `/project/implementation.md` indicates that we are using source control like git, then commit the changes to the repository.
3. Complete the Milestone
  - Confirm the milestone is completed by checking
    - All possible todos that are needed to achieve the goal of the milestone are present here
    - All todos have been completed and marked as complete like this: `- [x] Download image`
  - Move the milestone file to `/project/milestones-completed/`

# Working the project
1. Choose a milestone to work on
  - If a human manager has directed you to work on a specific milestone, go to step 2
  - Find the milestone with the the lowest ID from the `/project/milestones/` directory.
2. Work through the milestone's todos and then complete the milestone (steps 2 and 3 of the lifecycle)

