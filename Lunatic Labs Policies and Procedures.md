# Lunatic-Labs-Policies-and-Procedures

**Table of Contents**

[**Software Development Life Cycle (SDLC)**](#software-development-life-cycle-\(sdlc\))	**[3](#software-development-life-cycle-\(sdlc\))**

   [Requirements Management](#requirements-management)	[3](#requirements-management)

   [Analysis](#analysis)	[3](#analysis)

   [Design](#design)	[3](#design)

   [Coding and Testing](#coding-and-testing)	[4](#coding-and-testing)

   [Code Coverage](#code-coverage)	[5](#code-coverage)

   [Deployment](#deployment)	[5](#deployment)

[**Project Management using Scrum**](#project-management-using-scrum)	**[6](#project-management-using-scrum)**

   [Sprint Planning](#sprint-planning)	[6](#sprint-planning)

   [Daily stand-ups](#daily-stand-ups)	[6](#daily-stand-ups)

   [Sprint Reviews](#sprint-reviews)	[6](#sprint-reviews)

   [Sprint Retrospective](#sprint-retrospective)	[7](#sprint-retrospective)

   [Reporting](#reporting)	[7](#reporting)

   [Velocity](#velocity)	[7](#velocity)

   [Burndown chart](#burndown-chart)	[7](#burndown-chart)

   [Github Project Organization](#jira-project-board)	[7](#jira-project-board)

[**Code management**](#code-management)	**[9](#code-management)**

   [Github](#github)	[9](#github)

   [Branch Format](#branch-format)	[9](#branch-format)

   [Creating a Feature Branch](#creating-a-feature-branch)	[9](#creating-a-feature-branch)

   [Committing](#committing)	[9](#committing)

   [Creating a Pull Request](#creating-a-pull-request)	[10](#creating-a-pull-request)

   [Git Commands](#git-commands)	[10](#git-commands)

   [Setup & Init](#setup-&-init)	[10](#setup-&-init)

   [Stage and Snapshot](#stage-and-snapshot)	[10](#stage-and-snapshot)

   [Branch & Merge](#branch-&-merge)	[10](#branch-&-merge)

[**Code Reviews**](#code-reviews)	**[12](#code-reviews)**

   [Purpose](#purpose)	[12](#purpose)

   [When and what to review](#when-and-what-to-review)	[12](#when-and-what-to-review)

   [Preparation](#preparation)	[12](#preparation)

   [Scribe](#scribe)	[12](#scribe)

   [Format](#format)	[12](#format)

[**Time management**](#time-management)	**[14](#time-management)**

[**Communication expectations**](#communication-expectations)	**[15](#communication-expectations)**

[**Roles and Expectations**](#roles-and-expectations)	**[16](#roles-and-expectations)**

# Software Development Life Cycle (SDLC)

All SDLCs must address how they will deal with the following phases of software development:  Requirements gathering and management, analysis of the requirements, design of the code that will be written, coding, testing the code, and delivery of the system into production.  Once a system is in production, then the team must integrate how the production system will be maintained into its process.  Lunatic Labs will use an Agile methodology known as Scrum for its SDLC.  

## Requirements Management

Scrum uses a backlog to manage requirements.  A User Story represents a requirement in a simple, customer-focused narrative.  User Stories are added to the backlog as new requirements are identified by the customer or the development team.  As User Stories are added to the backlog, they are prioritized by business value or the value they will bring to the development team in learning or building foundational pieces of a system.

## Analysis

Analysis is somewhat informal in Scrum.   During a [Sprint Planning meeting](#sprint-planning), the backlog is prioritized and user stories are selected to be a part of the sprint.  Once the stories are selected, the team breaks the stories down into smaller tasks needed to complete the User Story.  This analysis step transforms the user story from the user's perspective to a software engineering perspective.

## Design

Scrum advocates “design by discovery” or “emergent design,” but Scrum also assumes a level of experience that most students do not yet possess.  Therefore, Lunatic Labs will rely on more formal design approaches to make the design step more explicit.  Many developers like to use the Unified Modeling Language (UML) to produce diagrams that help to communicate design decisions.  

UML 2.0 defines thirteen types of diagrams, divided into three categories: Six diagram types represent static application structure; three represent general types of behavior; and four represent different aspects of interactions:

* **Structure Diagrams** include the Class Diagram, Object Diagram, Component Diagram, Composite Structure Diagram, Package Diagram, and Deployment Diagram.   
* **Behavior Diagrams** include the Use Case Diagram (used by some methodologies during requirements gathering); Activity Diagram, and State Machine Diagram.   
* **Interaction Diagrams,** all derived from the more general Behavior Diagram, include the Sequence Diagram, Communication Diagram, Timing Diagram, and Interaction Overview Diagram. (Milutinovich and Bondareva)

The following design activities should be incorporated into your process as appropriate:

* developing a user interface design using mock-ups or tools specifically created for designing UI’s, like Figma  
* using a modeling tool like UML to   
  * produce an architecture design that helps communicate the structure of the system to the entire team   
  * model classes and their interactions in the system  
  * Illustrate how your system interacts with other systems using an Interaction Overview Diagram

## Coding and Testing

Automated Unit tests should be written at the same time as the production code, whether you choose to write the tests before or after the production code.

Code should be written in short increments.  If you add small amounts of production and test code and your system breaks, then you know exactly where the problem was created.  If you write several pages worth of code and your system breaks, your debugging becomes much more complicated as you try to figure out where the bug was introduced into the code.

For integration and system testing, code should be deployed into an environment specifically used for testing.  

### Code Coverage

For Lunatic Labs, our standard will be to have at least 80% Code Coverage.  The ideal would be to always have 100% code coverage, but this is practically impossible to achieve.  

## Deployment

TBD.

# Project Management using Scrum

## Sprint Planning

Per the Scrum Guide, Sprint Planning addresses the following topics (Schwaber and Sutherland):

1. Why is this Sprint valuable?  
   1. Agile emphasizes delivering business value with each sprint.  The team should understand what business value they will deliver with this sprint.  
2. What can be Done in this Sprint?  
   1. The user stories in the product backlog should already have story points assigned to them and should already be prioritized.  Existing teams will know what their [Velocity](#velocity) is.  User stories are added to the sprint based on their priority and how many of them can be accomplished based on the team’s velocity.  For instance, if a team has a velocity of 15, and the highest prioritized user stories have story points of 2, 3, 5, 1, 3, and 5, the team can commit to the first five stories adding up to 14 points.    
3. How will the chosen work get done?  
   1. In this step, the team will decompose each User Story into smaller tasks and estimate them by hours.  They will also assess whether they need further input from the Customer or a technical expert to successfully deliver the user story.

In addition to these 3 items, the team should set goals for the sprint and address any known obstacles for the sprint.  

## Daily stand-ups

The daily stand-up should last no more than 15 minutes.  Each team member answers 3 questions:

1. What did you do yesterday?  
2. What will you do today?  
3. Is anything blocking your progress?

These meetings should focus on the requirements and the progress made on the task assigned.  The team should not engage in trying to problem solve during the meeting, especially if it is a technical roadblock.  If someone is experiencing a blockage, a subsequent meeting should be scheduled with the people who can help remove the blockage, whether it be a question about how the functionality should work or if they need technical assistance.

## Sprint Reviews

Typically, a sprint review entails a presentation of the work accomplished during the sprint, but in addition, the team assesses the Product Backlog (see [Github Project Organization](#jira-project-board)) to see if user stories have been added, and if so, to assign story points and prioritize each new story.  The Customer may wish to change the priorities of existing stories so they will be developed sooner.  When this occurs, the user stories should be reordered in the Github Project kanban board to reflect the new prioritization.

## Sprint Retrospective

The Sprint Retrospective meeting should occur after the Sprint Review is completed and before the next sprint begins.  While the Sprint Review focuses on the user stories planned and delivered, the Sprint Retrospective focuses on “how the last Sprint went with regards to individuals, interactions, processes, tools, and their Definition of Done. “  (Schwaber and Sutherland)  Typically, the team answers three questions:

1. What work has been done well in this sprint?  
2. What work hasn’t been done well?  
3. What should we start doing to improve?

Definition of Done is related to how teams manage their project boards.  Refer to [Github Project Organization](#jira-project-board) for more information.

Team members should remember that the purpose of the sprint retrospective is not to assign blame or penalize anyone.  It is focused on improving performance in the future.  

## Reporting

### Velocity

Velocity is a measure of a team’s rate of progress.  It is calculated by summing the number of story points assigned to each user story that the team completed during the iteration.  (Cohn 38\)  

### Burndown chart

TODO

## Jira Project Board

Teams should use the Github Project feature to communicate the team’s progress.  At a minimum, it should have the following columns: User Stories, Todo, In Progress, In Review, Done.  Here is an example of the columns:  
![][image1]

The first column should contain all of the User Stories that have been identified, and the stories should be in prioritized order.  When a new User Story is identified, it should be added to the bottom of the column.  User Stories are reprioritized at the beginning of each Sprint Planning Meeting.

When stories are selected to be part of a Sprint during the Sprint Planning Meeting, they should be broken down into smaller tasks or issues and added to the Todo column.  Each smaller task should have an abbreviation in its description that links it back to a User Story.  Once a task is assigned to an individual, it should be moved into the In Progress column.  

Once an individual has completed their task, a Pull Request should be created and the item should be moved to In Review.  Code should then go through a [Code Review](https://docs.google.com/document/u/0/d/1sXHGnpG732YWbyXVmWRHCo6h9gVe1PBCAZRwSWdtw80/edit).  The project lead and/or technical lead should review the code to ensure that it meets coding standards and has adequate code coverage.  If the code is approved, the Pull Request should be merged and the issue should be moved to Closed.  If the code does not pass the code review, the item should be moved back to In Progress until it passes the code review.

# 

# Code management

## Github

### Branch Format

The project is split up between the prod, test, dev, and various feature branches.

* The prod branch is the LIVE production site that anyone can access and will hold the major version releases of the product.  
* The test branch contains the code pushed to our testing environment, where we will test our completed tickets for stability before we push to production.  
* Feature branches are merged to dev for inclusion in other developers’ local development environments.  
* There will be a feature branch for every issue/ticket and in these branches, we will develop different features and elements that we want to add to the product.

### Creating a Feature Branch

A user is able to create a feature branch right from an issue posted as a ticket in the GitHub issues tab.

* Go to the page of the repository you're working on.  
* Click on the Issues tab to open up a page listing all the issues in your repository.  
* Here you can select your issue. You can filter by Assignee for convenience.  
* You can also reach the specific issue page by clicking on the Projects tab on the main repository page and then the specific project. Here all the issue tickets are sorted by Backlog, Todo, In Progress, In Review, and Done. You can then click on your specific issue ticket there.  
* On the specific issue page, you can click on Create a branch under Development on the right-hand margin.  
* From there you can pick a branch name and the repository destination.

### Committing

Developers should commit their code early and often.  Any time a piece of code is completed (i.e., a new function or new variables are added, a new call to another piece of code is added, etc.), that should trigger the developer to commit their code.  

### Creating a Pull Request

Before creating a Pull Request, the developer needs to pull any changes in the dev branch to their local git repository and resolve any merge conflicts.  Once a feature is completed we will create a pull request to review the code before we merge it into the dev branch.

* Go to the page of the repository you're working on.  
* Click on the Pull Requests tab to see all pull requests for the project.  
* Click on the button towards the right that says New pull request.  
* Use the compare dropdown menu to select the feature branch you'd like to merge and the base dropdown to select the branch you'd like to merge into.  
* Add a title and description for your pull request before clicking Create pull request. *Note*: It is good practice to move the position of your ticket in the Projects page when its status changes. For example, when you are currently working on it, move it to In Progress, or when you've submitted a pull request for it, move it to In Review.

### Git Commands

#### Setup & Init

* git init \- initialize an existing directory as a Git repository.  
* git clone \[url\] \- retrieve an entire repository from a hosted location via URL.

#### Stage and Snapshot

* git status \- show modified files in working directory, staged for your next commit.  
* git add \[file\] \- add a file as it looks now to your next commit(stage).  
* git reset \[file\] \- unstage a file while retaining the changes in working directory.  
* git diff \- diff of what is changed but not staged.  
* git diff \--staged \- diff of what is staged but not yet committed.  
* git commit \-m "\[descriptive message\]" \- commit your staged content as a new commit snapshot.

#### Branch & Merge

* git branch \- list your branches, a \* will appear next to the currently active branch.  
* git branch \[branch-name\] \- create a new branch at the current commit.  
* git checkout \- switch to another branch and check it out in your working directory.  
* git merge \[branch\] \- merge the specified branch's history into the current one.  
* git log \- show all commits in the current branch's history.

# [6 best practices review PRs Github](https://blog.mergify.com/6-best-practices-to-review-pull-requests-in-github/)

# Code Reviews

## Purpose

Code reviews can service a number of goals but all of them can be grouped into two broad categories. The technical category is to improve the code base. While [Linus’ Law](https://en.wikipedia.org/wiki/Linus%27s_law) (given enough eyeballs, all bugs are shallow) may not be technically true, evidence definitely indicates that reviewing code is much better than the alternative. The second category is about improving the team or the project as a whole. These goals may even be considered incidental benefits. In any case, these benefits accrue because knowledge is distributed among the team, which reduces risk and improves cohesion. 

## When and what to review

Each code review should have a well-defined scope. A mature development process typically requires all code changes to be reviewed and approved before they are committed to the main branch of the project source repository. In this circumstance, commits should be kept small enough to allow all changes to be reviewed in one sitting. This may necessitate breaking changes into several steps, which is a symptom of successful development. However, if your development process is not yet mature it is not unreasonable to choose a single module or source file to be reviewed.

## Preparation

* Select the changes or modules to be reviewed.  
* Cleanup your code, compile, run tests, etc. *before* the review.  
* Choose 1-3 appropriate goals to concentrate on.  
* Choose 1-5 other developers to participate.  
* Schedule a block of uninterrupted time available for everyone.

## Scribe

Choose one of the participants to be the official scribe. This provides an artifact to capture the work product and ensures all suggestions are recorded. Remember one of the goals is to improve the development process. It is common during code reviews to recognize a deficiency in a team's process. The scribe should make a note of these so they can be addressed at the next team-wide meeting or by the project lead. If there are many other developers, the scribe may not be an active participant since their time will be filled with making notes.

## Format

The author of the code will “host” the meeting and begin by describing the code under consideration and formally asking the participants to provide constructive feedback. This is also a good time to emphasize any specific goal(s) this review should concentrate on. The scribe should make a note of any specific goals.

Before reviewing individual lines or functions, the group should determine where the code stands with regard to the following attributes, and the scribe should record the results.

* Conformance to the project coding standard  
* Complexity  
* History (for example: new, legacy, active development, refactored, etc.)

The author should describe each section of the code in some appropriate order (bottom-up, or top-down, or order of processing, or some other logical sequence) so the other participants understand both the desired outcome and the implementation. Stop after each section so participants can ask questions or raise concerns. All of the following dimensions of the code should be considered if they apply. Some may be more appropriate to discuss once all the code has been described by the author.

* Correctness (Is the code correct? Is the code complete?)  
* Clarity/maintainability (Is the code as simple as possible? Does it repeat itself?)  
* Architecture  
* Security  
* Test coverage (Are all edges tests? Are all code paths executed?)  
* Optimization/performance

# 

# Time management

Time should be tracked against an issue in Jira.

# 

# Communication expectations

# 

# Roles and Expectations

Works Cited  
Milutinovich, Jovana, and Kate Bondareva. “What is UML | Unified Modeling Language.” *UML.org*, https://www.uml.org/what-is-uml.htm. Accessed 3 January 2023\.  
Schwaber, Ken, and Jeff Sutherland. “The Scrum Guide.” *The Scrum Guide*, https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-US.pdf\#zoom=100. Accessed 3 January 2023\.  


[image1]: <data:image/png;base64,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>
