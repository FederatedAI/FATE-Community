# FederatedAI Project Process Guideline

## Goal
The purpose of this document is to define the base guidelines of common project management for all projects hosted in FederatedAI. According to the TSC board, all projects in FederatedAI should follow stated governance processes, this document specifies the practices corresponding to them.

## No-Goals
This document does not cover all details of managing a project. Flexibility is a must for the project manager to set out according to the actual situations of different projects.

## Project Management Processes
### Release
* Breakthrough release may contain PR and other activities. It indicates the integral digits. e.g. 1.0, 2.0, etc.
* Major release means a release consists of major new features and/or large architectural changes. It indicates the tenth place. e.g. 1.7, 1.8, 1.9, etc.
* Minor release means a release merely a revision or a bug fix release. It indicates the hundreded place. e.g. 1.7.1, 1.7.2, etc.
* Patch means a fix may apply to releases. 

```
#.#.#.#
(Breakthrough release).(Major release).(Minor release).(Patch)
```

The community maintains the latest 2 major releases. Each major release, only maintains the latest minor release.

### Git
Gitflow (what FATE project using) is recommended:
* Create release developing branch for initial a new release following practices: deveop-%{release}%;
* Create a new feature branch for developing new a new feature;
* Project lead responsible for managing PRs merge to release developing branch; \* 
* Project lead PRs from release developing branch to master branch. **This PR has to get approval from more than half of FATE OSS Development Team members**;
* Project lead publish release from the master branch.

> **_NOTE:_**  project lead decides if contributor PR to feature branch or release developing branch. This document ignores the flexibilities in the following sections.

All commits must be signed. GPG sign is a plus.

### Development processes
All FederatedAI projects. All features, bug fixes should be added to Github issues. All PRs should be linked to related issues.
#### Gather requirements and issues
All feature requirements come from Github issue -> Feature request. 
Each project must add a *Feature request* template to the project repo.

The significant modifications expect a design proposal submitting to FederatedAI projects, for example:
* Adding a new subproject, application, dependency or component
* Any large-scale refactoring of existing subprojects or applications
* Substantial changes to a public API, UX or UI

Besides, the project lead may ask for a design proposal of feature contribution.

The issue of *Feature requirement* should be updated to add the link of the corresponding design proposal once existed.

##### Design proposal workflow (Optional)
The workflow for submitting and reviewing a new proposal is as follows:
1. A markdown file (\*.md) will be drafted for the proposal using [the template](https://github.com/FederatedAI/FATE-Community/blob/master/PROPOSAL_TEMPLATE.md);
2. A PR will be filed against [FATE-Community](https://github.com/FederatedAI/FATE-Community) in the folder *[proposal](https://github.com/FederatedAI/FATE-Community/tree/master/proposal)*;
3. The proposal will be announced in the community, and the related project will organize the meeting to discuss it;
4. Review and feedback take place on the PR, in standard PR review fashion;
5. At the end of the review period, a vote will be held. This vote will also take place on the PR. Different kinds of proposals should be different reviewers:
	- For the proposal of new subproject or matters across projects, the reviewer should be the whole TSC board, more than half of "+1" votes, the proposal will be accepted and added to the community repo;
	- For the proposal affected only one project, one reviewer is assigned by TSC board "+1" vote and the project leads "+1" vote, the proposal will be accepted and added to the community repo. 
The PR will be merged, and the label *accepted-proposal* will be added to the PR.
6. If a proposal is voted down, the PR will be left unmerged, and the label tabled-proposal will be added to the PR.

#### Discuss and created a development plan
In each release, the project manager should gather all issues (features), and PR the "Develop %{release}% Features List" to the [FATE-Community](https://github.com/FederatedAI/FATE-Community). The *"Develop_%{release}%_Features List"* should include the feature, issue id for tracing.

The project manager should organize the review meeting if necessary. 

At the end of the review period, a vote will be held. This vote will take place on the *"Develop %{release}% Features List"* PR. If the PR of release features list receives more than half of "+1" votes and the project leads "+1" vote, the feature list will be accepted and added to the community repo. The PR will be merged, and the label *accepted-proposal* will be added to the PR.

After the release features list review, the project manager should create the related development plan and add to *Github projects*. All approved issues (features) and their status should be found in related *Github projects*. 

#### Dev plan review 
The project manager hosts the bi-weekly meeting and introduces the project issues with the *Github Projects*.

#### Developing in progress
The project manager responsible for tracking the development progress in *Github Projects*. The development progress publishes to the community.

#### Before release
Corresponding to the Gitflow introduced above, the project lead is responsible for PR from the release developing branch to the master branch. This PR must receive the  of:
* more than half of the *FATE OSS Development Team* ;
* project lead followed by the approval of TSC Board.

## Tools
The community Process WG is responsible for creating related tools to facilitate the project management process in the future.
