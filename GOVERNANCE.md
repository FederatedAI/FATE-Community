# **FATE GOVERNANCE** #

This document defines the project governance for FATE.
# Principles #
The FATE community adheres to the following principles:

- Open: FATE is an open source project.
- Welcoming and respectful: See[ Code of Conduct](./CODE_OF_CONDUCT.md). 
- Transparent and accessible: Work and collaboration are done in public.
- Merit: Ideas and contributions are accepted according to their technical merit and alignment with project objectives, scope, and design principles.
- Vision: Benefit the ecosystem of federated AI solution providers, users and researchers, focused on federated AI use cases that will work across industries.

# Changes in Maintainership #
## Process for becoming a maintainer ##
- Express interest to the maintainers that you are interested in becoming a maintainer. 
- We will expect you have domain expertise.
- We will expect you to start contributing some PRs, under the guidance of the existing maintainers.
- As you gain experience with the code base and our standards, we will expect you to do some code reviews for incoming PRs and answer questions from community.
- After a period of time working together, the existing maintainers will confer and decide whether to grant maintainer status or not. New maintainers are nominated by an existing maintainer and are elected by a 1/2 majority of existing maintainers vote.
## When does a maintainer lose maintainer status ##
- If a maintainer is no longer interested or cannot perform the maintainer duties, they are free to step down.
- A maintainer will never be removed forcefully, unless they fail to meet the principles of FATE community or adhere to the Code of Conduct.
- In extreme cases this can also occur by voting process. Maintainers can be removed by a 1/2 majority of existing maintainers vote.
# Decision making and voting #
- The project aims to operate as a consensus-based community, and decisions are built on the agreement reached by maintainers. Proposals and ideas for agreement can either be submitted via a GitHub issue or PR, or by sending an email to [FedAI-maintainers@groups.io](https://groups.io/g/FedAI-maintainers).
- Decision making process should be transparent to adhere to the principles of FATE project.
- If any decision requires a vote to move the Project forward, maintainers will vote on a one vote per voting maintainer basis.
- Quorum for voting requires all voting maintainers to participate. 
- Any decisions require to be supported by a majority approval of maintainers vote.
- For formal votes, a specific statement of what is being voted on should be added to the relevant GitHub issue or PR, and a link to that issue or PR should be added to the maintainers meeting agenda document. Maintainers should indicate their yes/no vote on that issue or PR, and after a reasonable period of time, the votes will be tallied and the outcome will be noted.
- All proposals, ideas, and decisions made by maintainers should either be part of a GitHub issue or PR.
# Maintainer responsibilities #
- Making a community work requires input/effort from everyone. Maintainers should actively participate in Pull Request reviews. Maintainers are expected to respond to assigned Pull Requests in a reasonable time frame, either providing insights, or assigning it to other maintainers. And make sure that ongoing PRs are moving forward at the right pace or close them.
- Diligently providing supports (via mailing list, GitHub, slack, email, WeChat, etc.), answering questions，responding to requests and replying to bugs, etc.
- Publishing releases
- Fixing bugs
- Writing and updating documentation for usage and development
- Getting the word out and making your project known 
- Monitoring the improper speech and behavior of the community and dealing with community conflicts and disputes. 
# Project #
## Release cadence ##
- Our current release cycle is intended to be two months. We may change this based on user demand.
- In general, master is assumed to be release candidate quality at all times for documented features. For undocumented or clearly under development features, use caution or ask about current status when running master.
## Proposal Process ##
Significant changes to the codebase and / or new features must be first discussed and weighed, and sometimes formally documented, before they can be implemented. The process for proposal informs and involves all the members of the community in major improvements to the codebase and / or new features throughout the development process, to increase their sharing comments and ideas and offering to help.

The proposal process is the process for reviewing a proposal and reaching an agreement on whether to accept or decline the proposal.

**Design Documents**

The proposal should be documented as a separated markdown file pushed to the root of the `proposals` folder in the community repository via PR. The name of the file should follow the name pattern `design/shortname.md`.
Use the [Proposal Template](./PROPOSAL_TEMPLATE.md) as a starting point.

**Proposal lifecycle**  
The proposal PR can be marked with different status labels to represent the status of the proposal:

- **New**: Proposal is just created
- **Reviewing**: Proposal is under review and discussion
- **Accepted**: Proposal is reviewed and accepted (either by consensus or vote)
- **Rejected**: Proposal is reviewed and rejected (either by consensus or vote)

**Proposal Review**

The maintainers hold “proposal review meetings” approximately weekly to review pending proposals.

The principal goal of the review meeting is to make sure that proposals are receiving attention from the right people, by cc'ing relevant developers, raising important questions, pinging lapsed discussions, and generally trying to guide discussion toward agreement about the outcome. The discussion itself is expected to happen on the issue tracker, so that anyone can take part in.

Once comments and revisions on the design doc wind down, there is a final discussion on the issue, to reach one of two outcomes:

- Accepted proposal or
- Declined proposal

After the proposal is accepted, implementation work proceeds in the same way as any other contribution.

## Adding new sub-project to the FATE GitHub organization ##
The `Federated AI Ecosystem` organization is open to receive new sub-projects under its umbrella. To apply a project as part of the Federated AI Ecosystem organization, it has to meet the following criteria:

- Licensed under the terms of the Apache License v2.0
- Project has been active for at least one year since its inception
- Related to one or more scopes of FedAI ecosystem:
	- Federated machine learning
	- Federated transfer learning
	- Federated data network
	- Federated inference
	- Federated machine learning on Edge
	- Federated learning workload management using cloud native technologies
	- Multi-party security protocol
	- …
- Be supported by 2/3 majority of the existing maintainers

The submission process starts a Pull Request or Issue with the required information mentioned above. Once a project is accepted, it's considered as a Federated AI Ecosystem sub-project under the umbrella of Federated AI Ecosystem.
## Contributing ##
Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for general contribution guidelines
## Code of Conduct ##
FATE adhere to the [Code of Conduct](./CODE_OF_CONDUCT.md).
# Updating Governance #
All substantive changes in Governance require total Maintainership vote supported by 1/2 majority of existing maintainers.

