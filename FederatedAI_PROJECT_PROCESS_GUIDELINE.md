# FederatedAI Project Process Guideline

## Goal
The purpose of this document is to define the base guidelines of common project management for all projects hosted in FederatedAI. According to the TSC board, all projects in FederatedAI should follow stated governance processes, this document specifies the practices corresponding to them.

## No-Goals
This document does not cover all details of managing a project. Flexibility is a must for the project manager to set out according to the actual situations of different projects.

## Roles
* Project lead
* Project manager
* Feature developer

## Project Management Processes
### Release
* Major release means a release consists of major new features and/or large architectural changes. It indicates the tenth place. e.g. 1.7, 1.8, 1.9, etc.
* Minor release means a release merely a revision or a bug fix release. It indicates the hundreded place. e.g. 1.7.1, 1.7.2, etc.

```
#.#.#
(Integer release).(Major release).(Minor release)
```

The community maintains the latest 2 major releases. Each major release, only maintains the latest minor release.

### Git
Gitflow (what FATE project using) is recommended:
* The project lead creates a *release developing branch* for initial a new release following practices: develop-%{release}%;
* The feature developer creates a new *feature branch* for developing a new feature;
* The project lead is responsible for managing PRs merge to the *release developing branch* with SIG on Security (SIGoS)' approval; [Ref: Before merging a PR to the *release developing branch*](#before-merging-a-pr-to-release-developing-branch); \* 
* The project lead PRs from the *release developing branch* to the *master branch* with the community's approval [Ref: Before release](#before-release);
* The project lead publishes release from the *master branch*.

> **_NOTE:_**  the project lead decides if contributor PR to the *feature branch* or the *release developing branch*. This document ignores the flexibilities in the following sections.

All commits must be signed by the contributor. A GPG sign is a plus.

### Development processes
All FederatedAI projects. All features, bug fixes should be added to Github issues. All PRs should be linked to related issues. The PR should be set to require review.
#### Gather requirements and issues
All feature requirements come from Github issue -> Feature request. 
Each project must add a *Feature request* template to the project repo.

The significant modifications expect a design proposal submitting to FederatedAI projects, for example:
* Adding a new subproject, application, dependency or component
* Any large-scale refactoring of existing subprojects or applications
* Substantial changes to a public API, UX or UI

Besides, the project lead may ask for a design proposal of feature contribution.

The issue of *Feature request* should be updated to add the link of the corresponding design proposal once existed.

##### Design proposal workflow (Optional)
The workflow for submitting and reviewing a new proposal is as follows:
1. A markdown file (\*.md) will be drafted for the proposal using [the template](https://github.com/FederatedAI/FATE-Community/blob/master/PROPOSAL_TEMPLATE.md);
2. A PR will be filed against [FATE-Community](https://github.com/FederatedAI/FATE-Community) in the folder *[proposal](https://github.com/FederatedAI/FATE-Community/tree/master/proposal)*;
3. The proposal will be announced in the community, and the related project will organize the meeting to discuss it;
4. Review and feedback take place on the PR, in standard PR review fashion;
5. At the end of the review period, a vote will be held. This vote will also take place on the PR. Different kinds of proposals should be different reviewers:
	- For the proposal of new subproject or matters across projects, the reviewer should be more than half of the FATE OSS Development Team members "approve" votes, the proposal will be accepted and added to the community repo;
	- For the proposal affected only one project, one reviewer is assigned by TSC board "approve" vote and the project leads "approve" vote, the proposal will be accepted and added to the community repo. 
The PR will be merged, and the label *accepted-proposal* will be added to the PR.
6. If a proposal is voted down, the PR will be left unmerged, and the label tabled-proposal will be added to the PR.

#### Discuss and created a development plan
In each release, the project manager should filter the issues of *feature requests* and organize a meeting to gather all issues (features), and PR the *"Develop_%{release}%_Features_List"* to the [FATE-Community](https://github.com/FederatedAI/FATE-Community) *Features_List* folder. The *"Develop_%{release}%_Features_List"* should include the feature, issue id for tracking.

The project manager should organize the review meeting if necessary. 

At the end of the review period, a vote will be held. This vote will take place on the *"Develop_%{release}%_Features_List"* PR. If the PR of release features list receives more than half of the "approve" votes and the project leads "approve" vote, the feature list will be accepted and added to the community repo. The PR will be merged, and the label *accepted-proposal* will be added to the PR.

After the release features list review, the *"Develop_%{release}%_Features_List"* will be triaged to stories or tasks and add them to *Github projects*. All approved issues (features) and their status should be found in related *Github projects*. 

The SIGoS labels *security_check_required* to the issues (features) which need special security checks during the review period. 

#### Dev plan tracking 
The project manager hosts the bi-weekly meeting and introduces the project issues with the *Github Projects*.

#### Developing in progress
The project manager is responsible for tracking the development progress in *Github Projects*. The development progress publishes to the community.

#### Before merging a PR to *release developing branch*
After a feature finishes development, the project lead is responsible for merging the PR from the *feature branch* to the *release developing branch*. But all PRs linked to the feature issues, which are labeled *security_check_required* must pass the security checks processed by SIGoS and be labeled *security_approved* before merging to the *release developing branch*.

#### Before release
Corresponding to the Gitflow introduced above, the project lead is responsible for PR from the *release developing branch* to the *master branch*. This PR must receive the of:
* more than half of the *FATE OSS Development Team*;
* project lead followed by the approval of TSC Board.

Because FATE project consists of several subprojects, once FATE got approval for a new release, all the subprojects (e.g. FATE-Board, FATE-Flow, etc.) are derived the approval from the FATE project. Only FATE-Serving and KubeFATE requires seperated approvals by now.

If only a subproject (e.g. FATE-Board) needs to be published a new release, it still needs the approval process. 

#### Exceptionals
##### Additional features or fixes add to developing release
The features and fixes must come from Github issues, or the project manager responsible for creating related issues. The issues should be added to *Github projects* for tracking. 

If the features and fixes miss the windows of development, they should follow the process of creating a new release.

##### Fixes patch to old release
If there is a patch that needs to apply to old but supporting release, the development team is suggested to follow the process:
* The project lead creates a *release developing branch* for initial a new release following practices: develop-%{release}%;
* The feature developer creates a new *feature branch* for developing a new feature;
* The project lead is responsible for managing PRs merge to the *release developing branch* with SIG on Security (SIGoS)' approval; [Ref: Before merging a PR to the *release developing branch*](#before-merging-a-pr-to-release-developing-branch); \* 
* The project lead responsible for creating a *patch release branch*: release-%{release}%;
* The project lead PRs from the *release developing branch* to the *patch release branch* with the community's approval [Ref: Before release](#before-release);
* The project lead publishes release from the *patch release branch*.

## Tools
The community Process WG is responsible for creating related tools to facilitate the project management process in the future.
