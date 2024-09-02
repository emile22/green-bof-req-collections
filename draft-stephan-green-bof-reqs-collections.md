---
title: "Green BoF requirements collections"
abbrev: "Green BoF requirements collections"
docname: draft-stephan-green-bof-reqs-collections-latest

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
  latest: "https://emile22.github.io/green-bof-req-collections/draft-stephan-green-bof-reqs-collections.html"

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

  charter-refinement:
    title: "GREEN BOF Charter Refinement discussion"
    date: 2024-08-20
    target: "https://github.com/marisolpalmero/GREEN-bof/blob/main/Meetings/Meeting_0820_2024/GREEN%20BOF%20Charter%20Refining%20discussion-2024-8-20.pdf"

  operators-inputs:
    title: "Input from Operators to GREEN BoF"
    date: 2024-07-20
    target: "https://datatracker.ietf.org/meeting/120/materials/slides-120-green-input-from-operators-to-green-bof-01"

  network-inventory:
    title: "YANG Data Model for Network Inventory"
    date: 2024-07-20
    target: "https://datatracker.ietf.org/doc/draft-ietf-ivy-network-inventory-yang"

--- abstract

This memo extracts and groups requirements from the revisit of  operator's requirements made in the last charter refinement work and from the drafts which provided material to the green BoF. The aim is to determine initial sets of requirements actionable at different levels of the framework.

Discussion Venues

The source of this draft and an issue tracker can be found at https://github.com/emile22/green-bof-req-collections

--- middle

# Introduction

This memo extracts and groups requirements from the revisit of  operator's requirements made in the last charter refinement work [charter-refinement] and from the drafts which provided material [GREEN-BOF], [sustainability-insights], [legacy-path] and [rfc6988bis-green] to the green BoF. The aim is to determine initial sets of requirements actionable at different levels of the framework presented in [charter-refinement].

The tables below respect the format and the semantic of operators requirements table of [charter-refinement].

# Operator'requirements from [charter-refinement] document

The table below is a copy of the operator'requirements table of [charter-refinement]. They are based on the inputs received from operators for the GREEN BoF [operators-inputs].

|category|requirements|note|Priority|
|:----|:----|:----|:----|
|Observability|Component granularity, e.g., per line-card, per-port|Per component measurement|1|
|Observability|Availability of information on the power consumption of the device, without needing instrumentation connected to the infrastructure|Related to connected device case|1|
|Observability|Triggering of alarms when consumption deviate from a nominal usage|Alarm notification|1??|
|Observability|Improvement of metering solutions (finer granularity, control of the energy efficiency and saving, interoperability, exposure)|Standardized metering??|1|
|Analysis|Common definition of energy efficiency in network devices/components|Standard metric|1|
|Analysis|Common methodology of measurements for fair comparison|Standard methodology|2|
|Analysis|How to provide accurate figures (context of the measurement in terms of time period, location, traffic, etc|Time based, location based visualization|2 ??|
|Analysis|Database for decision in case of large data transfer|Information Correlation|3|
|Analysis|Ability of multi-layer analysis (e.g., IP plus optical)|POI Use Case|3|
|Control& Mgmt|To have devices with elastic power consumption according to the carried traffic|Dynamic Energy Saving|2|
|Control& Mgmt|Support of network-wide energy saving and optimization functions|Network Level Mgmt|2|
|Control& Mgmt|Support of network-wide control of energy optimization APIs, allowing external applications to optimize consumption|Network Level Mgmt|2|
|Control& Mgmt|Advanced sleep mode, needing some sort of low power mode when node is lightly utilized|Dynamic Energy Saving|2|
|Control& Mgmt|Ability to steer traffic based on power savings|Traffic Engineering|4|
|Control& Mgmt|Comparison of decision vs optimal case|Intent based Concept|2|
|Control& Mgmt|Synchronous query support|Network Level Query|2|
|Inventory Management|Inventory of power components (of devices, racks, etc) including together|Component & Device Level|1|
|Interaction with other domain|Inclusion of data center networks in the picture|Data Center Case|3|
|Interaction with other domain|Inclusion of data center networks in the picture|Mobile Network Case|3|
|Sustainability & Carbon Emission|Optimize the overall CO2 footprint (i.e., energy mix based on source type) facilitating the engineering of PoP More renewable energy|More renewable energy|4|
|Sustainability & Carbon Emission|Support GHG units|Measurement Units|4|
|Sustainability & Carbon Emission|Support Energy units|More renewable energy|2 ??|
|Sustainability & Carbon EmissiCarbon, renewable|4|
|Sustainability & Carbon Emission|Accounting of legacy installed based GHG/energy|Accounting Cost|4|
|Sustainability & Carbon Emission|Track device/network Energy Consumption Before Operation|Manufacturing, transport(weight, volume, package)|4|

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

# Framework Discussed During the BoF
The overall framework is shown in {{green-framework}}.

~~~~

        What needs to be standardized for Framework


 (3) Network Level :

 (a)              (b)              (c)
 Discovery        Monitor       +- DataSheets/DataBase and/or via API
 Or Inventory     Energy        ¦  Metadata and other device/component
 Of identity      Efficiency    ¦  /network related information:
 Inventory of         ^         ¦
 Capability           ¦         ¦  .Power/Energy related metrics
      ^               ¦         ¦  .information
      ¦               ¦         ¦  .origin of Energy Mix
      ¦               ¦         ¦  .carbon aware based on location
      ¦               ¦         ¦
      ¦               ¦         ¦
      ¦               ¦         ¦
      ¦               ¦         v
 +--------------------------------------------------------------------+
 ¦                   *                                                ¦
 ¦     (2) controller   (collection, compute and aggregate?)          ¦
 ¦                                                                    ¦
 +--------------------------------------------------------------------+
              ^              ^                   ^ ¦
  (d)         ¦  (e)         ¦  (f)              ¦ ¦(g)
  Discovery   ¦  IPPM WG:    ¦  GREEN WG:        ¦ ¦GREEN WG: Control
  Or Inventory¦  Monitor     ¦  Monitor power    ¦ ¦(Energy saving
  Of identity ¦  Network     ¦  Proportion,      ¦ ¦Functionality
  Inventory of¦  Performance ¦  Energy efficiency¦ ¦Localized mgmt/
  Capability  ¦  (Throughput,¦  ratio, Maximum   ¦ ¦network wide mgmt)
              ¦  Traffic load¦  sleep time, etc) ¦ ¦
              ¦  ,etc)       ¦                   ¦ ¦
              ¦              ¦                   ¦ v
 +--------------------------------------------------------------------+
 ¦                                                                    ¦
 ¦                  (1) Device/Component Level*                       ¦
 ¦                                                                    ¦
 ¦ +---------+  +-----------+  +----------------+  +----------------+ ¦
 ¦ ¦ (I)     ¦  ¦ (II)      ¦  ¦ (III)          ¦  ¦ (IV)           ¦ ¦
 ¦ ¦ Network ¦  ¦ Device    ¦  ¦ Legacy Network ¦  ¦ 'Attached'(PoE ¦ ¦
 ¦ ¦ Device  ¦  ¦ Component ¦  ¦ Device         ¦  ¦ kind) Device   ¦ ¦
 ¦ ¦         ¦  ¦           ¦  ¦                ¦  ¦                ¦ ¦
 ¦ +---------+  +-----------+  +----------------+  +----------------+ ¦
 +--------------------------------------------------------------------+

 (*) Energy Efficiency Management Function is implemented inside the
 device or in a controller

~~~~
{: #green-framework title="Framework discussed during the BoF"}

The main elements in the framework are as follows:

(a),(d) Inventory and Discovery

(b) Monitor Energy Efficiency

(c) DataSheets/DataBase information

(e) Network Performance

(f) Monitor Power

(g) control energy saving

## Inventory and Discovery

Based on the framework discussed during the BoF, the architectural requirements for the “GREEN” Framework:

From a Network Inventory {{network-inventory}} {{?I-D.draft-ivy-network-inventory-yang}} point of view, when discussing Energy Efficiency metrics, also known as GREEN metrics, it is important to distinguish between static and dynamic attributes:

“Static” attributes refer to those that do not change based on the state of the network infrastructure. The following examples are all static attributes that we can relate to the inventory, implemented in the network devices or as part of external sources:

- Serial number

- Product name

- Part number

- Vendor

- Device family

- Sensor(s)

Static attributes also include benchmarking information related to energy consumption by design and test conditions, normally associated to PSU’s, line-cards, etc.:

- Idle power

- Max power

- Typical power

- Accuracy rate

- PSU efficiency (80+)

- Power allocation

- Etc.

These attributes might be collected from the device/component itself or they might be parameters as part of external sources, i.e., databases owned by the hardware or software providers, where API access will be preferred.

Normally, the “Discovery” process will be updating static attributes that represent the up-to-date inventory of the network. The Discovery process relates primarily to the static attributes, where will consider if a device or component has been replaced or is out of service. The “Operation” process will be updating the so-called dynamic attributes.

Dynamic attributes are those that are subject to change due to the running operations, including configuration and state changes, and they will need to be collected regularly.

They will be updated as part of the regular operations. Dynamic attributes might be related to sensors(environmental), traffic, state, etc. They will include attributes like:

- Temperature

- Current

- Voltage

- Power

- Input and output traffic

The data collection frequency might need to be adjusted based on the specific attributes. For example, the discovery of linecards installed on network devices will not change every hour, whereas temperature and power sensor information changes will need to be closer to real-time.

Even though sensors normally are embedded in the network device/component, there are external sensors meant to measure temperature and energy consumption. The network controller will need to collect and correlate information to compose the right GREEN metric for the network device/component.

## Monitor Energy Efficiency

## DataSheets/DataBase information

## Network Performance

## Monitor Power

## Control Energy Saving

# TODO Security

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.

