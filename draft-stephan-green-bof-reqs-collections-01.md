---
title: "Green BoF requirements collections"
abbrev: "Green BoF requirements collections"
docname: draft-stephan-green-bof-reqs-collections-01

category: info
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
consensus: true
area: "Operations and Management"
workgroup: "Getting Ready for Energy-Efficient Networking"
keyword: Sustainability, Ressources

venue:
  group: "Getting Ready for Energy-Efficient Networking"
  type: "Working Group"
  mail: "green-bof@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/green-bof/"
  github: "emile22/green-bof-req-collections"
  latest: "https://emile22.github.io/green-bof-req-collections/draft-stephan-green-bof-reqs-collections-01.html"

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
    title: "Sustainability Insights"
    date: 2024-05-07
    target: "https://datatracker.ietf.org/doc/html/draft-almprs-sustainability-insights"

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

Discussion Venues

The source of this draft and an issue tracker can be found at https://github.com/emile22/green-bof-req-collections 
   
--- middle

# Introduction

This memo extracts and groups requirements  from the drafts which provided material [GREEN-BOF], [sustainability-insights], [legacy-path] and [rfc6988bis-green] to the green BoF. The aim is to determine initial sets of requirements actionable at different levels of the framework [last-charter].

The tables below respect the format and the semantic of operators requirements table of [last-charter].

# Requirements extracted from [legacy-path]

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Inventory Management|component control capacity (aka component max on/off frequency supported)|Per component control| 1 (i)|
|Analysis|assess the gains of introducing eco-designed components in a device|Device Level Mgmt| 1 (ii)|
|Control& Mgmt|comprehensive support of network-wide energy efficiency includes legacy devices|Network Level Mgmt| 1 (iii)|

(i) Avoid control to break the component

(ii) the gain must be measurable

(iii) network-wide solution must include legacy devices and green-wg ready devices

# Requirements from [rfc6988bis-green] draft Open Issues

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Control& Mgmt|Distinguish backup sources|rfc6988bis battery| 2|
|Inventory Management|Reporting on Other Entities, typically smart PDU or PoE|Fit in "Inventory of power components (of devices, racks, etc) including together"| 2|
|Observability or Interaction with Other domain|Room sensor (hvac...)|Data Center Case| 4|
|Observability|flexible (future-proof) description of the nature of the sources of the energy used |Standard metric|2 |

# Requirements extracted from [sustainability-insights] uses cases

There are limited to energy consumption vs sustainability

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Observability|Provide near-real-time energy consumption to different device types, service types, and individual users | Helps identify which devices or network functions are consuming more energy. | 2 |
|Migration or Upgrade | Provide KPIs for energy efficiency parameters, enhance accuracy of upgrade decisions | Helps make informed decisions about upgrades based on actual usage data. |   |
|Recycling | Report on percentage of recycled user devices and components. Enable comprehensive reporting and recycling efforts | Major driver of the circular economy, transparency is key | 4 |
|Power Optimization | Provide KPIs for energy efficiency parameters. Perform actions to reduce energy consumption | Monitor network and application performance to optimize power usage | 4 |
|Control& Mgmt Switch off | Stop and restart WiFi APs with the right time, space, and service granularity | Save power consumption during periods when APs are not in use.| 2|


# Security Considerations

TODO Security

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.

