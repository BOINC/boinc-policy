# BOINC Project Governance
June 1, 2015

## 1. Overview
BOINC is an open-source middleware system for volunteer computing, originally developed at UC Berkeley.  BOINC is a meritocratic, consensus-based project.  Anyone can join the BOINC community and contribute to the project in various ways.  Those who consistently make positive contributions, as recognized by the community, can then become part of the decision-making process.  This document describes the structures and processes governing these activities.

### 1.1 Mission
The general goal of the project is to maintain and develop BOINC in a way that
- Reflects the needs and interests of its community.
- Is “sustainable”, i.e. does not depend on any one person, group, or funding source, and which allows and encourages volunteer participation.
- Leads to world peace (*sorry" test edit; will remove in a sec)

Specific goals include:
- Distribute an “official” version of the BOINC source code, and a revision history with branches corresponding to public releases.
- Ensure that the BOINC software is modified as needed to work correctly with new versions of operating systems and virtualization software, new GPUs and other coprocessors, and new versions of server software such as Linux, PHP, Apache, and MySQL.
- Maintain a “public web site” (currently http://boinc.berkeley.edu) where volunteers can learn about volunteer computing, download the client software in installer form, and get support.  The web site will also have instructions for people wanting to contribute to the project, and will describe the governance structure of the project, including the current version of this document.
- Ensure that the BOINC documentation is available online and is maintained.
- Maintain the process of internationalizing (translating) the BOINC software.
- Ensure that future development of BOINC proceeds coherently according to architectural plans agreed upon by the community.

## 2. Roles and responsibilities
### 2.1 Users
“Users” are people who use BOINC in some way.  Examples include:
- “Volunteers” run the BOINC client software, contributing processing power and storage capacity to computing projects.
- “Project admins” operate BOINC-based computing projects (academic science projects, hobbyist projects, commercial projects).  They run the project’s servers, maintain its web site, and develop and deploy its applications.
- “Add-on developers” create and operate systems that, although not part of BOINC, interact with it through its various APIs.  Examples include:
  - Account managers (such as BAM! And GridRepublic)
  - Statistics web sites (such as BoincStats and BOINC All-Project Stats)
  - GUIs such as BOINCTasks
  - Branded versions of BOINC (such as HTC Power to Give, Samsung Power Sleep, and Intel Progress Thru Processors).
- Leaders of BOINC teams.

Anyone can be a user.  The project asks its users to participate in the project and community as much as possible, for example by
- Evangelizing about the project (e.g. by web links or word of mouth).
- Informing the community of strengths and weaknesses of BOINC’s products.

Users may contribute in other ways, as described below.

### 2.2 Contributors
“Contributors” are people who contribute in concrete ways to BOINC, other than by computing for a BOINC-based project.   Forms of contribution include:
- Programming.
- Testing and bug reporting.
- Writing and editing documentation.
- Doing translations for a particular language.
- Identifying and defining new software requirements.
- Providing “customer support” by answering questions from  volunteers and contributors.
- Providing infrastructure (servers, hosting of email lists).
- Financial support, such as paying the salary of other contributors.

In some forms of contribution, such as programming and documentation, contributors submit changes as “patches”, which will be considered for inclusion in the project by committers (see the next section).  As contributors gain experience, their reputation within the community will increase, and at some point they may be nominated to become committers.

### 2.3 Committers
“Committers” are contributors who have shown, via a sequence of positive contributions, their value to the project.  Committers are able to make changes directly, rather than by Committers have no more authority over the project than contributors.   Their work is visible to the community (e.g. in a commit history) and can be reviewed by the community.  The key difference is that this review happens after the change is made, rather than before.
submitting patches.  
Each committer will be associated with one or more “areas” of the project:
- Software development and maintenance
- Translation system
- Testing and release management
- Documentation
- BOINC web site, including News items.
- Support
- Infrastructure (e.g. setting up and maintaining email lists and Github repository; maintaining BOINC web server).

Depending on the committer’s area(s), they will be given specific privileges such as:
- Commit access to the source code repository.
- Write access to the documentation Wikis.
- Write access to the public web site.
- Moderator status on project message boards.

Committers are expected to:
- Read the communication channels relevant to their area(s).
- Participate in the process of evaluating and committing patches in their area(s).

### 2.4 Project Management Committee
The Project Management Committee (PMC) is a group of community members who have consistently and significantly contributed to the project, for example by
- Directly contributing in any of the ways listed in Section 2.2
- Operating a related system, such as an account manager, that is used by a significant number of volunteers.
- Operating a BOINC project with a significant number of volunteers.
- Contributing significant resources to the project, for example by paying the salary of a contributor.

The functions of the PMC are:
- Decide on the strategic directions of the project.
- Decide issues of intellectual property (copyright, licensing) and other legal issues.
- Choose committers.
- Decide on PMC membership.
- Decide on the set of “approved” projects and account managers.
- Modify the governance policies of the project as needed.

PMC members are expected to actively participate in these processes, by
- Reading the PMC email lists (see below).
- Participating in votes (see below).

The “PMC Chair” is an individual, elected by the PMC.  The Chair remains in that role until they retire or the PMC votes to remove them. The Chair has various administrative functions (such as managing votes) and is expected to ensure that governance processes are adhered to.  He or she has no additional authority beyond that of other PMC members.

The initial membership of the PMC will be by invitation from the BOINC project at UC Berkeley.

## 3. Communication channels
The project will provide communication channels for various purposes:
- PMC public email list, used for
  - Requests to be a submitter.
  - Requests to be a PMC member.
  - Project-level discussion.
- PMC private email list, used for sensitive issues, such as discussion of potential new committers, or legal matters that can’t be discussed in public.  It is not used for project management or planning.
- Issue tracking system, for bugs and development requests.
- Volunteer message boards, for support requests and responses.
- Project admin email list, for announcements and discussion related to the BOINC server software and other issues related to BOINC-based computing projects.
- Email lists for specific contribution areas, such as software development, testing, and translations.

Except for the PMC private email list, all of these channels will be publicly readable and writeable.

## 4. Contribution processes
Anyone can contribute to BOINC.  The general process is:
- Read the BOINC web site to learn about the areas of contribution.  For each area, the web site will contain instructions for how to contribute, e.g. how to submit patches.
- Read the communication channels relevant to the chosen area.
- Contribute, either directly (e.g. by responding to support requests on the volunteer message boards) or by submitting a patch.

In all cases, contributors are expected to work as part of the community.  For example:
- Before submitting a software patch for a new feature, a contributor should discuss the feature and its implementation with the community.
- Before filing a bug report, a contributor should scan the relevant message boards and the issue tracking system to ensure that the behavior is actually a bug, and has not already been filed.

A contributor can request to become a committer by posting a request on the PMC public email list.  If accepted, they will be given the necessary privileges for the area(s) of the request.

Committers are responsible for handling patches submitted to their areas.   This involves reading the relevant communication channel, and accepting or rejecting each submission.  In either case the submitter should be acknowledged and thanked.  In the case of rejection, the decision should be explained to the submitter.

## 5. Decision processes
### 5.1 Committer decisions
The procedure for handling submissions in a particular area is up to the committers in that area.  For example, the duty of handling submissions might be rotated among the committers.  If the committer handling a submission is uncertain about it, they should discuss it and reach consensus with the other committers.  If the committers fail to reach consensus on a submission they should forward it to the PMC.

The committers in an area must also decide on development plans in that area – for example, whether and how a new feature will be implemented.  These decisions should be made by consensus of the committers in that area, with review and discussion of the community as a whole.  If the committers fail to reach consensus on an issue they should forward it to the PMC.

### 5.2 PMC decisions
Three specific types of decisions by the PMC must be made by voting (see below).  For all other types of decisions, the PMC will attempt to decide by consensus of PMC members.  The PMC chair has responsibility of deciding when a consensus has been reached.  If the PMC chair decides that a consensus cannot be reached, they must call a vote to decide the issue.  The PMC chair is expected to conduct this process in a way that accurately reflects the opinions of the PMC as a whole, not just their own opinions.  If a PMC member feels that the chair has not done this, they can demand a vote on a particular issue.

#### 5.2.1 Decisions where voting is mandatory
Decisions of the following types must be made by a vote of the PMC:
- Intellectual property issues, e.g. those involving copyright and licensing of BOINC code.
- Other legal and financial decisions.
- PMC membership.
- Selection of the PMC chair.
- Changes to the project governance structure (i.e. changes to this document).

Votes can be called by any PMC member.  The voting process is:
- A vote is announced on the PMC public list, phrasing the issue as a yes/no decision.
- Discussion of the issue (by the entire community) takes place on the PMC public list.  Sensitive discussion among PC members uses the PMC private list.
- PMC members cast their votes publicly (by email on the PMC public list, or perhaps on a suitable web-based voting system).
- Votes on these issues are decided by agreement of at least 75% of responding voters.  The vote will be final when there is agreement of at least 75% of PMC members, or when 14 days have passed since the vote was called.  If there is not agreement of at least 75% of responding voters, no action is taken on the issue.

#### 5.2.5 Other voting decisions
Other decisions that require a PMC vote (such as committer requests not handled by consensus) will use a process similar to the above, except that only a majority (greater than 50% of responding voters) is required to make a decision, and votes are final 7 days after being called.
