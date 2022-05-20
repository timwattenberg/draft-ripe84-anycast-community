---
title: "ANYCAST Community"
#abbrev: "TODO - Abbreviation"
category: info

docname: draft-ripe84-anycast-community-latest
submissiontype: IETF  # also: "independent", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: "Internet"
workgroup: "Global Routing Operations"
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: "Global Routing Operations"
  type: "Working Group"
  mail: ""
  arch: ""
  github: "timwattenberg/draft-ripe84-anycast-community"
  latest: "https://timwattenberg.github.io/draft-ripe84-anycast-community/draft-ripe84-anycast-community.html"

author:
 -
    fullname: Tim Wattenberg
    organization: DE-CIX
    email: tim.wattenberg@de-cix.net
 -
    fullname: Your Name Here
    organization: Your Organization Here
    email: your.email@example.com

normative:

informative:


--- abstract

This document describes the use of a well-known Border Gateway Protocol (BGP) community for identifying anycast prefixes in IP networks. This well-known advisory transitive BGP community named "ANYCAST" allows an origin Autonomous System (AS) to signal a neighboring network that the tagged IP prefix is available via anycast and should be routed hot potato.


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# ANYCAST Community

This document defines the use of a new well-known BGP transitive community, ANYCAST.

The semantics of this community allow a network to interpret the presence of this community as an advisory qualification that this prefix is available via anycast and should be routed in a hot potato fashion.


# Vendor Implementation Recommendations

Vendors MAY provide a shorthand keyword in their configuration language to reference the well-known ANYCAST community attribute value. The suggested string to be used is "anycast".


# Security Considerations

TODO Security


# IANA Considerations

This document requires addition of a new entry to the "BGP Well-known Communities" registry. 
IANA should make include in the registry before publication:

```
ANYCAST (=0xFFFF????)
```


--- back

# Acknowledgments
{:numbered="false"}

The creation of this document was initiated by Fredy Künzler on RIPE84.
