---
layout: default
title: 2024 Annual Review Hyperledger AnonCreds
parent: 2024
grand_parent: Project Updates
---

# 2024 Annual Review Hyperledger AnonCreds

## Project Health

Hyperledger AnonCreds LFX Insights Page for [Calendar Year 2023](https://insights.lfx.linuxfoundation.org/foundation/hyp/overview?project=anoncreds&repository=all&dateFilters=2023-01-01%20to%202023-12-31&dateRange=2023-01-01%20to%202023-12-31&compare=PP&granularity=month&hideBots=true) (v. [2022](https://insights.lfx.linuxfoundation.org/foundation/hyp/overview?project=anoncreds&repository=all&dateFilters=2022-01-01%20to%202022-12-31&dateRange=2022-01-01%20to%202022-12-31&compare=PP&granularity=month&hideBots=true))  and for [Q1 2024 Oct-Dec.](https://insights.lfx.linuxfoundation.org/foundation/hyp/overview?project=anoncreds&repository=all&dateFilters=2023-10-01%20to%202023-12-31&dateRange=2023-10-01%20to%202023-12-31&compare=PP&granularity=month&hideBots=true) (v. [Q4 2023](https://insights.lfx.linuxfoundation.org/foundation/hyp/overview?project=anoncreds&repository=all&dateFilters=2023-07-01%20to%202023-09-30&dateRange=2023-07-01%20to%202023-09-30&compare=PP&granularity=month&hideBots=true)).

Compared to 2022, the Pull Request count was up by about 100% to 219 in 2023, while the number of contributors was up a little to 31. Compared to Q4 2023, the Q1 2024 report shows Pull Requests up about 30% (to 32) in Pull Requests, and Contributors up a couple (to 14). 2022 was the inaugural year of Hyperledger AnonCreds, and so the year-to-year comparison is not quite apples-to-apples.

AnonCreds has made great strides in the past year, surviving the archiving of the Ursa Project, which actually resulted in considerable improvement in the AnonCreds code shifted from Ursa, completing a significantly improved AnonCreds RS implementation aligned with the AnonCreds v1.0 specification, and a contribution of AnonCreds v2.0 code. However, there has been a lack of engagement in moving the AnonCreds v2.0 codebase forward, and that is a cause for concern.

## Maintainer Diversity

There are currently 11 maintainers in the project representing 8 organizations.

Typical AnonCreds [Maintainers File](https://github.com/hyperledger/anoncreds-rs/blob/main/MAINTAINERS.md).

## Project Adoption

Information on adoption is hard to find about AnonCreds and the projects that build on AnonCreds — Hyperledger Aries and Indy. Wherever you find Aries and Indy (which is a lot of places), you find AnonCreds.

Our sense is that adoption is steady, climbing (somewhat) along with the rest of the digital trust world. On the one hand, AnonCreds are well known to be the most privacy-preserving kind of verifiable credentials, through the use of easy to deploy ZKP-based technology that limits data sharing and tracking. On the other hand, AnonCreds are seen as differing from other VC standards and open specifications (notably the W3C VC data model) and OpenID4VCs and tied to Hyperledger Indy ledger deployments. We are working to eliminate those perceptions and enable the digital trust world to have both verifiability and maximum privacy.

We are concerned that more needs to be done to educate the broader digital trust community about the possibilities of AnonCreds v2, and the new capabilities it brings. AnonCreds is not a one-time, fixed implementation of CL Signatures, but a relatively easy abstraction layer on top of VCs to enable the use of ZKPs using different signatures. The v2 code base we have is a clear demonstration of that. Getting organizations to contribute to and use AnonCreds v2 seems to be a challenge.

## Goals

### Performance Against Prior Goals

As this is the first Hyperledger AnonCreds Annual Report, there is not a 2022 Annual Report to look back on. Instead, in this section we highlight some of the accomplishments in the project, in no particular order.

* Completion of the AnonCreds RS implementation of AnonCreds, aligned with the AnonCreds v1 specification.
* Transfer of the Ursa CL Signatures implementation to an AnonCreds repository, and the application of significant improvements to the code, including addressing identified vulnerabilities and improving performance.
* A very successful Hyperledger Mentorship to add the cryptography to the AnonCreds v1 specification.
* Completion (pending a final editorial pass) of the AnonCreds v1 specification.
* Support for AnonCreds verifiable credentials and verifiable presentations in W3C Verifiable Credentials Data Model Standard format, eliminating the longstanding complaint that AnonCreds VCs are “not compliant”.
* Contribution of the AnonCreds v2 codebase, with new ZKP capabilities and pluggable support for several cryptographic signature schemes, including PS Signatures (implemented), BBS+ Signatures, and PS Post Quantum Signatures.

### Next Year’s Goals

Recent AnonCreds Working Group meetings have covered defining a roadmap for 2024. The following is extracted from the discussions and notes from the meetings. The ordering is from activities well underway, to “reach for the clouds” ideas:

* Support for deploying AnonCreds in W3C format in Aries frameworks, and other AnonCreds implementations.
* Completion of the AnonCreds v1 specification and consideration of if and where to submit the specification for standardization.
* A draft of the AnonCreds v2 specification that outlines the adjustments made to the AnonCreds objects, signature schemes, and ZKP presentation capabilities available in using AnonCreds v2.
* Progress on the AnonCreds v2 “to do” list in transitioning it from the current complete, but not opinionated (and so, harder to deploy) to one that is the logical successor to AnonCreds v1. This includes:
    * W3C VC/VP Data Model support.
    * Abstraction of the signature scheme to meet the “pluggable” promise.
        * Experimentation with post quantum AnonCreds.
    * Support for the built-in “link secret” holder binding mechanism.
    * Support for both human- and ZKP-friendly date/date-time encodings.
* A documented path from AnonCreds v1 to v2.

### Help Required

There is a lot that the Hyperledger Foundation provides that we need to be making better use of, particularly in the area of marketing / getting the word out about the capabilities of Hyperledger Aries/AnonCreds. Our challenge is that the project is driven largely by technical types, not marketers.

Collaboration on AnonCreds as it transitions to v2 with new signature schemes, such as BBS+ (currently incubated at DIF and IETF) is a great opportunity to bring together a number of initiatives in the verifiable identity communities.

## Project Lifecycle Stage Recommendation

AnonCreds is an Incubation project and should probably remain so. AnonCreds is one of the most mature and battle-tested code bases in Hyperledger, has a solid specification, and (we think) broad adoption. However, we think that the acceptance and support for AnonCreds v2 is a driving factor in determining if privacy will win the day in digital trust, and that will dictate if AnonCreds should transition to a graduated project.

## TOC Hyperledger AnonCreds Annual Review Notes

[TOC Meeting Recording - 2024.02.15](https://zoom.us/rec/play/9R-g9dDkev58KyjPT7XkYJ6fltM879Tba6rdC-Loz_6pjyCjMabH5KwO8vcC-kvs_WoKp8ksD6Y8O1qG.FcT2qG1CM2RydRmp?canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2FSEWW2lMg14g4kV7hsjvXFr-i5hVtJDPlUb9_BmFb2S8cA-YyP-jw3EfEx4qbk4sA.AmQb1tXouL7kdu6A) -- AnonCreds Annual Review discussion starts at the 4:36 mark.

### Project Health

* Project reports great strides in the past year
* Project reports lack of engagement in moving the AnonCreds v2.0 codebase forward as concerning
* LFX Insights seems to have inaccurate information
    * showing contributors from other projects that do not have anything to do with AnonCreds or the identity space
    * the same committer is showing up under different names (swcurran vs. Stephen Curran, as well as others)
    * organization mapping does not line up with contributor mapping
* Based on LFX Insights, it appears that the project contributions have decreased over the last 6 months of 2023
* Based on LFX Insights, it appears that new contributors are not staying
* Based on LFX Insights, the PR average wait time for first review is ~5 days and the average lead time (time it takes for pull requests to be raised, reviewed, accepted and merged) of ~9 days

### Maintainer Diversity

* 11 maintainers in the project representing 8 organizations
* This is great diversity for a project
* From what LFX Insights provides, it does appear that there is a fairly even distribution of activity across maintainers

### Project Adoption

* Hard to find information on — would there be projects using it as a dependency
* Getting organizations to contribute to and use AnonCreds v2 seems to be a challenge because of inaccurate perceptions with it being viewed as different to other VC standards and specification

### Goals

* 2023 Goals were not set due to new project status. A number of accomplishments did occur in 2023, including completion of a v1 specification and its implementation
* 2024 Goals - good set focused on formalizing the v1 specification into a standard, work towards v2 with a migration path between v1 and v2, and support for deploying W3C format.
* It might be worth mentioning in the goals work what will be done for fixing the perception of AnonCreds

### Help Required

* Need help from marketing the capabilities of AnonCreds
* Collaborating with others in the verifiable identity community on v2 with new signature schemes

### Lifecycle

* Project recommends remaining in incubation
* Concur with this recommendation

### Project Suggestions

* Blog posts, webinars, meetups and conference talks for AnonCreds could help with perception issues, even if driven by technologists 
* Working with the other communities within the LF via presenting to those groups could also help with perception issues
* Consider doing a 1.0 release to reflect the true status of the software