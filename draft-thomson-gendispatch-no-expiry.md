---
title: "Internet-Drafts Don't Expire"
docname: draft-thomson-gendispatch-no-expiry-latest
date: {DATE}
category: bcp
area: General
workgroup: GENDISPATCH
updates: 2026, 2418

stand_alone: yes
pi: [toc, sortrefs, symrefs, docmapping]

author:
  -
    ins: M. Thomson
    name: Martin Thomson
    org: Mozilla
    email: mt@lowentropy.net

normative:
informative:

--- abstract

The long-standing insistence that Internet-Drafts carry expiration dates is a
concept that is no longer necessary.  This document removes requirements for
expiration for Internet-Drafts from RFC 2026/BCP 9 and RFC 2418/BCP 25.


--- middle

# Introduction

The [I-D Guidelines](https://www.ietf.org/standards/ids/guidelines/) declares
that Internet Drafts expire 185 days after their posting unless replaced or
under a range of special conditions, such as when the document is under IESG
review.

Expiration of drafts is believed to encourage authors to update drafts that they
wish to discuss.  Expired drafts are no longer served from the primary IETF
servers.

Copies of expired drafts are retained and can be obtained using other services.
Expired drafts are routinely cited and referenced.  Published RFCs routinely
include informative references to drafts, which then usually expire.

Forced expiration serves no purpose that is not adequately served by the
publication date on the document.


# Removing Internet-Draft Expiration

The date of posting for an Internet-Draft is sufficient information for readers
to understand validity.

This document proposes that the "Expires:" field be removed from the header of
submitted Internet-Drafts, and that the boilerplate be amended as follows:

OLD:

> Internet-Drafts are draft documents valid for a maximum of six months and may
  be updated, replaced, or obsoleted by other documents at any time. It is
  inappropriate to use Internet-Drafts as reference material or to cite them
  other than as "work in progress."

NEW:

> Internet-Drafts are draft documents that may be updated, replaced, or
  obsoleted by other documents at any time. It is inappropriate to use
  Internet-Drafts as reference material or to cite them other than as "work in
  progress."

Creating a revision to the I-D Guidelines will be necessary to remove references
to expiration.

This document updates RFC 2026 {{!STD=RFC2026}} to remove the second paragraph
of Section 2.2 and RFC 2418 {{!WG=RFC2418}} to remove a single mention of
expiration from Section 7.2.


# Security and Privacy Considerations

This document has no direct implications on security or privacy.


# IANA Considerations

This document makes no request of IANA.


--- back
