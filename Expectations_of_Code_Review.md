# Reviewer Expectations for Code Review
Code reviews have to support the competing goals of rapid code development, architectural integrity and quality code.  To this end reviewers are asked to take a pragmatic approach to their review and they should accept code that may not be feature complete so long as it does not do any of the following:
- Contains known bugs that will occur under likely scenarios
- Prevent the code from building
- Prevent the code from working correctly under current use cases
- Interfere with the development activities of other contributors

In addition, the reviewer should do the following and provide feedback about the items to the contributors:
- Verify that Definition of Done has been completed
- Visual inspect code to see that it does what it needs to and doesn't do what is not reported
- Confirm that all comments and questions raised in discussion of the pull request have been resolved
- If possible, a reviewer should build and test the code changes
- Check that consensus voting has resulted in approval of each issue resolved with the pull request (see governance document for details)
- Check that consensus voting has resulted in approval of the pull request itself (see governance document for details)
