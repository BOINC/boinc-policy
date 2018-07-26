# Issue Management Process
The [Development Workflow](Development_Workflow) document describes the concept by which changes are proposed, reviewed, and prioritized. This document expands on that specifically by defining the standard practices used by BOINC community within the Github issue tracking system.

## 1. Creating Issues
Whether submitting a new issue as a bug report or a feature request, the submission should contain the same general information and will follow the same process. The information to include in any new issue would be:
- a title
- a description
- appropriate labels to indicate the BOINC components that the issue affects (these labels are prefixed by "C: ", e.g. "C: Manager" for the BOINC manager desktop software, or "C: Server - Validator" for the validator component of the BOINC server)

The assignee should only be set when someone has taken ownership of the issue, as issues without an assignee will show up in a list of issues waiting for someone to begin work on them.

### 1.1 Issue Review
Issues should be reviewed prior to development beginning on them. Other members on the BOINC community should look for issues that have not been reviewed and determine, if they are able, whether an issue is suitable for development now, in the future, or not at all. The following labels determine the review status:
- Verified: a good candidate for current development
- Discussion Needed: bring up on the BOINC Contributors call for discussion
- Parked: likely to be a candidate for development in the future, but not now

Importantly, if an issue is not ever likely to be a candidate for development, it should be given a proper explanation and then be closed to prevent the backlog of issues from being overwhelmed in time.

### 1.2 Milestones
Milestones are used for organizing BOINC client and server releases. Only the release manager for a BOINC client or server release should add issues to a milestone (conversely, any pull request being merged into the master branch should be added to the milestone for the next release branch that has not been cut).

### 1.3 Assignees
The assignee of an issue indicates who has taken ownership of it and is responsible for seeing that it is carried to completion. Issues should not be arbitrarily assigned to users, as what is most important is willingness to work on the task.

Any unassigned issues can be found using "no:assignee" in the issue search filter, which is valuable for developers looking for tasks that need to be done. For this reason, a user who is the assignee for an issue but is not willing to continue working on it should clear out the assignee field so that another developer can pick up the task (any final comments should also be made at this time to aid in the transition).

## 2. Use Cases

### 2.1 New Contributor
A user looking to make first contributions to the BOINC community can use the "good first issue" label to find a list of issues that the community has deemed to be friendly ways to get involved and learn some of the ins and outs of BOINC development. 

[Open, unassigned issues in the boinc repo good for new contributors](https://github.com/BOINC/boinc/issues?q=is%3Aissue+is%3Aopen+no%3Aassignee+label%3A%22good+first+issue%22)

### 2.2 Returning Contributor
Users who are involved in the BOINC community, or have been in the past, can find issues waiting for someone to pick up the work by using the "no:assignee" filter.

[Open, unassigned issues in the boinc repo](https://github.com/BOINC/boinc/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+no%3Aassignee)

### 2.3 "Pet Project"
A developer who creates an issue and is both capable and self-motivated to complete it should set the assignee field appropriately upon creation of the issue so that it is clear that other developers should not pick it up. However, it would still be a good idea to wait for review by other members of the community prior to beginning development to avoid wasted effort. Once the issue is "Verified", development work can begin.

### 2.4 Tracking Release Status
The release manager for the client or server software can use a milestone for a specific release version and add issues to that milestone that should be included in the release. All issues that have been resolved as part of a pull request to the master branch after the previous release branch was cut should already be included in this current release milestone, so the release manager can see the history of all changes that are being included.

### 2.5 Stalled Issues
Any open issues that have been inactive for a long period of time should be labeled as "Stalled". These issues should be reviewed again to determine if they should be changed from their review state of Verified, Parked, or Discussion Needed, or if they should be closed.

