# Issue and Pull Request Management
The purpose of this document is to explain how the BOINC community makes use of GitHub project boards.  Managing issues and pull requests effectively can help contributors and committers see what work needs doing more easily.  They exist to help us answer questions like the following:
- I'm a developer and I'd like to help the project.  What needs doing?
- I've implemented an enhancement or fix.  How do I make sure that someone knows to review it?
- Someone reported a bug on a project forum.  How do I make contributors and committers aware of it?
- What needs to be fixed in this release?

We will use these examples at the end of this document after briefly explaining how the project boards are set up.

The usage of project boards is intended to support the BOINC [development workflow](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md)
# Project Boards
GitHub allows a repository like [BOINC/boinc](https://github.com/BOINC/boinc) to create one or more project boards (also called projects).  BOINC's project boards are high level in nature and cover different components of the overall BOINC system.  At this time there are 8 defined:
- Android
- Client and Manager
- Client Release X.Y
- Governance
- Installation
- Server
- Website and Drupal
- Other

The project boards for BOINC can be seen here: https://github.com/BOINC/boinc/projects

Issues and pull requests can belong to one or more projects as appropriate.
## Project Board Columns
Each project board contains a set of columns that reflect the status of an issue or pull request.  These can be seen by viewing a specific project board.
### Backlog
Issues that are new or haven't been reviewed are put into the backlog column.  This is the default column for issues newly assigned to the project.  They remain in this column until they are discussed and reviewed.

Pull requests are not usually in this column.
### Review
Issues that are undergoing review are moved to this column.  At this point the person that moved it here should be making sure that sufficient information is present in the issue for it to be implemented.  See the [Change Review](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md#11-change-review) section of the development workflow for details.

Pull requests are not usually in this column.
### TODO: Ready to Implement
After the review is complete, then the issue should be moved to the TODO: Ready to Implement column to indicate that it is ready to be implemented.

Pull requests are not usually in this column.
### TODO: Prioritized
This contains the 3-5 most important issues that have been reviewed and are ready to implement.  This column is used to make it easy for someone who is looking to help to find the most important tasks to implement.

Pull requests are not usually in this column.
### Development
Once a developer claims an issue, they should move it to "Development" and assign themselves to the issue and begin work.  It should remain in this status until the developer has finished their work and tested the change.

Pull requests that are in this status are considered work in progress should also have the their title prefixed with [WIP].
### Testing
Once a developer has finished their work and created a pull request for the work, then the issue should be moved to the testing status.

Pull requests that are in this status are ready for reviews by a committer.
### Done
Once a the pull request where the issue was implemented is merged, the issue should be tagged to the release it will be in and then closed.  

Pull request that are closed or merged are moved to this column.
# Examples
## I'm a developer and I'd like to help the project.  What needs doing?
- You want to help the project but you aren't sure what needs doing.  Here is how you find something to contribute:
- Visit the [project boards](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) and decide what part of the project you want to help with
- View the project board for the area that you want to help with and look at the issues in the TODO: Prioritized column to find an issue you can help with.  You can also review the issues in TODO: Ready to Implement if none of the prioritized issues grabs your interest
- Once you have found an issue to work on, review the [Development Workflow](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) and in particular section 2 that explains how to develop and submit your contribution.

If you need help getting started, you can connect with other contributors on the [BOINC development forums](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) or on the [boinc-dev](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) mailing list.
## I've implemented an enhancement or fix.  How do I make sure that someone knows to review it?
If you have followed the [Development Workflow](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) you should now have a pull request open.  You should:
- Assign the pull request to the appropriate project
- Go into that project board and move it to the "testing" column.
- Committers should be periodically checking the boards and notice your pull request and start a review

If no-one is starting a review of your pull request after a few days, please post in the [BOINC development forums](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) or on the [boinc-dev](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md) mailing list to request someone to conduct a review
## Someone reported a bug on a project forum.  How do I make contributors and committers aware of it?
- [Open an issue](https://github.com/BOINC/boinc/issues/new)
- Document what the problem is and how to reproduce it (follow the guidelines in the [Development Workflow](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md))
- Add the issue to the appropriate project board and move it into the "Review" column and discuss it as appropriate
- Once discussion has concluded it can be moved into the appropriate TODO column where it is available to be claimed by a developer
## What needs to be fixed in this client release?
If you want to see the status of the issues and pull requests for a client release, visit the [project boards](https://github.com/BOINC/boinc/projects) and click on the Client Release project board.
# Document Change Process
Changes to this document are proposed by creating a pull request against BOINC policy repository. Approval of the pull request requires a successful consensus vote of the committers as outlined in section 5.1.1 of the Governance document.