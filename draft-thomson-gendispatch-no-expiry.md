---
title: "Removing Expiration Notices from Internet-Drafts"
abbrev: Drafts Aren't Milk
docname: draft-thomson-gendispatch-no-expiry-latest
date:
category: bcp
area: "General"
workgroup: "General Area Dispatch"
updates: 2026, 2418

submissiontype: IETF
number:
consensus: true
v: 3
keyword:
 - dead mans switch
venue:
  group: "General Area Dispatch"
  type: "Working Group"
  mail: "gendispatch@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/gendispatch/"
  github: "martinthomson/no-expiry"
  latest: "https://martinthomson.github.io/no-expiry/draft-thomson-gendispatch-no-expiry.html"

author:
  -
    ins: M. Thomson
    name: Martin Thomson
    org: Mozilla
    email: mt@lowentropy.net
  -
    ins: P. Hoffman
    name: Paul Hoffman
    org: ICANN
    email: paul.hoffman@icann.org

normative:
  IDCG:
    title: "Content guidelines overview"
    target: https://authors.ietf.org/en/content-guidelines-overview
    date: 2022-06-01

informative:

--- abstract

The long-standing policy of requiring that Internet-Drafts bear an expiration
date is no longer necessary.  This document removes requirements for expiration
for Internet-Drafts from RFC 2026/BCP 9 and RFC 2418/BCP 25.
In place of expiration, this document introduces Internet-Drafts being labeled
"active" and "inactive" in the IETF tooling.


--- middle

# Introduction

The Content Guidelines for Internet Drafts {{IDCG}} requires that
Internet-Drafts include an expiration statement.  Tooling and IETF practice
insist on Internet-Drafts including an expiry date 185 days after their posting.
After this expiration date, some systems might display an Internet-Draft
differently or not at all, with some exceptions, such as when the document is
under IESG review.

Some people believe that automatic expiration prevents the use of an Internet-Draft for reference
purposes, so that they do not become stable references in other work.
Some people believe that automatic expiration encourages authors to update drafts that they wish to
discuss.  Originally, expired drafts were deleted from IETF servers completely;
more recently, expiration only causes the document to be hidden from certain
views or searches.

Copies of expired drafts are retained and can be obtained using other services.
Expired drafts are routinely cited and referenced in various contexts,
such as in IANA registries, academic papers, and informational references in RFCs.
Thus, statements about it being inappropriate to cite drafts
can lead readers not familiar with IETF processes to misunderstand how old
drafts may be used in practice.

This document does the following:

- Updates {{!STD-PROCESS=RFC2026}} to eliminate the removal of an Internet-Draft
when the latest version is unchanged for more than six months.

- Updates {{!WG=RFC2418}} to eliminate the inclusion of an expiration date in
Internet-Drafts.

- Updates the Content Guidelines {{IDCG}} to remove references to expiration.

- Updates the boilerplate text for Internet-Drafts to no longer include the
"Expires:" field.

- Introduces a status for Internet-Drafts which can be set to either "active" or "inactive" in
tooling without specifying how this is implemented.


# No More Expiration and Automatic Removal

The day of posting for an Internet-Draft is the best -- or perhaps only -- date
that can be added to a document that might help readers understand whether the
content is valid in the future.  Future events might invalidate the content
virtually immediately; conversely, an Internet-Draft could remain relevant for
an arbitrarily long period of time.

## Changes to Existing RFCs and Guidelines

RFC 2026 {{!STD-PROCESS=RFC2026}} talks about removal of Internet-Drafts in
the second paragraph of Section <xref section="2.2" sectionFormat="bare"
target="STD-PROCESS"/>, which is amended as follows:

OLD:

{:quote}
> An Internet-Draft that is published as an RFC, or that has remained
> unchanged in the Internet-Drafts directory for more than six months
> without being recommended by the IESG for publication as an RFC, is
> simply removed from the Internet-Drafts directory.  At any time, an
> Internet-Draft may be replaced by a more recent version of the same
> specification, restarting the six-month timeout period.

NEW:

{:quote}
> At any time, an
> Internet-Draft may be replaced by a more recent version of the same
> specification.

RFC 2418 {{!WG=RFC2418}} talks about header information in Internet-Drafts in
Section <xref section="7.2" sectionFormat="bare" target="WG"/>.
The bullet point "- The expiration date for the I-D." from that section is removed.

The Content Guidelines {{IDCG}} refers to boilerplate that will be updated; see {{boilerplate}}.
Content Guidelines also says
"A statement specifying the expiry date of the Internet-Draft."
This statement and the description of how to specify the expiry date is removed.

## Removing the Expires field from Internet-Drafts {#boilerplate}

This document specifies that the "Expires:" field be removed from the header of
submitted Internet-Drafts, and that the boilerplate be amended as follows:

OLD:

> Internet-Drafts are draft documents valid for a maximum of six months and may
  be updated, replaced, or obsoleted by other documents at any time. It is
  inappropriate to use Internet-Drafts as reference material or to cite them
  other than as "work in progress."

NEW:

> Internet-Drafts are draft documents that may be updated, replaced, or
  obsoleted at any time. It is inappropriate to cite them other than as "work in
  progress."


# Active and Inactive Status for Internet-Drafts

The tooling maintained by the IETF (such as the Datatracker) can mark the latest
version of a draft as "active" or "inactive".
When a new version of a draft is published, it is immediately marked as "active",
and all earlier versions of that draft are marked as "inactive".

Other reasons that a draft might be marked "active" or "inactive" are open,
but will be informed by the communities that use Internet-Drafts.
Suggestions have already been made
for automatically marking drafts as "inactive" after a certain period of time,
for allowing working group chairs to control the marking for working group drafts,
for allowing documents targeting different streams (see {{Section 5 of ?RFC8729}}) to be subject to stream-specific policies,
and for authors being able to change the status of their draft,
either to mark a draft that has been overcome by events as "inactive"
or mark a draft as "active" when there is renewed interest.

## Replacement Procedures

Originally, the expiration of a draft was intended to ensure that the topic is disqualified
from consideration. Updating a draft before expiration was intended to
indicate continued interest from the authors.

Expiration was also used as a reminder to authors to update documents.
Without expiration, a substitute might be to provide a note in advance of
planned sessions.  For instance, for an upcoming session N+1, a reminder might
be issued for drafts that have not been updated in the interval between session
N and session N+1, but were updated between session N-1 and session N.
The "active" and "inactive" markings can also be used nudge authors to update
drafts before a meeting.

People might choose to concentrate their efforts on drafts that have been
recently updated.
With "active" and "inactive" markings, those people will have another indicator
for which documents might be of interest.


# Referencing Internet-Drafts

Documents referencing Internet-Drafts should always include the two-digit version number of the draft,
unless there is a reason to refer to the draft generically.
For instance, when producing an Internet-Draft it can be convenient to refer to another draft generically,
where document production tools ensure that the final artifact refers to the most recent version.

The IETF Datatracker service maintains a stable archive of most Internet-Drafts that is accessible by version.
Using IETF Datatracker URLs in references ensures the availability of the referenced document.


# Security and Privacy Considerations

This document has no direct implications on security or privacy.


# IANA Considerations

This document makes no request of IANA.


--- back
