# BOINC Project Governance
January 12, 2018

## 1. Overview
BOINC is an open-source middleware system for volunteer computing, originally developed at UC Berkeley. BOINC is a meritocratic, consensus-based project. Anyone can join the BOINC community and contribute to the project in various ways. Those who consistently make positive contributions, as recognized by other contributors and users, can then become part of the decision-making process. This document describes the structures and processes governing these activities.

### 1.1 Mission
The general goal of the project is to maintain and develop BOINC in a way that:
- Reflects the needs and interests of its community.
- Is “sustainable”, i.e. does not depend on any one person, group, or funding source, and which allows and encourages volunteer participation.

Specific goals include:
- Distribute an “official” version of the BOINC source code, and a revision history with branches corresponding to public releases.
- Ensure that the BOINC software is modified as needed to work correctly with new versions of operating systems and virtualization software, new GPUs and other coprocessors, and new versions of server software such as Linux, PHP, Apache, and MySQL.
- Maintain a “public web site” (currently https://boinc.berkeley.edu) where volunteers can learn about volunteer computing, download the client software in installer form, and get support. The web site will also have instructions for people wanting to contribute to the project, and will describe the governance structure of the project, including the current version of this document.
- Ensure that the BOINC documentation is available online and is maintained.
- Maintain the process of internationalizing (translating) the BOINC software.
- Ensure that future development of BOINC proceeds coherently according to architectural plans agreed upon by the community.

## 2. Roles and responsibilities
In the following discussion, it is important to note that people may belong to one or more categories. For example, someone can be a committer and a PMC member. In another case, someone might only be a PMC member. In all cases, one person only gets one vote on issues even if they have multiple roles.

### 2.1 Users
“Users” are people who use BOINC in some way. Examples include:
- “Volunteers” run the BOINC client software, contributing processing power and storage capacity to computing projects.
- “Project admins” operate BOINC-based computing projects (academic science projects, hobbyist projects, commercial projects). They run the project’s servers, maintain its web site, and develop and deploy its applications.
- “Add-on developers” create and operate systems that, although not part of BOINC, interact with it through its various APIs. Examples include: Account managers (such as BAM! And GridRepublic) Statistics web sites (such as BoincStats and BOINC All-Project Stats) GUIs such as BOINCTasks Branded versions of BOINC (such as HTC Power to Give, Samsung Power Sleep, and Intel Progress Thru Processors)
- Leaders of BOINC teams.

Anyone can be a user. The project asks its users to participate in the project and community as much as possible, for example by:
- Evangelizing about the project (e.g. by web links or word of mouth)
- Informing the community of strengths and weaknesses of BOINC’s products
- Users may contribute in other ways, as described below.

### 2.2 Contributors
“Contributors” are people who contribute in concrete ways to BOINC, other than by computing for a BOINC-based project. Forms of contribution include:
- Programming
- Testing and bug reporting
- Writing and editing documentation
- Doing translations for a particular language
- Identifying and defining new software requirements
- Providing “customer support” by answering questions from volunteers and contributors
- Providing infrastructure (servers, hosting of email lists)
- Financial support, such as paying the salary of other contributors

In some forms of contribution, such as programming and documentation, contributors submit changes by developing code in branches and submitting them as pull requests for review by committers (see the next section). As contributors gain experience, their reputation within the community will increase. Contributors can nominate themselves or other people to the PMC as potential committers. 

### 2.3 Committers
“Committers” are contributors who have shown, via a sequence of positive contributions, their value to the project. Committers facilitate the software development process both by contributing code themselves and also by mentoring contributors to help them become more effective contributors. Only committers can merge a pull request into the master branch and they should only do so through the process defined in [section 4. Contribution Process](#4-contribution-processes). Committers have voting rights in the consensus process as it pertains to proposed design changes and to the reviews of pull requests. They contribute to discussion and approval of the software development process as documented in [section 4. Contribution Process](#4-contribution-processes).

Each committer will work on one or more “areas” of the BOINC project:
- Software development and maintenance
- Translation system
- Testing and release management
- Documentation
- BOINC web site, including News items
- Support
- Infrastructure (e.g. setting up and maintaining email lists and Github repository; maintaining BOINC web server)     
- And any other such thing as might be required from time to time

Depending on the committers' area(s), they can be given one or more specific privileges such as:
- Commit access to the source code repository
- Write access to the documentation Wikis
- Write access to the public web site
- Moderator status on the BOINC project message boards

Committers are expected to do several of the following:
- Read the communication channels relevant to their area(s)
- Subscribe to pull request notifications within github (https://help.github.com/categories/notifications/)
- Review bug reports and features and make sure that they are valid and contain sufficient detail to implement
- Review proposed solutions to bugs and feature requests
- Prioritize bug reports and features so that contributors and other developers know which issues are most important and in need of contribution
- Review pull requests and merge code when appropriate
- Identify contributors who would be helpful as committers; nominate these contributors to the PMC

Commiters can resign by sending an email to the PMC chair or the PMC public email list.

### 2.4 Supporters
"Supporters" are contributors who have shown, via continued contribution over a period of time, their value to the project.  Supporters are focused on the end user experience and support the project by engaging with end-users wherever they may engage with the BOINC software and BOINC projects to both help the end-users as well as open issues as needed when there is a need for a change in the software.  Supporters also contribute by performing functions such as testing, enhancing documentation, and creating translations.

"Supporters" are similar to "Committers" except that they are not contributing source code to the project.  They have voting rights equal to committers except that they cannot vote on issues that specifically pertain to software architecture and source code.

Each supporter will work on one or more “areas” of the BOINC project:
- Translation system
- Testing and release management
- Documentation
- BOINC web site, including News items
- Support
- And any other such other thing as might be required from time to time     

Depending on the supporter’s area(s), they can be given one or more specific privileges such as:
- Permission to manage issues on GitHub
- Write access to the documentation Wikis
- Write access to the public web site
- Moderator status on the BOINC project message boards

Supporters are expected to do one or more of the following:
- Periodically review a few of the BOINC, project and team forums in order to remain aware of the experience the end-users are reporting with the software
- Identify bugs, issues and feature requests from users and turn them into issues on GitHub
- Review bug reports and features and make sure that they are valid and contain sufficient detail to implement
- Prioritize bug reports and features so that contributors and other developers know which issues are most important and in need of contribution
- Read the communication channels relevant to their area(s)
- Assist with testing new releases of the software
- Identify contributors who would be helpful as supporters; nominate these contributors to the PMC

Supporters can resign by sending an email to the PMC chair or the PMC public email list.

### 2.5 Project Management Committee
The Project Management Committee (PMC) is a group of community members who engage with and play a leadership role on the BOINC project.  They are selected on the basis of one or more of the following criteria:
- Directly contributing in any of the ways listed in [section 2.2 Contributors](#22-contributors)
- Operating a related system, such as an account manager, that is used by a significant number of volunteers
- Operating a project with a significant number of volunteers
- Contributing significant resources to the BOINC project, for example by paying the salary of a contributor
- Thought leaders in the field of high performance computing who have an interest in promoting the use of volunteer computing

The functions of the PMC are:
- Decide on the strategic directions of the project
- Decide issues of intellectual property (copyright, licensing) and other legal issues
- Support and encourage the recruitment and development of committers and supporters
- Ensure that necessary tasks for the long term success of the BOINC project are being done
- Resolve conflicts within the community
- Review and vote on nominated committers and supporters
- Vote on adding or removing members of the PMC as needed
- Decide on the set of “approved” projects and account managers             
- Modify the governance policies of the BOINC project as needed
- And any other such other thing as might be required from time to time     

Individual PMC members are expected to actively participate in these processes by:
- Reading the PMC public and private email lists (See [section 3. Communication channels](#3-communication-channels) below)
- Participating in votes (see [section 5.3 PMC decisions](#53-pmc-decisions) below)
- Regularly participate in monthly PMC calls

Members of the PMC can resign by sending an email to the PMC chair or the PMC private email list.

#### 2.5.1 PMC Positions
##### 2.5.1.1 PMC Chair
The “PMC Chair” is a member of the PMC, elected by the PMC to take this role. The chair has the following responsibilities:
- Ensures that the functions of the PMC are being performed   
- Ensures that the activities of the BOINC community are in agreement with this document and established procedures
- Ensures that votes are taken promptly on issues that require votes
- Schedules monthly meetings of the PMC

The PMC Chair shall be elected for a term of one year.  They can be re-elected to successive terms up to a maximum of three consecutive terms.

##### 2.5.1.2 PMC Secretary
The "PMC Secretary" is a member of the PMC, appointed and ratified by the PMC to take this role.  The secretary has the following responsibilities:
- Ensure that items posted in the public PMC mailing list are addressed   
- Take notes at monthly meetings of the PMC and distribute them to all PMC members within 7 days of the meeting
  - Must officially record who attends each meeting as part of the minutes
- Ensure that a public version of the notes is distributed on the public PMC mailing list
- Monitor and identify PMC members who should be considered for removal due to inactivity (see [2.5.3 Inactive Removal](#253-inactive-removal) below)
- Maintain the official record of committers, supporters and members of the PMC (see [section 2.6 Official Record](#26-official-record) below)
- Act as the official vote counter and recorder for all votes taken
  - An email to the private PMC list must made at the conclusion of each vote stating:
    - What was the issue voted on
    - The outcome of the vote
    - Who voted and how they cast their vote
  - An email sent to the public PMC list must be made at the conclusion of each vote stating:
    - What was the issue voted on
    - The outcome of the vote
    - Who voted
  - In the event that the PMC determines a vote is sensitive in nature, then they can decide to not announce the vote publicly.  The PMC is encouraged to do this rarely and with clear justification.

The PMC Secretary is appointed by the Chair and ratified by the PMC using consensus voting to serve in this role.  Another person can be appointed to this position as determined by the PMC Chair.

#### 2.5.2 PMC Chair Elections
Any member of the PMC can call for an election of the PMC Chair.  When a member of the PMC calls for an election they must specify that the election is either to immediately replace the current Chair or if the newly elected Chair will start their term when the current term expires. 

Elections shall use the election decision process outlined in [section 5.3.2 Election decisions](#532-election-decisions) below.

#### 2.5.3 Inactive Removal
PMC members are expected to remain engaged and connected to the community.  If they are not, then they cannot effectively act as the advisor and leader to the community as is their role.  As a result, any member of the PMC that goes for a year without actively participating in the [processes of the PMC](#25-project-management-committee) should be considered for removal from the PMC.  Removal requires a successful vote using [super majority voting](#531-pmc-decisions-that-require-super-majority-voting) below.

### 2.6 Official Record
The official list of committers, supporters and members of the PMC shall be maintained by the secretary at http://boinc.berkeley.edu/trac/wiki/ProjectGovernance. This page shall also clearly list the email address of the PMC public email list with instructions on how someone can subscribe to the list.

## 3. Communication channels
The project will provide communication channels for various purposes:
- PMC public email list, used for:
  - Requests to be a submitter
  - Requests to be a PMC member
  - Project-level discussion
- PMC private email list, used for sensitive issues, such as discussion of potential new committers, or legal matters that can’t be discussed in public. It is not used for project management or planning
- Issue tracking system, for bugs and development requests (https://github.com/BOINC/boinc/issues)
- Volunteer message boards, for support requests and responses
- Project admin email list, for announcements and discussion related to the BOINC server software and other issues related to BOINC-based computing projects
- Email lists for specific contribution areas, such as software development, testing, and translations

Except for the PMC private email list, all of these channels will be publicly readable and writable.

## 4. Contribution processes
Anyone can contribute to BOINC. There are multiple ways to contribute to BOINC:

- Help other users by answering questions on the BOINC forums (https://boinc.berkeley.edu/dev/forum_index.php), project forums (see project list: https://boinc.berkeley.edu/projects.php) or on the BOINC mailing lists (https://boinc.berkeley.edu/trac/wiki/EmailLists)
- Add or maintain documentation to the BOINC wikis
- Add or maintaining translations of BOINC
- Participate in the Alpha testing of software releases (https://boinc.berkeley.edu/alpha/)
- Make a technical contribution

If you need help getting started, then please visit https://boinc.berkeley.edu/dev/forum_index.php and post in the "How to Contribute" forum.

### 4.1 Technical Contributions
The process of making technical or code contributions is the same for everyone, regardless of whether they are a contributor, committer or PMC member. You can contribute by doing the following:

- Read the BOINC developer information (https://boinc.berkeley.edu/trac/wiki/SoftwareDevelopment) to learn about the BOINC system
- Find something that needs to be implemented in BOINC:
  - Review the Project (https://github.com/BOINC/boinc/projects) associated with the area of BOINC in which you want to contribute
  - Issues that have been reviewed and are ready for implementation are listed under Longterm or TODO
  - Issues with a higher priority for implementation are listed under TODO
- Follow the software development process that BOINC uses (See [Development_Workflow.md](Development_Workflow.md))

If you are reporting a bug or requesting a feature, make sure you review the [Development Workflow](Development_Workflow.md) before you submit it.

## 5. Decision processes
### 5.1 Voting Processes
Decisions in the BOINC community should made easily but also in a way that promotes a collaborative environment.  As a result, the following mechanisms for voting on a decision are defined:

#### 5.1.1 Consensus Voting
Consensus voting consists of a 7 day review period. During this time anyone can review and discuss the item. At the end of the 7 day period, if there is at least one "Yes" vote for an item (apart from the vote of the person who created the item) and zero "No" votes, then the vote shall be deemed as having passed.

A vote of "No" shall not be valid unless it is accompanied by a detailed explanation of the objection to the item. It is preferable to suggest an alternative implementation if possible.

If discussion cannot remove the concerns that resulted in the "No" vote, then the vote shall be deemed as having failed.

If the vote fails, but the original proposer of the item still believes that the item is worth pursuing, they can appeal to the PMC. The PMC shall consider the appeal at their next regularly scheduled meeting and will use Majority Voting to determine the outcome.

#### 5.1.2 Majority Voting
Majority voting requires that at least 66% of eligible voters cast a vote and, of those who cast a vote, a majority must approve the item.

#### 5.1.3. Super-Majority Voting
Super-majority voting requires that at least 75% of eligible voters cast a vote and, of those who cast a vote, a majority must approve the item.

### 5.2 Committer decisions
Committers can vote on issues surrounding the technical infrastructure of the project and the code base itself. This includes voting to determine if a reported bug, feature request, proposed design, or pull request should be accepted. Committers are encouraged to review and participate in the discussion of any of these items, but they are also expected to know when it is advisable to get help from other committers who are stronger in the technology involved or have more experience in the area of application under consideration. Committers are expected to understand the Development Workflow and Client Release Process and their associated guidelines before voting to approve.

Committers are expected to subscribe to notifications from github in order to be aware of proposals under consideration. Committers should make a reasonable attempt to respond quickly if they are personally asked to review an item. Since most decisions that committers are involved in will use consensus voting, it is important for them to try to remain aware of proposed items.

Different committer decisions should be recorded and discussed in the following locations:
- Whether or not to fix a bug or implement a feature request (documented and voted on as an issue on github)
- The design of a proposed feature or bug fix (documented and voted on within the relevant issue on github)
- A change in code or configuration to the system (documented and voted on as a pull request on github)
- General availability of stable releases (documented and voted on in the boinc_alpha mailing list)
- All other committer decisions should be discussed and voted on in the boinc_dev mailing list.


- Procedural and other issues
  - Other committer votes not otherwise identified will be voted on in the boinc_dev mailing list
  - Other PMC votes not otherwise identified will be voted on in the boinc_adm or private boinc_pmc mailing lists as deemed appropriate by the PMC.

Votes on design reviews, pull requests, and general availability of a stable release shall use the consensus voting process.

Procedural and other issues shall always follow the majority voting process.


### 5.3 PMC decisions
PMC decisions will be made by majority voting unless specified in section 5.3.1 or in section 5.3.2.

Votes can be called by any PMC member. The process is:
- A vote is announced on either the PMC public or private email list (depending on the sensitivity of topic), phrasing the issue as a yes/no decision.
- If the vote is announced on the PMC public list, then the entire community is encouraged to participate in the discussion of the vote and that discussion should occur on the PMC public list. 
- If the vote is accouned on the PMC private list, then discussion is limited to PMC members and it shall be conducted in a meeting or on the PMC private email list.
- Vote outcomes are announced by the PMC secretary as described in [section 2.5.1.2 PMC Secretary](#2512-pmc-secretary)

#### 5.3.1 PMC Decisions that Require Super-Majority Voting 
The following types of decisions require a super-majority vote of the PMC
- Intellectual property issues, e.g. those involving copyright and licensing of BOINC code
- Other legal and financial decisions
- PMC membership changes
- Changes to the project governance structure (i.e. changes to this document)

#### 5.3.2 Election decisions
The PMC will conduct elections to elect the PMC Chair.   An election starts when any member of the PMC calls for an election as specified in section 2.5.2 PMC Elections.  This call starts a 7 day nomination period which is followed by a 7 day voting period.  Any member of the PMC can nominate themselves or another member of the PMC to be the PMC Chair.  A nomination is only valid if the person nominated accepts the nomination.  Once the 7 day nomination period ends, the 7 day voting period begins automatically.  At the conclusion of 7 day voting period and if at least 75% of the membership of the PMC has voted, then the person with the majority of votes is elected. 

All nominations and voting need to be recorded on the private PMC mailing list.

##### 5.3.2.1 Voting Irregularities
Various situations can arise during voting.  Some of these are listed below with the actions that should be taken if they occur:
- If fewer than 75% of the members of the PMC cast a vote during the 7 day voting period, then a new election must be held.
- In the event that no-one has a majority at the end of the 7 day voting period, then a new election must be held.
- If after 2 attempts to conduct an election no-one has been elected or nominated, then the previous chair is automatically re-instated to a new one year term.
- In the event that a member of the PMC reports an issue with regards to access to the PMC private mailling list that impacts their ability to nominate someone or cast a vote, then the election shall be null and void and must be redone once the issue is resolved.

#### 5.3.3 Other voting decisions
For all other types of decisions that require a PMC vote, the PMC will start decision making using the consensus voting with PMC members voting. If consensus voting fails to reach agreement, the chair or the person who called the vote can request that a majority vote occurs to determine the outcome.
