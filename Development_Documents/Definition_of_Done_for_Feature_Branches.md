# Definition of Done for Feature Branches
The definition of done is an agile document that clarifies what it means for a set of development tasks to be completed.  It is both a check list and a set of guidelines that should be followed.

## Development Practices
- Code has followed the style guide for BOINC (http://boinc.berkeley.edu/trac/wiki/CodingStyle)
- Commit does not contain unrelated code changes
- Code uses atomic commits (https://www.freshconsulting.com/atomic-commits/)

## Testing
- The code compiles on relevant major platforms (this should be available via automation)
  - For Client or API it builds on reference systems (Ubuntu 14.04LTS, OSX 10.11, Windows Visual Studio 2013) (enabled via Travis CI and !AppVeyor)
  - For Server it builds on reference systems (Ubuntu 14.04LTS)
- The code passes all existing automated build and unit tests
- The developer has tested the code in a working environment (i.e. ran the client code with a project, tested server changes against an alpha project, etc)

## Documentation
- The pull request to merge a branch should list the issue(s) that it fixes.  (Use keywords to link the pull request to issue: https://help.github.com/articles/closing-issues-using-keywords/)
- If this code changes the available features or behavior of the system, then the documentation on the BOINC wiki needs to be updated to reflect that (reference the version it belongs to)

# Pending - Not Yet Applicable
The following will be added to the definition of done when the necessary automation and configuration is enabled.  It is included here to indicate the direction the project is moving.

## Development Practices
- Code developed includes automated unit tests or is already covered by existing tests.
  - Will be added when a framework is adopted for each part of the code
- Code quality scans have been run and no new issues have created due to these changes.  (need information on code quality scans)
  - Will be added as soon as Scrutinizer and Coverity are configured to generate useful information without a lot of noise due to conflicts in code styles

# Document Change Process
This document can be updated by following the process documented in section 6.2 of the [Governance](../Governance_Documents/Governance.md#62-development-documents) document.