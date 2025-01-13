# TLS WG FAQs

This page holds answers to frequently asked questions in the TLS WG. Pull requests to maintain this page are highly encouraged.

## What's in scope for this WG?

The TLS working group concerns itself with the maintenance of the core TLS protocol. This includes the TLS and DTLS specification, plus any extensions that have wide applicability to TLS usage. 

## What's out of scope?

Anything not in the previous question, though there are a few things in particular:

1. Certificates or Certification Authorities: The [IETF LAMPS](https://datatracker.ietf.org/wg/lamps/documents/) WG does some maintenance on certificates. Concerns about the Web PKI should be taken to the [CA/Browser Forum](https://cabforum.org/).
2. Cryptographic primitives: The [IRTF Crypto Forum Research Group (CFRG)](https://irtf.org/cfrg) is one venue that you can discuss standardizing new primitives.
3. Application or domain-specific extensions to TLS: The working group usually only considers extensions to the protocol that are widely applicable. If your extension is specific to an application or deployment, the working group might not consider adopting the work. You are still encouraged to discuss such work, particularly if you are not sure. The working group has many people with considerable expertise in this area.

<a name="interest"></a>
## I have an idea for the TLS WG — what is the best way to see if others are interested in it?

There are several things you can do to gauge interest. First, it might help to look through the WG archives for related ideas. If the same proposal was brought to the group and rejected, understanding the rationale for said decision is an important piece of historical data to consider. Have circumstances changed since that decision such that the idea is now practical? 

If there are no obviously related drafts, the next step is to write up the idea in an Individual Draft and submit it; see [drafting](https://authors.ietf.org/en/choosing-a-format-and-tools), [content]([https://authors.ietf.org/en/content-guidelines-overview,) and [submitting](https://authors.ietf.org/submitting-your-internet-draft). Be sure to carefully motivate the problem in consideration and clearly describe the proposed solution. If applicable, also discuss the extent to which the proposal’s security properties have been studied or formally analyzed. It is common to submit new ideas without any sort of analysis. After submitting the draft to the datatracker, send an announcement to the mailing list about the Individual Draft. In this announcement, link to the Individual Draft’s datatracker page and summarize the purpose and who should be interested; this announcement should come well before asking for agenda time to allow the Working Group time to discuss it. It is better to have discussed the proposal on the list for at least one meeting cycle before requesting agenda time {{#agenda-requests}}. If you do attend an IETF meeting in person, you can discuss your Individual Draft with a smaller group and address any initial suggestions before engaging with the entire WG. In other words, submitting an initial version of the Internet Draft at the submission deadline, which is two weeks before the IETF face to face meetings, and expecting widespread support is unlikely to happen.

Just a reminder that the chairs run the Working Group call for adoption, i.e., the formal process for judging whether there is consensus to adopt an Individual Draft, but authors are free to send emails asking what the Working Group thinks of their Individual Draft.

## How do I interact with the TLS WG list?

The TLS list, tls@ietf.org, is governed by IETF’s Working Group Procedures [BCP25](https://datatracker.ietf.org/doc/bcp25/), which also includes Anti-Harassment Procedures, and by participating you agree to the Note Well [NW](https://www.ietf.org/about/note-well/) and to follow the Code of Conduct [CoC](https://datatracker.ietf.org/doc/bcp54/). Thank you for contributing as part of the TLS Working Group.

As moderators of this list, we are charged with determining when messages are “disruptive to the WG process”, phrase from [RFC 3934](https://datatracker.ietf.org/doc/rfc3934/), and, at a minimum, we consider the following to be disruptive:

* Unsolicited bulk e-mail (from [RFC 3683](https://datatracker.ietf.org/doc/rfc3683/))
* Discussion of subjects unrelated to IETF policy, meetings, activities, or technical concerns RFC 3683](https://datatracker.ietf.org/doc/rfc3683/)
* Unprofessional commentary, regardless of the general subject RFC 3683](https://datatracker.ietf.org/doc/rfc3683/)
* Repetition of arguments without providing substantive new information 
* Requesting an unreasonable amount of work to provide information

To elaborate on unprofessional commentary, we believe that this also includes uncivil commentary as defined by the IETF List Moderators that includes threats of violence, personal attacks, and derogatory language (see https://github.com/ietf/Moderators/blob/main/uncivil-commentary.md#descriptions).

RFC 3683 also includes “announcements of conferences, events, or activities that are not sponsored or endorsed by the Internet Society or the IETF”. Please contact the chairs if you wish to share these types of announcements, but in general we do not believe they are disruptive unless they are excessive and lack relevance.

Reminder that if at anytime you feel that if somebody is out of line you can say so on list or directly to us (mailto:tls-chairs@ietf.org), the ADs (mailto:sec-ads@ietf.org), or the Ombudsteam (mailto:ombudsteam@ietf.org); all IETF Participants are encouraged to talk with the Ombudsteam if they are uncomfortable or unsure about any behaviors.

## How do I register codepoints for TLS ciphersuites, extensions, etc.?

All registrations require an Expert Review; the panel of experts can be  reached at tls-reg-review@ietf.org. Some registrations are also Specification Required, which means a permanent readily-available document describing the document. Note that an Internet-Draft, even an expired one, is acceptable (although there is some discussion within the IETF about changing that). Also, the current panel of experts is inclined to require some form of documentation for all registrations.

 See [RFC8447](https://tools.ietf.org/html/rfc8447) for more details on this process.

The following list enumerates all items whose policy is Expert Review.

1. [TLS Application-Layer Protocol Negotiation (ALPN) Tokens](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#alpn-protocol-ids)
2. [TLS Heartbeat Message Types](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#heartbeat-message-types)
3. [TLS Heartbeat Modes](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#heartbeat-modes)

The following list enumerates all items whose policy is Specification Required.

1. [TLS Ciphersuites](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-4)
2. [TLS ClientCertificateTypes, in the range 64-223](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-2)
3. [TLS Supported Groups](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-8)
4. [TLS EC Point Formats](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-9)
5. [TLS EC Curve Types](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-10)
6. [TLS UserMappingType, in the range 64-223](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-14)
7. [TLS Signature Algorithm, in the range 64-223](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-16)
8. [TLS HashAlgorithm, in the range 64-223](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-18)
9. [TLS Exporter Labels](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#exporter-labels)
10. [TLS Authorization Data Format, in the range 64-223](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#authorization-data)
11. [TLS SignatureScheme](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-signaturescheme)
12. [TLS PskKeyExchangeMode](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-pskkeyexchangemode)
13. [TLS Extensions](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#tls-extensiontype-values-1)
14. [TLS Certificate Types](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#tls-extensiontype-values-3)
15. [TLS CachedInformationType, in the range 64-223](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#cachedinformationtype)

The following list enumerates all items whose policy is neither Expert Review nor Specification Required.

1. [TLS ClientCertificateTypes, in the range 0-63](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-2)
2. [TLS ContentType](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-5)
3. [TLS Alerts](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-6)
4. [TLS HandshakeType](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-7)
5. [TLS Supplemental Data Formats](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-12)
6. [TLS UserMappingType, in the range 0-63](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-14)
7. [TLS Signature Algorithm, in the range 0-63](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-16)
8. [TLS CachedInformationType, in the range 0-63](https://www.iana.org/assignments/tls-extensiontype-values/tls-extensiontype-values.xhtml#cachedinformationtype)
9. [TLS HashAlgorithm, in the range 0-63](https://www.iana.org/assignments/tls-parameters/tls-parameters.xhtml#tls-parameters-18)

## Should the WG adopt and work on my draft?

In short, the TLS WG aims to adopt work items that introduce core changes to the TLS protocol or extensions which have wide applicability and use. In practice, this means documents with intended Proposed Standard status or which seek recommended registry (Y) codepoints should aim for WG adoption. This is to ensure that any significant change to TLS receives adequate community review prior to publication.

RFC2026 (BCP 9) describes the differences between different document status levels, i.e., Proposed Standard, Experimental, or Informational. Briefly, Standards track documents expect significant community review prior to completion. In contrast, Informational documents encapsulate information for the community, without any form of consensus around the information, and Experimental documents aim to record some technology development efforts for the broader community. 

Documents which aim to seek non recommended codepoints (N) do not require WG adoption, and should follow the Specification Required process outlined above for codepoint registration. Documents which target Experimental status should only seek adoption if they introduce non-trivial changes to TLS. Likewise, documents which target Informational status should consult the TLS WG to see if there’s interest in the WG adopting the work for the purposes of broad review. Otherwise, said documents do not require adoption.

While the WG will be considerate of perspectives of different TLS user communities, there is the possibility that a proposal, even one that is in scope, is not adopted. There are a lot of reasons for this, but the most likely reason is lack of interest. Lack of interest can be attributed to many things, but two that spring to mind are:

* lack of bandwidth. The IETF is contribution driven, and sometimes the Working Group participants, who are essentially volunteering their time to review an Individual Draft, want to focus their limited time elsewhere.
* lack of support. The chairs need to judge whether there is sufficient interest to adopt an Individual Draft as a Working Group item, and that means there needs to be some number of participants willing to review,comment, and eventually implement. A lot of times, the reason for lack of support is a motivating use case; see [interest](#interest). A good practice is to attempt to evaluate the level of support yourself prior to asking for adoption.

In some cases, the community that is interested in the draft is in another Working Group along with the expertise about the problem the draft is trying to solve.  In these cases, it may be more appropriate to have the draft adopted in another Working Group with review from the TLS Working Group at various points in the document lifecycle. Along these lines, see [extensions](#extensions); the proposal describes usage of TLS, see [usage](#usage), and; the proposal defines a TLS profile; see [profile](#profile).

## Will my proposal require formal analysis before acceptance by the WG? 

In general, this depends on the draft in question. Formal analysis may be required by the group prior to any draft advancing to IESG (towards RFC publication). Some proposals may introduce sufficiently invasive changes that the WG deems formal analysis necessary prior to adoption in the group. Others may be uncontroversial and therefore require no formal analysis. If you are unsure about your proposal, please contact the TLS WG chairs (tls-chairs@ietf.org) for clarification.

<a name="extensions"></a>
## My proposal introduces a new TLS extension — is it relevant for the TLS WG, or does it require review by the TLS WG?

Many working groups propose new TLS extensions for use. See [RFC5764](https://tools.ietf.org/html/rfc5764) and [RFC8472](https://tools.ietf.org/html/rfc8472) as recent examples of such extensions. However, as per the new registration process outlined above, only TLS designated expert review is required for said extensions prior to allocation. 

Authors are encouraged to ask the TLS WG for review of their extension to ensure proper use.

<a name="usage"></a>
## My proposal describes usage of TLS — is it relevant for the TLS WG, or does it require review by the TLS WG?

No, it does not require review by the TLS WG. However, we encourage authors to seek best current practice guidance from the TLS WG. 

<a name="profile"></a>
## My proposal describes a profile for TLS — is it relevant for the TLS WG, or does it require review by the TLS WG?

No, it does not require review by the TLS WG. However, we encourage authors to seek best current practice guidance from the TLS WG. 

## Outside of the TLS WG, what are good working groups to consult if my proposal impacts TLS?

If your proposal introduces new cryptographic algorithms or mechanisms, or even uses existing mechanisms, consider reaching out to the [IRTF Crypto Forum Research Group (CFRG)](https://irtf.org/cfrg) for consultation.

If your proposal describes how to use TLS in a particular application, consider reaching out to the [Using TLS in Applications Working Group (UTA-WG)](https://datatracker.ietf.org/wg/uta) for consultation.

## Guidance for TLS WG Presenters

1. All slides must be sent to the TLS WG chairs (tls-chairs@ietf.org) or submitted to the [GitHub repository](https://github.com/tlswg/wg-materials) as a Pull Request in PDF format. PowerPoint and Keynote files will not be accepted.

2. With few exceptions, all non-WG presentations must have an accompanied [I-D submitted before the IETF draft deadline preceding the meeting](https://datatracker.ietf.org/submit/). This gives WG members ample time to review the document prior to the meeting as well as ensuring draft authors acknowledge the [Note Well](https://datatracker.ietf.org/submit/note-well/).

3. Presentation slides and any supporting materials for non-WG drafts must be sent to the TLS WG chairs (tls-chairs@ietf.org) at least 48 hours in advance. This gives the chairs an opportunity to review the presentation and post it for the WG to review before the meeting. (Chairs post the item at least 24 hours in advance of the meeting.) Failure to provide the slides in this time frame will result in your presentation being removed from the agenda. The presentation should not focus on explaining all technical details. Instead, aim for a high level overview and reserve details for those items that need additional  elucidation. For example, use of a particular cryptographic primitive within the context of TLS should be described without explaining the mathematical details of said primitive.

4. Every presentation should have a one-slide overview of the main points with links to additional reading resources. Presentations should be able to cover this slide in a few minutes. In cases where the WG runs short on time due to critical working group discussions, such slides provide enough information for interested readers to learn more.

5. Plan time for questions. This should typically be 25% or more of your allotted time, or 50% if you are planning on asking the working group questions such as, “is there interest in my draft?”
