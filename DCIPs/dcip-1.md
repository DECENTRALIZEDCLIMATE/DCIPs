---
dcip: 1
title: Purpose and Guidelines
status: Living
type: Standards Track
author: David E. Perez Negron R. User (@p1r0)
category: Core
created: 2023-06-26
layout: post
--- 

## Simple Summary

DCIP-01, specifies what is an DCIP (Decentralized Climate Improvement Porposals) and how to write one.


## Abstract

This proposal specifies a standard and a best practice guide to create DCIPs,
what a DCIP should include as a minimum requirement, their life cycle, and workflow for making the decentralized climate foundation and its projects operate in the most collaborative and decentralized manner through its DAO Governance Model.


## DCIP Motivation

The goal of the Decentralize Climate Foundation is to be as Decentralized as posible, these also includes its organization, governance, operations, projects development and even founding.

The Decentralized Climate Fundation base philosophy is considering that by bringing together a diversity of perspectives and encouraging open, evidence-based discussion, it is possible to reach better decisions and minimize corruption and mistakes. The Decentralized Climate Foundation seeks to take advantage of collective wisdom and challenge individual biases through a participatory and transparent process.

The Decentralized Climate Foundation aims to operate in a decentralized manner, involving various participants in its governance and projects. It seeks to promote inclusion, transparency and informed participation to make evidence-based decisions and avoid corruption. Through a decentralized governance model, quadratic and rating voting mechanisms, openness in its operations and continuous evaluation, the foundation seeks to take advantage of the diversity of perspectives and knowledge to address climate change effectively.



## Specification: Work Flow

The workflow begins with discussing and drafting improvement proposals on the DCF forum, where participants engage in commenting, brainstorming, and reaching a consensus. Once a proposal is ready, it undergoes a voting stage within the community. If the proposal doesn't receive approval, further discussion and potential changes are encouraged. This iterative process continues until the proposal either gets approved or is blacklisted by the majority to prevent spam. Existing proposals can also be modified based on suggestions and submitted for voting. Approved proposals are added to a pull request in the "Decentralized Climate Proposal" project, serving as a repository for all proposals. The pull request follows the Git Flow model, ready for the next release on the development branch. This concise description highlights the key steps and the role of the DCF forum, voting process, and pull requests in the overall lifecycle of the improvement proposals.


### DCIP Actors

Shepherding an DCIP

![](/assets/dcip-1/Img1.svg)

Img 1. DCIP Actors Interaction with the DCIPs Process.

Parties involved in the process are the DCIP author (you), the DCIP editors, and the Decentralized Climate Foundation Members.

Before you begin writing a formal DCIP, you should vet your idea. Ask the Decentralized Climate Foundation community first if an idea is original to avoid wasting time on something that will be rejected based on prior research. It is thus recommended to open a discussion thread on the [DCF forum](https://forum.decentralizedclimate.org) to do this.

*In short, your role is to write the DCIP using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea.*


### DCIP Process

![](/assets/dcip-1/Img2.svg)

Img 2. A DCIP Process as an Activity Diagram.

1. The process begins with the discussion of an idea in the forum associated with the system. Participants engage in brainstorming and consensus-building to refine the idea.

2. Once the draft of the proposal is considered ready, a fork of the DCIP repository is created, and the proposal draft is posted in the forked repository.

3. The improvement proposal in the forked repository is submitted for voting. Participants determine its approval status through a voting phase.

4. If the proposal is approved, it is merged into the main DCIP repository, officially accepting and incorporating it into the system.

5. If the proposal is not approved, two branches are followed. In one branch, participants engage in further discussion and make changes to address feedback and concerns. The modified proposal is resubmitted for voting, continuing the iterative process until it receives approval.

6. In the other branch, participants have the option to vote for blacklisting the proposal. If the majority votes for blacklisting, the proposal is marked as blacklisted, indicating it will not be considered further or included in the system.

7. The process continues in a loop until the proposal is either approved or blacklisted.

8. Once the proposal is merged into the DCIP repository, the process concludes, and the proposal becomes part of the system.


## DCIP Status

![](/assets/dcip-1/Img3.svg)

Img 3. Possible Status of a Improvement Proposal

1. **Draft**: This is the initial status of a proposal. It represents the stage where the proposal is being drafted and prepared for submission.

2. **Ready**: Once the proposal is deemed ready for evaluation and voting, it transitions to the "Ready" status. At this stage, the proposal is considered complete and eligible for review.

3. **Under Review**: When the proposal is submitted for voting, it enters the "Under Review" status. This status indicates that the proposal is currently being evaluated by the community or relevant stakeholders.

4. **Approved**: If the proposal receives the necessary approval votes, it transitions to the "Approved" status. This status indicates that the proposal has been accepted and endorsed by the community.

5. **Changes Required**: If feedback or concerns are raised during the voting process, the proposal may be deemed in need of changes. In such cases, it moves to the "Changes Required" status, indicating that modifications or revisions are necessary.

6. **Blacklisted**: In certain situations, a proposal may be deemed inappropriate or unsuitable for inclusion. If the majority votes to blacklist the proposal, it moves to the "Blacklisted" status. This status signifies that the proposal has been rejected and will not be further considered.

7. **Merged**: Once an approved proposal successfully undergoes the necessary procedures, such as merging into the DCIPs repository, it reaches the "Merged" status. This status indicates that the proposal has been officially incorporated into the system and its changes have been applied.


## What belongs in a successful DCIP?

Each DCIP should have the following parts:

- Preamble - RFC 822 style headers containing metadata about the DCIP, including the DCIP number, a short descriptive title (limited to a maximum of 44 characters), a description (limited to a maximum of 140 characters), and the author details. Irrespective of the category, the title and description should not include DCIP number. See [below](./dcip-1.md#dcip-header-preamble) for details.
- Abstract - Abstract is a multi-sentence (short paragraph) technical summary. This should be a very terse and human-readable version of the specification section. Someone should be able to read only the abstract to get the gist of what this specification does.
- Motivation *(optional)* - A motivation section is critical for DCIPs that want to change the Decentralized Climate Foundation Governance. It should clearly explain why the existing protocol specification is inadequate to address the problem that the DCIP solves. This section may be omitted if the motivation is evident.
- Specification - The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for any of the current Decentralized Climate Foundation platforms (Forum, Snapshot, AragonDAO, Sheets).
- Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale should discuss important objections or concerns raised during discussion around the DCIP.
- Backwards Compatibility *(optional)* - All DCIPs that introduce backwards incompatibilities must include a section describing these incompatibilities and their consequences. The DCIP must explain how the author proposes to deal with these incompatibilities. This section may be omitted if the proposal does not introduce any backwards incompatibilities, but this section must be included if backward incompatibilities exist.
- Reference Implementation *(optional)* - An optional section that contains a reference/example implementation that people can use to assist in understanding or implementing this specification. This section may be omitted for all DCIPs.
- Security Considerations - All DCIPs must contain a section that discusses the security implications/considerations relevant to the proposed change. Include information that might be important for security discussions, surfaces risks and can be used throughout the life-cycle of the proposal. E.g. include security-relevant design decisions, concerns, important discussions, implementation-specific guidance and pitfalls, an outline of threats and risks and how they are being addressed. DCIP submissions missing the "Security Considerations" section will be rejected. An DCIP cannot proceed to status "Final" without a Security Considerations discussion deemed sufficient by the reviewers.
- Copyright Waiver - All DCIPs must be in the public domain. The copyright waiver MUST link to the license file and use the following wording: `Copyright and related rights waived via [CC0](../LICENSE.md).`

## DCIP Formats and Templates

DCIPs should be written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) format. There is a [template]() to follow.

## DCIP Header Preamble

Each DCIP must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order.

`dcip`: *DCIP number* (this is determined by the DCIP editor)

`title`: *The DCIP title is a few words, not a complete sentence*

`description`: *Description is one full (short) sentence*

`author`: *The list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.*

`discussions-to`: *The url pointing to the official discussion thread*

`status`: *Draft, Ready, Under Review, Approved, Changes Required, Blacklisted, Merged.*

`last-call-deadline`: *The date last call period ends on* (Optional field, only needed when status is `Last Call`)

`type`: ToDo

`category`: ToDo

`created`: *Date the DCIP was created on*

`requires`: *DCIP number(s)* (Optional field)

`blacklisted-reason`: *A sentence explaining why the DCIP was blacklisted.* (Optional field, only needed when status is `Blacklisted`)

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

### `author` header

The `author` header lists the names, email addresses or usernames of the authors/owners of the DCIP. Those who prefer anonymity may use a username only, or a first name and a username. The format of the `author` header value must be:

> Random J. User &lt;address@dom.ain&gt;

or

> Random J. User (@username)

or

> Random J. User (@username) &lt;address@dom.ain&gt;

if the email address and/or DCF GIT username is included, and

> Random J. User

if neither the email address nor the DCF GIT username are given.

At least one author must use a DCF GIT username, in order to get notified on change requests and have the capability to approve or reject them.

### `discussions-to` header

While an DCIP is a draft, a `discussions-to` header will indicate the URL where the DCIP is being discussed.

The preferred discussion URL is a topic on the [DCF Forum](https://forum.decentralizedclimate.org/). The URL cannot point to DCF GIT pull requests, any URL which is ephemeral, and any URL which can get locked over time (i.e. Reddit topics).

### `type` header

The `type` header specifies the type of DCIP: ToDo.

### `category` header

The `category` header specifies the DCIP's category. ToDo.

### `created` header

The `created` header records the date that the DCIP was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

### `requires` header

DCIPs may have a `requires` header, indicating the DCIP numbers that this DCIP depends on. If such a dependency exists, this field is required.

A `requires` dependency is created when the current DCIP cannot be understood or implemented without a concept or technical element from another DCIP. Merely mentioning another DCIP does not necessarily create such a dependency.

## Linking to External Resources

Listed below, links to external resources **SHOULD NOT** be included. External resources may disappear, move, or change unexpectedly.

## Linking to other DCIPs

References to other DCIPs should follow the format `DCIP-N` where `N` is the DCIP number you are referring to.  Each DCIP that is referenced in an DCIP **MUST** be accompanied by a relative markdown link the first time it is referenced, and **MAY** be accompanied by a link on subsequent references.  The link **MUST** always be done via relative paths so that the links work in this DCF GIT repository, forks of this repository, the main DCIPs site, mirrors of the main DCIP site, etc.  For example, you would link to this DCIP as `./dcip-1.md`.

## Auxiliary Files

Images, diagrams and auxiliary files should be included in a subdirectory of the `assets` folder for that DCIP as follows: `assets/dcip-N` (where **N** is to be replaced with the DCIP number). When linking to an image in the DCIP, use relative links such as `../assets/dcip-1/image.png`.

## Transferring DCIP Ownership

It occasionally becomes necessary to transfer ownership of DCIPs to a new champion. In general, we'd like to retain the original author as a co-author of the transferred DCIP, but that's really up to the original author. A good reason to transfer ownership is because the original author no longer has the time or interest in updating it or following through with the DCIP process, or has fallen off the face of the 'net (i.e. is unreachable or isn't responding to email). A bad reason to transfer ownership is because you don't agree with the direction of the DCIP. We try to build consensus around an DCIP, but if that's not possible, you can always submit a competing DCIP.

If you are interested in assuming ownership of an DCIP, send a message asking to take over, addressed to both the original author and the DCIP editor. If the original author doesn't respond to the email in a timely manner, the DCIP editor will make a unilateral decision (it's not like such decisions can't be reversed :)).

## DCIP Editors

The current DCIP editors are

- David E. Perez Negron R. User (@p1r0)
- Omar Octavio Huerta Valdez. User &lt;ohuerta@decentralizedclimate.org&gt;
- Alfonso Nuñes Navarro. User &lt;anavrro@decentralizedclimate.org&gt;

## DCIP Editor Responsibilities

For each new DCIP that comes in, an editor does the following:

- Read the DCIP to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
- The title should accurately describe the content.
- Check the DCIP for language (spelling, grammar, sentence structure, etc.), markup (GitHub flavored Markdown), code style

If the DCIP isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the DCIP is ready for the repository, the DCIP editor will:

- Assign an DCIP number (generally the PR number, but the decision is with the editors)
- Merge the corresponding [pull request](https://git.decentralizedclimate.org/DecentralizedClimateFoundation/DCIPs/pulls)
- Send a message back to the DCIP author with the next step.

Many DCIPs are written and maintained by developers with write access to the Decentralized Climate Foundation codebase. The DCIP editors monitor DCIP changes, and correct any structure, grammar, spelling, or markup mistakes we see.

The editors don't pass judgment on DCIPs. We merely do the administrative & editorial part.

## Style Guide

### Titles

The `title` field in the preamble:

- Should not include the word "standard" or any variation thereof; and
- Should not include the DCIP's number.

### Descriptions

The `description` field in the preamble:

- Should not include the word "standard" or any variation thereof; and
- Should not include the DCIP's number.

### DCIP numbers

When referring to DCIPs it must be written in the hyphenated form `DCIP-X` where `X` is that DCIP's assigned number.

### RFC 2119 and RFC 8174

DCIPs are encouraged to follow [RFC 2119](https://www.ietf.org/rfc/rfc2119.html) and [RFC 8174](https://www.ietf.org/rfc/rfc8174.html) for terminology and to insert the following at the beginning of the Specification section:

> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 and RFC 8174.

## History

This document was derived heavily from [Ethereum EIP-01](https://eips.ethereum.org/EIPS/eip-1) wich also was based on [Bitcoin's BIP-0001](https://github.com/bitcoin/bips) written by Amir Taaki which in turn was derived from [Python's PEP-0001](https://peps.python.org/). In many places text was simply copied and modified. Although the PEP-0001 text was written by Barry Warsaw, Jeremy Hylton, and David Goodger, they are not responsible for its use in the Ethereum Improvement Process, and should not be bothered with technical questions specific to Ethereum or the EIP. Please direct all comments to the EIP editors.

## Copyright

Copyright and related rights via [GFDL](../LICENSE.md).


## References

\[1\] Martin Becze <mb@ethereum.org>, Hudson Jameson <hudson@ethereum.org>, et al., "EIP-1: EIP Purpose and Guidelines," Ethereum Improvement Proposals, no. 1, October 2015.


