# Development Workflow
The purpose of a development workflow is to make sure that the BOINC platform produces high quality code that solves the problems of its users. As such, the development workflow needs to have checkpoints to allow for the review and discussion of the following questions:

- Should this item be implemented?
- How should this item be implemented?
- Has this item been implemented correctly and is it ready for release?

It is important to note that for the purposes of this workflow, anyone who is submitting a proposal for a change or contributing code is considered a 'contributor'. Even if that person is on the PMC or is a committer, they cannot take the actions of a committer with respect to their own proposals or code changes. This ensures that every feature and piece of code contributed to the project has a least two people who have looked at it. This is a standard practice which improves design and code quality and reduces the chances of bugs and significant flaws making it into the software.

Code produced via this process is expected to be largely free of defects and should be available as a nightly build.

## 1. Proposed Changes
Code changes are made because somebody has a problem that cannot be solved with the current version of this software. This could be because the software is doing something wrong (a bug report) or this could be because the software does not yet do something that somebody needs it to do (feature request).

These changes are documented using [issues](https://github.com/BOINC/boinc/issues) on github. A good issue will clearly define the problem that needs to be solved and how the software is not currently solving that problem. In the case of a bug report, this will include instructions on how to reproduce the issue. In the case of a feature request, it will detail the capabilities that are required in order to solve the stated problem.

A design may or may not be needed for the proposed change. If you are not sure of your approach, or if the change is medium to large sized, especially if it changes the behavior of the application, then you should do a design so that it can be reviewed when it is still easy to make changes. If you proceed without doing a design, you run the risk of having to re-do significant portions of your change should your approach or design be rejected during code review.

Key elements of a design are:

- Details about changes in how users interact with the application
- Details about changes in the behavior of the application and if any defaults will change
- Description of the application changes (this can consist of anything from interaction and class diagrams to pseudocode )
- Database changes
- Steps that users of the software need to do in order to use or tune a new feature

### 1.1 Change Review
Once an issue is defined and created, anyone can review and comment on the issue. In particular, committers are expected to review the issue and make sure that the problem statement is clear. Committers also need to follow the consensus voting process and determine if the issue should be implemented or not. In the event that no voting is done on an issue, the issue remains open until a committer either votes yes or vetoes the issue.

Reviews are expected to examine two things:

- Is the problem that requires a change clearly explained?
- Is the bug reported or change requested something that should be implemented?
- If this change does not have a design, is that a reasonable decision?
- If provided, does the proposed design implement the change effectively and in an easily maintainable way?
- If provided, does the proposed design describe the impacts to existing users of the software (server or client)?

### 1.2 Prioritization
If a change is approved, the issue should be "ready to implement" and should be added to the project board for its respective area (https://github.com/BOINC/boinc/projects). Committers are expected to also prioritize issues and have a small collection of the highest priority issues in the To-Do column of the different project boards. This makes it easy for developers to find work that needs to be done and also helps with facilitation of the overall development process.

## 2. Implementation
All development is done using feature branches as defined in [GitHub Flow](https://guides.github.com/introduction/flow/). BOINC uses the [Fork and Pull Model](https://gist.github.com/Chaser324/ce0505fbed06b947d962) for development (background on this approach can be [read here](https://help.github.com/categories/collaborating-with-issues-and-pull-requests/)). Once you have created your fork, set it up locally, and created a feature branch, then you can begin coding. When you are finished with development you can create a pull request for review.

Make sure to review the [Definition_of_Done_for_Feature_Branches.md](../../blob/master/Definition_of_Done_for_Feature_Branches.md) before starting work so that you are familiar with the expectations of your work.

If you wish to get some early feedback on your changes, then you can create a pull request with the text [WIP] at the start of the title. This indicates to reviewers that you are inviting others to look at your code, but that it should not be merged. Once you are ready for final review and merge into master, then you can remove the [WIP] prefix.

Once the code has been approved it is merged into the master branch.

### 2.1 Code Review
Once a pull request has been created for the implementation of an issue, anyone can review and comment on the changes. Committers need to follow consensus voting and determine if the code change is accepted. Committers should use the [Expectations_of_Code_Review.md](../../blob/master/Expectations_of_Code_Review.md) as a guide to conducting the review.

# Document Change Process
Changes to this document are proposed by creating a pull request against [BOINC policy repository](https://github.com/BOINC/boinc-policy).  Approval of the pull request requires a successful consensus vote of the committers as outlined in section 5.1.1 of the [Governance document](https://github.com/BOINC/boinc-policy/blob/master/Governance.md).
