# Nix Governance Constitution (draft)

## Introduction

This document describes the highest level of governance structure for projects under the NixOS Foundation.

## Overview

There are two primary leadership bodies with a different scopes:
- The Steering Committee (SC), composed of 7 elected individuals to represent the community, is broadly responsible for technical and community decisions and delegation
- [The NixOS Foundation board](https://nixos.org/community/teams/foundation-board/), composed of the board members of the Stichting NixOS Foundation, a non-profit organisation in Utrecht, the Netherlands, is broadly responsible for legal, financial and partnership decisions and delegation

This constitution roughly comprises these parts:
- The detailed responsibilities of each body
- How SC decisions are made
- How the SC is elected

## Detailed Responsibilities

### Steering Committee

In order to guide the projects in accordance with Nix Community Values the Steering Committee shall have the following responsibilities, which it should delegate when appropriate.

- Manage which resources are considered official and manage the official resources
  - This involves both public communication resources and technical infrastructure
  - As of the time of establishment of SC, the [official resources](https://github.com/NixOS/org/blob/main/doc/resources.md) and access to them are listed in the repository
  - In particular, ensure existence and execution of processes for granting access to the projects and to the resources
- Manage the direction and processes of the projects when necessary
  - Ensure that project direction decisions and where the decisions came from are made explicit
    - Ensure timeliness of decisions as far as possible
    - Ensure that stalling on decisions is made explicit when unavoidable
      - When possible, recommend time or condition for followup
  - Ensure that the processes for making regular decisions exist and function
  - Ensure that escalation points exist and work
    - Final (until significant changes in the circumstances or available data and arguments) decision authority may be delegated, when significant analysis of the issue and the arguments is needed to build the competence to make a good decision. However, if the team receiving the authority does not reach internal consensus, the SC still has the responsibility to handle the delegation failure.
  - Evolve the constitution, including governance structure and governance processes, when appropriate, under supermajority requirements
- Create and manage teams in order to delegate authority on specific areas to them
  - Delegate authority over areas of interest to long-term teams and committees needing specific authority, and evolve their policy
  - Delegate analysis of arguments and the making of a consensus (inside the team) decision on specific contentious issues to short-lived teams
- In communication with the NixOS Foundation Board, set the policies and priorities for highly visible actions and events, and the resources under the care of the Foundation
  - Any delegation of this responsibility also delegates the communication with the Board on the delegated topics

### NixOS Foundation Board

The board is a partner with the SC in leadership and is primarily focused on corporate and general external relationships, fiscals/financials, legals and partnerships.

In particular, its responsibilities are to:
- Own and handle the administrative and legal
  - Serve as an interface between the community and the corporate/governmental/financial world
  - Manage trademarks
- Handle external relationships, partnerships and donations
  - Work with the SC to establish foundation policies that balance the interests of volunteers, commercial actors, and public institutions, while staying within legal and administrative feasibility constraints. This includes sponsorship and trademark policies.
  - Build and maintain beneficial and collaborative relationships
  - Maintain and support grants/grant providers
- Provide a framework for the community to self-organise:
  - Handle payments for tooling, meetups and infra
  - Manage credentials and permissions
- Own and be responsible for financials
  - Provide fiscal planning and funding for community events and efforts
  - Decide how much funding is available for each broadly scoped type of events and efforts, while the SC decides the priorities within these scopes and limits of the allocated funds

#### Board Composition Changes

Board changes are decided by a selection committee composed of some delegates from the current board and some delegates from the SC. To block any specific new or continuing appointment of a person, objections from a number of delegates equal to the size of the smaller delegation of the two (board or SC) suffice. For example, with 1 delegate from the board, and 3 delegates from the SC, one delegate from either can block an appointment.

This procedure can be invoked by the SC or the board at any point in time.

### Steering Committee Decision process

#### Extraordinary Decisions

The following decisions require at least a 2/3 supermajority agreement of the full SC size (vacant seats count as abstaining).

- Changing the constitution
- Forced removal of SC members

Furthermore, the SC decides on the Election Committee (EC) with a 2/3 supermajority. If the SC cannot come to supermajority agreement on the list of EC members, they will conduct an election using the same tallying system as the previous SC election, where only SC members can vote.

Disqualifications of candidates in an election requires unanimity among the currently serving non-running members.

Substantial amendments to the Nix Community Values require 90% agreement in a poll among eligible voters. Deciding that an amendment is not substantial can be done by unanimity among a full SC.

#### Ordinary decisions

Everything within the authority of SC that doesn't require an extraordinary decision can be decided with a simple majority (at least 50%) of a full SC (vacant seats count as abstaining).

An exception to that is when there is when the [conflict of interest balance](#conflict-of-interest-balance) condition is suspected to be violated, in which case all non-involved currently-serving SC members will have a simple majority decision over whether there is a violation.

### Composition and Appointment

The SC consists of 7 elected members.
Regular elections are once a year, with half (alternating rounding every year) of the seats up for election,
such that each member holds a seat for one term of at most 2 years before it is up for election again.
Members can at most serve two consecutive terms. There is no lifetime maximum.

The previous SC appoints an Election Committee (EC) of at least 3 people to administer the election. If the SC cannot come to supermajority agreement on the list of EC members, they will conduct an election using the same tallying system as the previous SC election, where only SC members can vote.
SC members can be EC members only if they're leaving after the election.

#### Vote eligibility

Before the election process is initiated, the EC selects a cutoff date.
Only contributions to official projects in the four years preceding the cutoff date are considered.

There are two automatic ways to become eligible for voting, either:
- Have authored enough merged PRs to the [NixOS GitHub organisation](https://github.com/nixos) to total at least 25 commits.
- Have merged any PR to the NixOS GitHub organisation.

The list of automatically eligible voters is made public.

People not automatically eligible then have some time to send a request to the EC, which can then make an exception and approve them as voters. This is for people whose official contributions are not visible in the NixOS GitHub organisation, such as:
- Official event organisers and speakers
- Maintainers of official third-party accounts (e.g. social media)
- etc.

After the decisions on exception requests are made, the list of approved requests is also made public.

Not eligible in any case are bot accounts and people that are banned at the time when the list of automatically eligible voters is published.

#### Candidates

The requirements to become a candidate for the SC elections are:
- To be eligible for voting
- Agree to be a candidate
- Provide a public position statement, why the candidate should be elected and what are the positions on the current issues.
- To be publicly endorsed by at least 3 other people eligible to vote
  - How endorsements are collected will be specified by the EC
  - Among the candidate and their endorsers, there must be at least 4 individuals where no two have the same conflict of interest (e.g. employees of the same company or otherwise the same payer for Nix work), as decided by the EC.
  - One can endorse a person who has not yet agreed to be a candidate, which also serves as nominating them (subject to acceptance of nomination)
  - Eligible voters may endorse multiple nominees
- To have been not a member of the SC for at least two complete years of the two immediately preceding terms
- To not be a member of the EC
- To not have any conflicts of interest that would [prevent one from being appointed](#conflict-of-interest-balance) to the SC, and publicly disclose all potential conflicts of interest
  - This includes conflicts of interest to arise during the term based on already finalised agreements

After the nomination deadline, the SC can prevent a nominee from becoming a candidate by unanimity (among the currently serving non-running members of the SC) in case their public image or conduct would not be compatible with the position in the SC.

#### Procedure

The election is done using a [proportional representation mode from Condorcet Internet Voting Service (CIVS)](http://web.archive.org/web/20240412235900/https://civs1.civs.us/proportional.html). The recommendation is to use [CIVS](https://civs1.civs.us/) itself, but if CIVS is unavailable, a reasonable alternative proportional representation election implementation is also permitted.

In any election where seats with different end-of-term dates are available, winning candidates with higher final election rankings are appointed to the longer terms.

#### Special considerations for the first SC election

- To stagger the terms, the first election will appoint half the members rounded up with 2-year terms and the remaining members with 1-year terms.
- The EC for the first election will be the members of the [Nix Constitutional Assembly (NCA)](https://github.com/nixos/nix-constitutional-assembly?tab=readme-ov-file#members), which are thus ineligible to be elected for the first SC
- And to help the first elected SC establish itself, members of the NCA are integrated into the SC as non-voting members for 6 months after the appointment.

#### Conflict of Interest (CoI) Balance

To encourage diversity there is a soft limit of one individual with the same CoI (e.g. employees of the same company or otherwise the same payer for Nix work) immediately after election results coming into force. If the results of an election would result in multiple individuals with the same CoI being elected, the lowest vote getters with any particular CoI will be removed until the condition is satisfied. In case of doubts (subsidiaries etc.) the election committee makes a decision. The candidates must disclose already-agreed-upon changes of affilation that are to happen during the term, and at the time of election these are taken into consideration as same-employer collisions.

Furthermore, there is a hard maximum of two employees with the same CoI at any time. If this condition is suspected to be violated because of job changes, acquisitions, or other events, all non-involved currently-serving SC members will have a simple majority decision over whether there is a violation. In case it is deemed a violation, sufficient members of the committee must resign until the max representation limit is achieved. If it is impossible to find sufficient members to resign, the entire company’s representation will be removed and a new special election is held.

#### Special Elections

In the event of a resignation or other loss of a steering committee member (including a [removal for conduct](#removal-for-conduct)), a special election for that position may be held if the SC deems it necessary, or SC does not have half of normal size. Otherwise the missing positions are assumed to be abstaining from all the SC votes. A committee member elected in a special election will serve out the remainder of the term for the person they are replacing, regardless of the length of that remainder.

#### Full Reelections

A simple majority within the SC may call a reelection of the entire SC based on perceived loss of confidence. In this case it also has to be decided whether this election is considered a special election for the remainders of all the corresponding terms, or an initial election for full 2-year terms for half of the seats rounded up, and 1-year half-terms for the remaining seats.

### Removal for conduct

A supermajority within the SC may remove SC members for violating the community expectations for members in positions of high authority. The reasons include but are not limited to unfitting conduct and unavailability, and a summary of the reason should be respectfully described. The SC is explicitly expected to be held to higher standards than applied to project communication in general.

The removal can be justification for a special election where the removed person is not eligible to be a candidate.
