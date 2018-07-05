# Client Release Process
The purpose of this document is to define the client release process at a high level, establishing a standard process so that the community knows what to expect and where they can help with new versions of the client. In order to understand this process, it is useful to first understand the [development workflow](Development_Workflow.md) and [BOINC Flow (Branch and merge strategy)](BOINC_Flow.md).

## Overview
The release process will produce some or all of the following items:
- Downloadable binaries for a new version of the client software for:
  - 32 bit Windows (one with VirtualBox and one without)
  - 64 bit Windows (one with VirtualBox and one without)
  - 64 bit OSX
- Updated application in the Google Play Store
- Updated versions of the Linux client by the package maintainers for EPEL and Debian
- Documentation about features
- Release notes / version history
- Announcements

In order to produce this, the following need to be updated, built, and tested:
- The code used to build the binaries
- Dependent libraries
- Copyright and other legal information
- Installer definitions 
- All text included in screen displays, messages, etc.
- Translations of text
- Test cases and their outcomes
- Any included data (e.g. 'all projects list' and ca-bundle)

## Roles
The process of releasing the client requires the work of a number of people in the community. As such there are some additional roles that are useful to define for this process. Note that one person can serve in one or more roles during the process (for example, one person can be the release manager as well as the build master for Windows).

### Release Manager
The release manager is the person who manages the release process. He or she is responsible for the communications and coordination required to get the release built, tested, and announced. Some of the things the release manager is expected to do are:
- Announce the intention to make a new release of the client
- Ask if anyone has anything that they are working on that they want to include the release.
- Determine when to create the release branch
- Coordinate the builds of the client
- Coordinate the testing of each build of the client
- As bugs are found during testing, identify which ones will be fixed and included in the current release vs deferred to a future release
- Ensure that all required items that need to be updated in the release have been updated (see list of items produced in a release in the overview above)
- Call for a consensus vote of committers to determine if a build is ready to be declared as generally available
Throughout the process, the release manager is expected to communicate what is going on as the work progresses and make sure to address concerns that are raised as the work progresses.

### Build Master
Someone needs to be responsible for building the clients for each of Windows, Mac, Linux, and Android. It can be a different person or the same person for each platform. These people will be responsible for creating official builds when the release manager requests a new build. Build masters will work with the PMC in order to gain access to any signing keys or login rights required to create builds for their platforms. 

The build masters will work with the release manager in order to ensure that new builds are created at the requested times as the release work proceeds.

### Testers
People who want to help test the client releases should be familiar with the [Alpha Testing](https://boinc.berkeley.edu/trac/wiki/AlphaInstructions) wiki page and associated processes.

## Process
### Prepare for a Release
The release manager will announce the intention to make a new release of the client. When they do this they should make a request to the community to find out if there is any work in progress that will be available shortly that should be included on the request. The release manager will work with anyone who responds to determine if that work will be included or not depending on the relevant concerns at the time.

The release manager should also connect with the build masters and confirm with them that they are available for creating builds during the next several weeks as the work progresses.

The release notes should be created/updated each time a build is made from a release branch. The information in the release notes should contain the new features and important bugs fixed since the previous release. They should be recorded in a style similar to this: https://boinc.berkeley.edu/wiki/Release_Notes_for_BOINC_7.6. 

### Release Branch
The release branch is created once the release manager has decided that all work that will be included in the release is available in the master branch. Once a release branch is created, it is expected that the community will work to quickly test and make the release available for general use. The release manager and the community should try to avoid having releases that take longer than two to three weeks between the creation of a release branch and making the release generally available.

The release branch is feature frozen. This means that no new features should be added to the release once the release branch is created. Additionally, only important bug fixes should be merged into the release branch. The release manager makes the final decision about what, if any, changes will be merged into the release branch.

All code merged into the release branch will be a cherry-pick based on a merge commit.

Please read [BOINC Flow](BOINC_Flow.md) for more details about how feature branches, bugfix branches and release branches are used by the BOINC community.

### Build and Test
The build and test cycle for the client is done by leveraging the supporters who are willing to test the client through the process outlined on the [Alpha Testing wiki page](https://boinc.berkeley.edu/trac/wiki/AlphaInstructions).

The test process should roughly follow the following path:
- The release manager increments the build version number and asks the build masters to create a new build of the client
- At this stage the build number should use an odd 'minor' number as it is considered a test build. Ex: 6.11.20
- The release manager updates (or asks someone to update for them) the version history with a list of significant changes since the last build
- Once the builds are available, the release manager sends an email to the boinc-alpha email list announcing the availability of a new release candidate and points them to the version history page. The release manager asks the testers to start a new round of testing
- Testers conduct testing and record bugs found
- The release manager monitors bugs being reported and designates those that need to be fixed in this release and those that can be fixed for a future release. The release manager should inform the community on boinc-alpha about which bugs are to be fixed and which are to be deferred to a future release. The release manager should respond to comments and different perspectives about these decisions and consider carefully the feedback from the community. 
- Repeat after designated bugs have been fixed

### General Acceptance
The build and test cycle repeats until there are no bugs remaining that have been designated to be fixed in this release. Once this occurs, the release manager will increment the version number so that the 'minor' version is even indicating that this is a release candidate. He or she will then ask the build masters to rebuild the clients using the new version number.

After the testers perform a lightweight regression test of the new builds and no new bugs are found, the release manager will call for a consensus vote of the committers to declare the build as generally available. If the vote succeeds, then the BOINC website is updated to reflect the status of the release as generally available.

### Post Release Management
It is inevitable that additional bugs will be found once the software is released to the general public. The release manager, build masters and testers should expect to remain engaged for several weeks following general availability of a release and continue to track bug reports that come in from end users. The release manager will continue to lead the community through the process of prioritizing these bugs, and determine if they need to be fixed in the current release with a new build, or if they can be deferred until a future release. If the release manager decides that a bug needs to be fixed, then the release manager will lead the community through another build and test cycle that includes the fixes for the designated bugs.

## Appendix
### Version Numbering
The BOINC client uses the following in its release numbering:

Major.Minor.Build
- The major is incremented when a significant and fundamental change is made to the client. The release manager shall decide when a release constitutes a significant enough change to merit incrementing the major version number.
- Odd minor version numbers indicate that the version is a test build.
- Even minor version indicate a release candidate or a generally available release. 
- Build version numbers are incremented each time a new build is made.

# Document Change Process
This document can be updated by following the process documented in section 6.2 of the [Governance](../Governance_Documents/Governance.md#62-development-documents) document.