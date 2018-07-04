# Server Release Process
The purpose of this document is to define the server release process at a high level, establishing a standard process so that the community knows what to expect and where they can help with new versions of the server. In order to understand this process, it is useful to first understand the [development workflow](https://github.com/BOINC/boinc-policy/blob/master/Development_Workflow.md).
## Overview
The release process will produce some or all of the following items:
- A versioned tag of the software, downloadable as a zip file
- Documentation about features
- Release notes / version history
- Announcements

In order to produce this, the following needs to be updated, built, and tested:
- The code used to build the server

## Roles
The process of releasing the server requires the work of a number of people in the community, mainly from with the projects.  As such there are some additional roles that are useful to define for this process.  Note that one person can serve in one or more roles during the process.

### Release Manager
The release manager is the person who manages the release process. He or she is responsible for the communications and coordination required to get the release built, tested, and announced. Some of the things the release manager is expected to do are:
- Announce the intention to make a new release of the server
- Ask if anyone has anything that they are working on that they want to include the release.
- Coordinate the build and testing of the server
- As bugs are found during testing, identify which ones will be fixed and included in the current release vs deferred to a future release
- Ensure that all required items that need to be updated in the release have been updated (see list of items produced in a release in the overview above)
- Call for a consensus vote of committers to determine if a tag is ready to be declared as generally available
Throughout the process, the release manager is expected to communicate what is going on as the work progresses and make sure to address concerns that are raised as the work progresses.

### Testers
People who want to help test the server releases should be familiar with deployment in a project. 

## Process
### Prepare for a Release
The release manager will announce the intention to make a new release of the server.  When they do this they should make a request to the community to find out if there is any work in progress that will be available shortly that should be included on the request. The release manager will work with anyone who responds to determine if that work will be included or not depending on the relevant concerns at the time.

### Release Branch
The release branch is created once the release manager has decided that all work that will be included in the release is available in the master branch.

The release branch is considered feature frozen. Only bug fixes designated by the release manager will be merged into the release branch.

Bug fixes designated by the release manager for fixing within the release should be branched from the release branch and merged directly into the release branch.  Doing this reduces the chance of inadvertently bringing in unrelated code changes.

If the release manager determines that some code should be merged from master into the release branch, then this can be done. However, this should be viewed as an unusual step and carefully considered due to the risk of introducing unexpected change.

The release notes will be created/update when the final tag is made from a release branch. The information in the release notes should contain the new features and important bugs fixed since the previous release. 

### Build and Test
The build and test cycle for the server is done by leveraging the supporters most probably related to a project, who are willing to test the server.

The test process should roughly follow the following path:
- The release manager increments the tag version number and asks the supported to build and tag the new server
- At this stage the tagged version should use an odd 'minor' number as it is considered a test.  Ex: 0.9.1
- The release manager updates (or asks someone to update for them) the version history with a list of significant changes since the last tagged version
- Once the tag is available, the server manager sends an email to the boinc-dev and boinc-projects email list announcing the availability of a new release candidate and points them to the version history page. The release manager asks the testers to start a new round of testing
- Testers conduct testing and record bugs found
- The release manager monitors bugs being reported and designates those that need to be fixed in this release and those that can be fixed for a future release. The release manager should inform the community which bugs are to be fixed and which are to be deferred to a future release. The release manager should respond to comments and different perspectives about these decisions and consider carefully the feedback from the community. 
- Repeat after designated bugs have been fixed

### General Acceptance
The build and test cycle repeats until there are no bugs remaining that have been designated to be fixed in this release. Once this occurs, the release manager will increment the version number so that the 'minor' version is indicating that this is a release candidate.

The release manager will call for a consensus vote of the projects to declare the tag as generally available.  If the vote succeeds, then the BOINC website is updated to reflect the status of the release as generally available.

At this point, if it has not already been done, the release branch should be merged back into the master branch to ensure that all bug fixes are part of the master branch (note that this can occur earlier and repeatedly during the process, but it must at a minimum occur at the end of the process).

### Post Release Management
It is inevitable that additional bugs will be found once the software is released. The release manager and testers should expect to remain engaged for several weeks following general availability of a release and continue to track bug reports that come in from the projects. The release manager will continue to lead the community through the process of prioritizing these bugs, and determine if they need to be fixed in the current release, or if they can be deferred until a future release.  If the release manager decides that a bug needs to be fixed, then the release manager will lead the community through another build and test cycle that includes the fixes for the designated bugs.

## Appendix
### Version Numbering
The BOINC server uses the following in its release numbering:

Major.Minor.Build
- The major is incremented when a significant and fundamental change is made to the server.  The release manager shall decide when a release constitutes a significant enough change to merit incrementing the major version number.
- Odd minor version numbers indicate that the version is a test release.
- Even minor version indicate a release candidate or a generally available release.  
- Build version numbers are incremented each time a new build is made.

# Document Change Process
This document can be updated by following the process documented in section 6.2 of the [Governance](../Governance_Documents/Governance.md#62-development-documents) document.
