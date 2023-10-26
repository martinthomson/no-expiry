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


--- middle

# Introduction

The Content Guidelines for Internet Drafts {{IDCG}} requires that
Internet-Drafts include an expiration statement.  Tooling and IETF practice
insist on Internet-Drafts including an expiry date 185 days after their posting.
After this expiration date, some systems might display an Internet-Draft
differently or not at all, with some exceptions, such as when the document is
under IESG review.

Expiration is believed to prevent the use of an Internet-Draft for reference
purposes, so that they do not become stable references in other work.
Expiration also existed to encourage authors to update drafts that they wish to
discuss.  Originally, expired drafts were deleted from IETF servers completely;
more recently, expiration only caused the document to be hidden from certain
views or searches.

Copies of expired drafts are retained and can be obtained using other services.
Expired drafts are routinely cited and referenced.  Published RFCs routinely
include informative references to drafts, which then usually expire.
Many IANA registries refer to expired drafts.


# Removing Internet-Draft Expiration

Forced expiration serves no purpose that is not adequately served by the
publication date on the document.

The date of posting for an Internet-Draft is the best -- or perhaps only --
information available that can be added to a document the time of publication
that might help readers understand whether the content is valid.  Future events
might invalidate the content virtually immediately; conversely, an
Internet-Draft could also remain relevant for an arbitrarily long period of
time.

This document proposes that the "Expires:" field be removed from the header of
submitted Internet-Drafts, and that the boilerplate be amended as follows:

OLD:

> Internet-Drafts are draft documents valid for a maximum of six months and may
  be updated, replaced, or obsoleted at any time. It is inappropriate to use
  Internet-Drafts as reference material or to cite them other than as "work in
  progress."

NEW:

> Internet-Drafts are draft documents that may be updated, replaced, or
  obsoleted by other documents at any time. It is inappropriate to
  cite them other than as "work in
  progress."

Creating a revision to the Content Guidelines {{IDCG}} will be necessary to
remove references to expiration.

This document updates RFC 2026 {{!STD-PROCESS=RFC2026}} to remove the second
paragraph of Section <xref format="none" section="2.2" sectionFormat="bare"
target="STD-PROCESS"/> and RFC 2418 {{!WG=RFC2418}} to remove a single mention
of expiration from Section <xref format="none" section="7.2"
sectionFormat="bare" target="WG"/>.

Other than these specific changes, both RFC 2026 and RFC 2418 refer to
expiration of drafts.  With this change, this is understood to apply to drafts
that are marked as "dead" in tooling.


# Replacement Procedures

The expiration of a draft is intended to ensure that the topic is disqualified
from consideration and discussion.  At the same time, updating a draft
indicates continued interest from the authors.

People might choose to concentrate their efforts on drafts that have been
recently updated.  For instance, when setting an agenda for a session, chairs
might give precedence to documents that have been updated since the preceding
session.

Expiration has also been used as a reminder to authors to update documents.  A
substitute for expiration reminders might be to provide a note in advance of
planned sessions.  For instance, for an upcoming session N+1, a reminder might
be issued for drafts that have not been updated in the interval between session
N and session N+1, but were updated between session N-1 and session N.


# Security and Privacy Considerations

This document has no direct implications on security or privacy.


# IANA Considerations

This document makes no request of IANA.


--- back
