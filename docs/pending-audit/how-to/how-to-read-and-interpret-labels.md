<!-- Reference Links ToC -->

[#intro]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#introduction
  [#toc]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#table-of-contents
[#new]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#labels-for-new-members
  [#role]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#the-role-series
  [#complexity]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#the-complexity-series
[#continuing]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#labels-for-continuing-members
  [#update]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#to-update--and-the-status-series
  [#feature]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#feature-series
  [#pfeature]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#p-feature-series
  [#dependency]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#dependency
  [#missing]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#missing-series
[#leads]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#labels-for-team-leads
  [#2weeks]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#2-weeks-inactive
  [#collab]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#collaborative-work
  [#fun]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#fun
  [#newwin]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#new-win-submission
  [#prioritization]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#ready-for-prioritization
  [#sensitive]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#time-sensitive
  [#vrms]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#transfer-to-vrms
[#unknown]: https://github.com/hackforla/website/wiki/How-to-read-and-interpret-labels#labels-of-unknown-use-or-origin


<!-- Reference Links Other -->
[#howtocommunicate]: https://github.com/hackforla/website/wiki/How-to-communicate-with-the-team
[#howtocreateissues]: https://github.com/hackforla/website/wiki/How-to-create-issues
[#projectboard]: https://github.com/hackforla/website/projects/7
[#issueapprovalcolumn]: https://github.com/hackforla/website/projects/7#column-15235217
[#howtoweeklyupdate]: https://github.com/hackforla/website/wiki/How-to-communicate-with-the-team#how-to-give-weekly-progress-updates
[#hflasitearchitecture]: https://github.com/hackforla/website/wiki/Hack-for-LA's-Site-Architecture
[#contributingmd]: https://github.com/hackforla/website/blob/gh-pages/CONTRIBUTING.md
[#hflagha]: https://github.com/hackforla/website/wiki/Hack-for-LA's-GitHub-Actions
[#hflamilestones]: https://github.com/hackforla/website/wiki/Hack-for-LA's-Milestones


# Introduction

Labels are the backbone of how we organize our massive project. Each label give a small piece of information that quickly summarizes the content of the issue before it is read. In most cases, it informs us on what to do regarding the issue without reading them, saving us tons of time and headaches. Therefore, learning about and understanding the purpose of each label is the job of everyone on the team. This guide is made to introduce you to labels, how to read them, and how to use them effectively!

The rest of this wiki will divide the labels into broad groups: labels for new members, labels for continuing members, and labels for team leads. We will also provide the following relevant information for each label:

* **Name**: `the name of a label`
* **Description**: The official description of the label
* **Default**: Whether or not the label is pre-made by GitHub
* **Usage**: Notes on how this label is used at HackForLA.
<p>&nbsp;</p>

**Note:** If you are updating this wiki and find the process painful, feel free to take up [#2228](https://github.com/hackforla/website/issues/2228) to investigate ways to automate the process!

## Table of Contents
* [Introduction][#intro]
  * [Table of Contents][#toc]
* [Labels for new members][#new]
  * [The `Role` Series][#role]
  * [The `Complexity` Series][#complexity]
* [Labels for continuing members][#continuing]
  * [`To Update !` and the `Status` Series][#update]
  * [`Feature` Series][#feature]
  * [`P-Feature` Series][#pfeature]
  * [`Dependency`][#dependency]
  * [`Missing` Series][#missing]
* [Labels for team leads][#leads]
  * [`2 weeks inactive`][#2weeks]
  * [`Collaborative Work`][#collab]
  * [`Fun`][#fun]
  * [`new-win-submission`][#newwin]
  * [`Ready for Prioritization`][#prioritization]
  * [`time sensitive`][#sensitive]
  * [`Transfer to VRMS`][#vrms]
* [Labels of unknown use or origin][#unknown]

# Labels for new members

If you are a new member at HackForLA, these are the labels you need to know to get started!

[Return to top][#toc]

## The `Role` Series

At HackForLA, we have many roles, such as administrators, user researchers, and more. When looking for an issue to work on, besides looking in the [Prioritized backlog](https://github.com/hackforla/website/projects/7#column-7198257), you must also be able to differentiate between issues that are for a developer vs for other teams. Our role labels are used to mark the role that the issue is for. You will recognize these labels because they are prefixed with `role: [name of role]`, for example `role: design`. The following are the role labels we have.

[Return to top][#toc]

* **Name**: `Role: Administrative`
* **Description**: 
* **Default**: no
* **Usage**: Rarely used label, but indicates issues that requires someone with leadership level permissions to resolve.
<p>&nbsp;</p>

* **Name**: `role: back end/devOps`
* **Description**: Tasks for back-end developers
* **Default**: no
* **Usage**: Denotes issues relating to our site architecture as well as support programs that are used outside of our website. Only take this issue if you are a developer.
<p>&nbsp;</p>

* **Name**: `role: design`
* **Description**: 
* **Default**: no
* **Usage**: Denotes issues for designers, usually involving creating prototypes and mock-ups on our Figma. Only take this issue if you are a designer.
<p>&nbsp;</p>

* **Name**: `role: front end`
* **Description**: Tasks for front end developers
* **Default**: no
* **Usage**: Denotes tasks that involves edits to our website's HTML, CSS, and JS code. Only take this issue if you are a developer.
<p>&nbsp;</p>

* **Name**: `role: legal`
* **Description**: 
* **Default**: no
* **Usage**: Rarely used label, but indicates an issue that requires someone with legal expertise to resolve.
<p>&nbsp;</p>

* **Name**: `role: product`
* **Description**: Product Management
* **Default**: no
* **Usage**: Denotes issues that involves work relating to the quality of the website, and interfacing with stakeholders. Only take this issue if you are a product manager.
<p>&nbsp;</p>

* **Name**: `role: user research`
* **Description**: 
* **Default**: no
* **Usage**: Denotes issues for user researchers. Usually involves gathering information from stakeholders. Only take this issue if you are a user researcher.
<p>&nbsp;</p>

* **Name**: `role: writing`
* **Description**: Tasks for writers
* **Default**: no
* **Usage**: Denotes issues that involves any kind of documentation writing, such as this wiki! Anyone can be a writer, so feel free to take up these issues anytime!
<p>&nbsp;</p>

## The `Complexity` Series

The `Complexity` series represents the overall time commitment and difficulty of an issue. At HackForLA, all newcomers start with a `good first issue` and `complexity: good second issue` as training before they have the freedom to take issues of a much higher complexity. The following lists the all of our complexity labels from smallest to largest.

[Return to top][#toc]

* **Name**: `good first issue`
* **Description**: Good for newcomers
* **Default**: yes
* **Usage**: Issues that are reserved to our newest members. This should be your first official issue! Most issues of this complexity involves changing only one small line of code.
<p>&nbsp;</p>

* **Name**: `Complexity: Good second issue`
* **Description**: 
* **Default**: no
* **Usage**: Issues that are reserved to our newest members after completion of a `good first issue`. This should be your second official issue! Most issues of this complexity involves changing a few lines of code.
<p>&nbsp;</p>

* **Name**: `Complexity: Small`
* **Description**: Take this type of issue after the successful merge of your good second issue
* **Default**: no
* **Usage**: Our smallest general issue. This is only for small changes such as a bug fix, or a small feature.
<p>&nbsp;</p>

* **Name**: `Complexity: Medium`
* **Description**: 
* **Default**: no
* **Usage**: Our mid-complexity general issue. Medium issues usually involves about an hour to five hours of work, depending on experience. Issues here are straightforward but often involves multiple files.
<p>&nbsp;</p>

* **Name**: `Complexity: Large`
* **Description**: 
* **Default**: no
* **Usage**: Very free-form issues. Large issues demands a high time commitment, as well as vague requirements. Large issues will test your creativity and perseverance, and, most importantly, your ability to ask for help when needed.
<p>&nbsp;</p>

# Labels for continuing members

These are labels you need to know once you have completed your `Good first issue` and `Complexity: good second issue`. This means you have finished the tutorials to initiate yourself into the team, and are ready to flex your coding muscles💪.

[Return to top][#toc]
 

## `To Update !` and the `Status` Series

These labels go hand in hand with one another and serves to help members asynchronously communicate the status on their issues. They are chiefly used to improve communication with the team. These labels enables us to help one another despite being volunteers with different work/life/volunteer schedules. To learn more about communication with the team, please visit [this page][#howtocommunicate].

[Return to top][#toc]

* **Name**: `To Update !`
* **Description**: No update has been provided
* **Default**: no
* **Usage**: This label indicates that a an issue had not had updates for a while and we would like to know what is going on. The goal here is to not be intrusive, but to quickly locate team members that need help, and provide a platform to communicate their needs and current status. This label is automatic, and should never be added manually.
<p>&nbsp;</p>

* **Name**: `Status: Updated`
* **Description**: No blockers and update is ready for review
* **Default**: no
* **Usage**: This label is used to indicate that an update has been made on an issue. This label is always added manually when instructed to do so, so please do not use it randomly!
<p>&nbsp;</p>

* **Name**: `Status: Help Wanted`
* **Description**: Internal assistance is required to make progress
* **Default**: no
* **Usage**: This label can be used whenever you need help! Is your blocker big? Add this label. Is it small? Add this label. When a team member notices this label, they will come along like a check-in fairy and find out what is going on. Conversely, if you see this label on an issue, it is a good chance for you to practice being a a mentor fairy for someone!
<p>&nbsp;</p>


## `Feature` Series

The `Feature` series and the `P-feature` series (see [below][#pfeature]), go hand in hand with one another. These labels indicates, broadly, what the issue involves. For example, an issue marked with `Feature: Accessibility` means that the issue relates to the accessibility of our website or our repository. The main difference between `Feature` and `P-feature` is that the `P-feature` series are reserved for the pages of our website that the issue concerns, while `Feature` involves activity outside of our website's pages. Normally, a new developer does not need to know about these labels at all. However, continuing members are expected to create issues, and these labels are required when creating a new issue. For more information on issue creation, visit [this page][#howtocreateissues].

[Return to top][#toc]

<details>
<summary>Click to open</summary>
<br>

* **Name**: `Feature: Accessibility`
* **Description**: Issues that would broaden website accessibility
* **Default**: no
* **Usage**: This label is used for anything accessibility related, such as performing an audit of alt text throughout the website.
<p>&nbsp;</p>

* **Name**: `Feature: Administrative`
* **Description**: Administrative chores etc.
* **Default**: no
* **Usage**: A label that goes hand in hand with the `role: administrator` label. This means the issue involves altering something only accessible to admins, such as our repository settings.
<p>&nbsp;</p>

* **Name**: `Feature: Analytics`
* **Description**: google analytics
* **Default**: no
* **Usage**: For issues that involves Google analytics or something similar. Usually involves something data intensive.
<p>&nbsp;</p>

* **Name**: `Feature: Board/GitHub Maintenance`
* **Description**: Project board maintenance that we have to do repeatedly
* **Default**: no
* **Usage**: For issues involving organizing our GitHub repository, such as our [project board] [#projectboard]
<p>&nbsp;</p>

* **Name**: `Feature: Infrastructure`
* **Description**: For changes on site technical architecture
* **Default**: no
* **Usage**: For issues involving changing our site [architecture][#hflasitearchitecture].
<p>&nbsp;</p>

* **Name**: `Feature: Onboarding/Contributing.md`
* **Description**: 
* **Default**: no
* **Usage**: For issues involving our [CONTRIBUTING.md][#contributingmd]
<p>&nbsp;</p>

* **Name**: `Feature: Refactor CSS`
* **Description**: Page is working fine - CSS needs changes to become consistent with other pages
* **Default**: no
* **Usage**: For issues involving refactoring our CSS code.
<p>&nbsp;</p>

* **Name**: `Feature: Refactor GHA`
* **Description**: Refactoring GitHub actions to fit latest architectural norms
* **Default**: no
* **Usage**: For issues involving refactoring our [GitHub actions][#hflagha].
<p>&nbsp;</p>

* **Name**: `Feature: Refactor HTML`
* **Description**: 
* **Default**: no
* **Usage**: For issues involving refactoring our HTML.
<p>&nbsp;</p>

* **Name**: `Feature: Refactor JS / Liquid`
* **Description**: Page is working fine - JS / Liquid needs changes to become consistent with other pages
* **Default**: no
* **Usage**: For issues involving refactoring our JS code or liquid syntax.
<p>&nbsp;</p>

* **Name**: `Feature: Wiki`
* **Description**: 
* **Default**: no
* **Usage**: For issues involving our wiki. If you are reading this, you are at our wiki!
<p>&nbsp;</p>

<br>
</details>

## `P-Feature` Series

The `P-Feature` series go together with the `Feature` series (see [above][#feature]). In general, each label of the `P-Feature` series involves either a page on our website, or a reusable component.

[Return to top][#toc]

<details>
<summary>Click to open</summary>
<br>

* **Name**: `P-Feature: 404 page`
* **Description**: https://www.hackforla.org/404
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: About Us`
* **Description**: https://www.hackforla.org/about/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Communities of Practice`
* **Description**: https://www.hackforla.org/communities-of-practice
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Credit`
* **Description**: https://www.hackforla.org/credits/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Donate`
* **Description**: https://www.hackforla.org/donate/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Events`
* **Description**: https://www.hackforla.org/events/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Footer`
* **Description**: 
* **Default**: no
* **Usage**: Used for edits to our footer component.
<p>&nbsp;</p>

* **Name**: `P-Feature: Getting Started`
* **Description**: https://www.hackforla.org/getting-started
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Home page`
* **Description**: https://www.hackforla.org/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Impact`
* **Description**: 
* **Default**: no
* **Usage**: This is for our future impact page.
<p>&nbsp;</p>

* **Name**: `P-Feature: Join Page`
* **Description**: https://www.hackforla.org/join
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Navigation`
* **Description**: 
* **Default**: no
* **Usage**: Used for edits to our navbar component.
<p>&nbsp;</p>

* **Name**: `P-Feature: Program Area`
* **Description**: https://www.hackforla.org/program-areas
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Project Info and Page`
* **Description**: A project's detail page (e.g. https://www.hackforla.org/projects/100-automations)
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Project Meetings`
* **Description**: https://www.hackforla.org/project-meetings
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Projects page`
* **Description**: https://www.hackforla.org/projects/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Sitemap`
* **Description**: https://www.hackforla.org/sitemap/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Toolkit`
* **Description**: https://www.hackforla.org/toolkit/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Wins Page`
* **Description**: https://www.hackforla.org/wins/
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

<br>
</details>


## Dependency

A dependency means that an issue requires some other work to be finished before this issue can start. For example, if we need to create a new component, but we are in the middle of reorganizing our CSS, it is not best to create a new component now. Therefore, we need to add a `Dependency` label to indicate that there is CSS work (the dependency) that needs to resolve before work can start. For more about dependencies, take a look at [our wiki on issues and issue creation][#howtocreateissues].

[Return to top][#toc]

* **Name**: `Dependency`
* **Description**: An issue is blocking the completion or starting of another issue
* **Default**: no
* **Usage**: A label that is placed on any issue with a dependency, meaning another issue needs to be resolved before work can begin.
<p>&nbsp;</p>


## `Missing` Series

Missing labels are important to know for issue creators. These missing labels indicate that a label of a certain series is missing from the issue. More information on this can be found on [our wiki on issues and issue creation][#howtocreateissues].

[Return to top][#toc]

* **Name**: `dependency missing`
* **Description**: 
* **Default**: no
* **Usage**: Rarely used, but indicates that an issue has a missing dependency in its description. Usually, a comment on the issue will clarify what edits to the description are needed.
<p>&nbsp;</p>

* **Name**: `Feature Missing`
* **Description**: This label means that the issue needs to be linked to a precise feature label.
* **Default**: no
* **Usage**: This label means that either a `Feature` or `P-Feature` series label is missing from the issue. Chiefly used by leadership to mark issues that are missing labels and indicates that the issue creator needs to add the missing label.
<p>&nbsp;</p>

* **Name**: `complexity: missing`
* **Description**: 
* **Default**: no
* **Usage**: This label means that a `Complexity` series label is missing from the issue. Chiefly used by leadership to mark issues that are missing labels and indicates that the issue creator needs to add the missing label.
<p>&nbsp;</p>

* **Name**: `role missing`
* **Description**: 
* **Default**: no
* **Usage**: This label means that a `Role` series label is missing from the issue. Chiefly used by leadership to mark issues that are missing labels and indicates that the issue creator needs to add the missing label.
<p>&nbsp;</p>


# Labels for team leads

These are the labels you need to know once you have made it to the team lead level (congratulations 🥳).

[Return to top][#toc]

## `2 weeks inactive`

The `2 weeks inactive` label is automatically placed on an issue. It indicates that no updates had been made on an assigned issue, and signals that the assignee might be stuck. The action to take after noticing this label is to 1) contact the assignee to find out if they are still working on the issue and 2) if no response is made after 3 days, recycle the issue back into the prioritized backlog (closing out the PR, if needed). For more about making updated on issue, check out [this wiki][#howtoweeklyupdate].

* **Name**: `2 weeks inactive`
* **Description**: 
* **Default**: no
* **Usage**: Added automatically to inactive issues. Do not add this manually.
<p>&nbsp;</p>

[Return to top][#toc]


## `Collaborative Work`

This label is used chiefly to allow a team member to work on multiple issues at once, and subvert the usual one issue per member rule. Issues with this label cannot be worked on alone, but requires either the cooperation or supervision of another developer. Only leads can assign this label to an issue, based on their judgment, and often the lead would appoint a special junior member on such issues. This is usually placed on work that not of the highest priority, but requires an unusually long time to complete, often involving extensive testing, research, and shifting requirements.

* **Name**: `Collaborative Work`
* **Description**: Work to be completed during meeting times
* **Default**: no
* **Usage**: Only to be added by a lead to note work that requires multiple developers. This allows a developer to work on a second issue.
<p>&nbsp;</p>

[Return to top][#toc]


## `Fun`

The `Fun` came out of a need to have an optional third issue after the first and second. Issues with this label are simple, and straightforward, yet gives the team member a chance to flex and learn. This issue was created as part of our internship program, and makes it easier to interns to ease into our team. This label is usually unused outside of internship season. Note: this is not part of the `Complexity` series--it is just a fun, optional label.

* **Name**: `Fun`
* **Description**: Congrats!  You finished your good first and second issues.  Please only do one of these
* **Default**: no
* **Usage**: To be added on `Complexity: Small` or `Complexity: Medium` issues that ease new team members into the team. Usually only used during internship season.
<p>&nbsp;</p>

[Return to top][#toc]


## `new-win-submission`

This label is an automatic label used only on an automatic issue. This issue, the wins-submission-issue, means that a new wins submission was made, and requires review by the product team. The product team who takes up this issue, will go to the wins spreadsheet in our admin drive, and make a decision on whether the new submission should be displayed or not.

* **Name**: `new-win-submission`
* **Description**: None
* **Default**: no
* **Usage**: Placed automatically, and only on an issue for the product team.
<p>&nbsp;</p>

[Return to top][#toc]


## `Ready for Prioritization`

The `Ready for Prioritization` label is a label chiefly used to mark that an issue is of good quality and is ready to be approved for adding to the backlog. You can learn more about this label from [our wiki on issue creation][#howtocreateissues]. This gist of this label is that it is added to issues on the ["New Issue Approval" column][#issueapprovalcolumn] to signal to the product team that the issue has been created and edited by the other teams. Only team leads should ever put on this label as they are responsible for editing issues.

* **Name**: `Ready for Prioritization`
* **Description**: 
* **Default**: no
* **Usage**: Only to be used by a lead on issues in the Issue approval column. It is only used to indicate that an issue is fully-formed according to the standards of the team lead.
<p>&nbsp;</p>

[Return to top][#toc]


## `time sensitive`

This label is not to be of concern to anyone besides the product team. This label is placed on issues that are considered of high importance *relative to the milestone* (to learn more about milestones, visit our wiki [about milestones][#hflamilestones]). This means that an issue marked with a milestone, say 03, is only considered important against all other 03 milestone issues. This label is chiefly used by the product team.

* **Name**: `time sensitive`
* **Description**: Needs to be worked on by a particular time-frame
* **Default**: no
* **Usage**: Only used by the product team to mark issues that are of great importance when compared to other issues of the same milestone.
<p>&nbsp;</p>

[Return to top][#toc]


## `Transfer to VRMS`

This rarely-used label are for issues that requires transferred to another project, because they have been erroneously made in our repository. This label is created because not every member of the team has the permissions to perform issue transfers.

* **Name**: `Transfer to VRMS`
* **Description**: Needs to be transferred from the hfla website GitHub repo to the VRMS GitHub repo
* **Default**: no
* **Usage**: Can be added by anyone to an issue that does not belong in our repository. This will signal to an admin team member to move the issue to the appropriate repository.
<p>&nbsp;</p>

[Return to top][#toc]


# Labels of unknown use or origin

These labels are labels whose use is very rare and overlap with other labels. Most of these labels were created a long time ago and so their use has become muddled as the website evolved. Some of them might even be used erroneously! For all intents an purposes, these labels are not to be used, and should be audited. The state of these labels are liable to change as part of [#1983](https://github.com/hackforla/website/issues/1983).

[Return to top][#toc]

<details>
<summary>Click to open</summary>
<br>

* **Name**: `automation`
* **Description**: for manual github board maintenance actions that are going to be automated
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Blockers`
* **Description**: Factors are preventing progress
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Bug`
* **Description**: Something isn't working
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Dependencies`
* **Description**: Pull requests that update a dependency file
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Discussion`
* **Description**: Starting point for gathering further information and/or feedback
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `documentation`
* **Description**: Documentation creation
* **Default**: yes
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `duplicate`
* **Description**: This issue or pull request already exists
* **Default**: yes
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `enhancement`
* **Description**: New feature or request suggestion
* **Default**: yes
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `external info needed`
* **Description**: Need more information before proceeding
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Feature: Design system`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Feature: Feature Branch`
* **Description**: Requires Branching off a Feature Branch instead of gh-pages
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Feature: Standards`
* **Description**: 
* **Default**: no
* **Usage**:
<p>&nbsp;</p>

* **Name**: `Feature: Tables`
* **Description**: We are going to use Tables to try to manage all HfLA members (including automating onboarding)
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `HOLD`
* **Description**: Not ready to be worked on yet
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Issue Incomplete`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `need more info to release to backlog/icebox`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Contact forms w usability research`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Contributors`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Open roles`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Organizational Page`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `P-Feature: Privacy Policy`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `p-feature: program area detail page`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Ready for dev issue`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Research`
* **Description**: Tasks for researchers
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `role: hfla leadership`
* **Description**: Any issue that the blocker is a resource controlled by HfLA leadership
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `Status: Urgent`
* **Description**: Needs to be worked on immediately
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `test`
* **Description**: None
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `UAT: has visuals`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `UAT: no visuals`
* **Description**: 
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `User Acceptance Testing`
* **Description**: Ready to be tested after review
* **Default**: no
* **Usage**: 
<p>&nbsp;</p>

* **Name**: `wontfix`
* **Description**: This will not be worked on
* **Default**: yes
* **Usage**: 
<p>&nbsp;</p>

<br>
</details>