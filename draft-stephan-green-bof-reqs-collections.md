---
title: "Green BoF requirements collections"
abbrev: "Green BoF requirements collections"
docname: draft-stephan-green-bof-reqs-collections

category: info
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
consensus: true
area: OPS
workgroup: WG Working Group
keyword: Sustainability, Ressources

venue:
  group: "Green BoF"
  type: "individual"
  mail: "green-bof@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/green-bof/"
  github: "emile22/sustainability"
  latest: "https://emile22.github.io/sustainability/draft-stephan-green-bof-reqs-collections-latest.html"

v: 3

author:
 -
   name: Emile Stephan
   organization: Orange
   country: France
   email: emile.stephan@gmail.com

 -
   name: Marisol Palmero
   organization: Cisco Systems
   email: mpalmero@cisco.com

normative:

informative:

  GREEN-BOF:
    title: "BOF proposal for GREEN WG Creation"
    date: 2024-05-10
    target: "https://github.com/marisolpalmero/GREEN-bof"

  rfc6988bis-green:
    title: "Requirements for Energy Efficiency Management, 11 years after the EMAN RFC6988"
    date: 2024-07-21
    target: "https://datatracker.ietf.org/doc/draft-eman-green-rfc6988bis"
    
  sustainability-insights:
    title: "Requirements for Energy Efficiency Management, 11 years after the EMAN RFC6988"
    date: 2024-07-21
    target: "https://datatracker.ietf.org/doc/draft-eman-green-rfc6988bis"

  legacy-path:
    title: "Requirements for Energy Efficiency Management"
    date: 2024-07-21
    target: "https://datatracker.ietf.org/doc/draft-stephan-legacy-path-eco-design"

  last-charter:
    title: "GREEN BOF framework"
    date: 2024-08-20
    target: "https://github.com/marisolpalmero/GREEN-bof/blob/main/Meetings/Meeting_0820_2024/GREEN%20BOF%20Charter%20Refining%20discussion-2024-8-20.pdf"

--- abstract

This memo extracts and groups requirements from the drafts which provided material to the green BoF. The aim is to determine initial sets of requirements actionable at different levels of the framework.

--- middle

# Introduction

This memo extracts and groups requirements from the drafts which provided material [GREEN-BOF], [sustainability-insights], [legacy-path] and [rfc6988bis-green] to the green BoF. The aim is to determine initial sets of requirements actionable at different levels of the framework [last-charter].

# Requirements extracted from [legacy-path]

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Inventory Management|component control capacity (aka component max on/off frequency supported)|Per component control| |
|Analysis|assess the gains of introducing eco-designed components in a device|Device Level Mgmt| |
|Control& Mgmt|comprehensive support of network-wide energy efficiency includes legacy devices|Network Level Mgmt| |

# Requirements from [rfc6988bis-green] draft Open Issues

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Control& Mgmt|Distinguish backup sources|rfc6988bis battery| |
|Inventory Management|Reporting on Other Entities, typically smart PDU or PoE|Fit in “Inventory of power components (of devices, racks, etc) including together”| |
|Observability or Interaction with Other domain|Room sensor (hvac…)|Data Center Case| |
|Observability|flexible (future-proof) description of the nature of the sources of the energy used |Standard metric| |

# Requirements extracted from [sustainability-insights] uses cases

|category|requirements|note|Priority|
|:----|:----|:----|:----|

# Security Considerations

TODO Security

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
