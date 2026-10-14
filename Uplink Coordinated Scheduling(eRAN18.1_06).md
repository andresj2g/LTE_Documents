

eRAN
## Uplink Coordinated Scheduling
## Feature Parameter Description
## Issue06
## Date2023-12-22
## HUAWEI TECHNOLOGIES CO., LTD.



Copyright © Huawei Technologies Co., Ltd. 2024. All rights reserved.
No part of this document may be reproduced or transmitted in any form or by any means without prior
written consent of Huawei Technologies Co., Ltd.

Trademarks and Permissions
and other Huawei trademarks are trademarks of Huawei Technologies Co., Ltd.
All other trademarks and trade names mentioned in this document are the property of their respective
holders.

## Notice
The purchased products, services and features are stipulated by the contract made between Huawei and
the customer. All or part of the products, services and features described in this document may not be
within the purchase scope or the usage scope. Unless otherwise specified in the contract, all statements,
information, and recommendations in this document are provided "AS IS" without warranties, guarantees
or representations of any kind, either express or implied.
The information in this document is subject to change without notice. Every effort has been made in the
preparation of this document to ensure accuracy of the contents, but all statements, information, and
recommendations in this document do not constitute a warranty of any kind, express or implied.






## Huawei Technologies Co., Ltd.
Address:Huawei Industrial Base
## Bantian, Longgang
## Shenzhen 518129
People's Republic of China
## Website:https://www.huawei.com
## Email:support@huawei.com
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 06 (2023-12-22)..................................................................................................................................................1
1.2 eRAN18.1 05 (2023-09-14)..................................................................................................................................................1
1.3 eRAN18.1 04 (2023-04-23)..................................................................................................................................................2
1.4 eRAN18.1 03 (2023-02-01)..................................................................................................................................................2
1.5 eRAN18.1 02 (2022-06-27)..................................................................................................................................................2
1.6 eRAN18.1 01 (2022-03-08)..................................................................................................................................................3
1.7 eRAN18.1 Draft B (2022-02-08)........................................................................................................................................ 3
1.8 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 3
2 About This Document.............................................................................................................5
2.1 General Statements................................................................................................................................................................ 5
2.2 Applicable RAT......................................................................................................................................................................... 5
2.3 Features in This Document.................................................................................................................................................. 6
3 Overview....................................................................................................................................7
4 UL CRA (FDD)...........................................................................................................................8
4.1 Principles.................................................................................................................................................................................... 8
4.2 Network Analysis.................................................................................................................................................................. 10
4.2.1 Benefits................................................................................................................................................................................. 10
4.2.2 Impacts..................................................................................................................................................................................11
4.3 Requirements......................................................................................................................................................................... 13
4.3.1 Licenses................................................................................................................................................................................. 13
4.3.2 Software................................................................................................................................................................................14
4.3.3 Hardware..............................................................................................................................................................................16
4.3.4 Cells........................................................................................................................................................................................ 16
4.3.5 Others....................................................................................................................................................................................17
4.4 Operation and Maintenance.............................................................................................................................................17
4.4.1 Data Configuration........................................................................................................................................................... 17
4.4.1.1 Data Preparation............................................................................................................................................................ 17
4.4.1.2 Using MML Commands............................................................................................................................................... 18
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 19
4.4.2 Activation Verification......................................................................................................................................................19
4.4.3 Network Monitoring.........................................................................................................................................................19
eRAN
## Uplink Coordinated Scheduling Feature Parameter
DescriptionContents
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.iii

5 UL CPC (FDD).........................................................................................................................21
5.1 Principles.................................................................................................................................................................................. 21
5.2 Network Analysis.................................................................................................................................................................. 24
5.2.1 Benefits................................................................................................................................................................................. 24
5.2.2 Impacts..................................................................................................................................................................................25
5.3 Requirements......................................................................................................................................................................... 27
5.3.1 Licenses................................................................................................................................................................................. 27
5.3.2 Software................................................................................................................................................................................28
5.3.3 Hardware..............................................................................................................................................................................29
5.3.4 Cells........................................................................................................................................................................................ 30
5.3.5 Others....................................................................................................................................................................................30
5.4 Operation and Maintenance.............................................................................................................................................31
5.4.1 Data Configuration........................................................................................................................................................... 31
5.4.1.1 Data Preparation............................................................................................................................................................ 31
5.4.1.2 Using MML Commands............................................................................................................................................... 32
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 32
5.4.2 Activation Verification......................................................................................................................................................33
5.4.3 Network Monitoring.........................................................................................................................................................33
6 Parameters..............................................................................................................................34
7 Counters.................................................................................................................................. 35
8 Glossary................................................................................................................................... 36
9 Reference Documents...........................................................................................................37
eRAN
## Uplink Coordinated Scheduling Feature Parameter
DescriptionContents
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 06 (2023-12-22)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.2 eRAN18.1 05 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Deleted the mutually exclusive relationship between UL CRA and GSM and LTE
FDD Dynamic Spectrum Sharing (LTE FDD) from 4.3.2 Software.
Revised descriptions in this document.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description1 Change History
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.1

1.3 eRAN18.1 04 (2023-04-23)
This issue includes the following changes.
## Technical Changes
Change DescriptionParameter ChangeRATBase Station
## Model
Added a mutually
exclusive relationship
between UL CRA and
uplink single-side in-band
interference management.
For details, see 4.3.2
## Software.
NoneFDD3900 and 5900
series base
stations (macro
base stations)
Added a mutually
exclusive relationship
between UL CPC and
uplink single-side in-band
interference management.
For details, see 5.3.2
## Software.
NoneFDD3900 and 5900
series base
stations (macro
base stations)

## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 03 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 02 (2022-06-27)
This issue includes the following changes.
## Technical Changes
## None
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description1 Change History
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.2

## Editorial Changes
Revised descriptions in this document.
Added the impact relationship between UL CRA and intelligent PIM interference
avoidance. For details, see 4.2.2 Impacts.
1.6 eRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.7 eRAN18.1 Draft B (2022-02-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
Changed the function name "uplink coverage boost" to "uplink full-antenna
reception". For details, see 4.3.2 Software.
1.8 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 05 (2021-11-27).
## Technical Changes
## Change Description
Parameter ChangeRATBase Station
## Model
Added the mutually
exclusive relationship
between UL CRA and
uplink full-antenna
reception. For details, see
## 4.3.2 Software.
NoneFDD● 3900 and 5900
series base
stations
(macro base
stations)
## ● DBS3900
LampSite and
## DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E

eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description1 Change History
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.3

## Editorial Changes
Revised descriptions in this document.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description1 Change History
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.4

## 2 About This Document
## 2.1 General Statements
## Purpose
This document is intended to acquaint readers with:
●  The technical principles of features and their related parameters
●  The scenarios where these features are used, the benefits they provide, and
the impact they have on networks and functions
●  Requirements of the operating environment that must be met before feature
activation
●  Parameter configuration required for feature activation, verification of feature
activation, and monitoring of feature performance
## NO TE
This document only provides guidance for feature activation. Feature deployment and
feature gains depend on the specifics of the network scenario where the feature is
deployed. To achieve optimal gains, contact Huawei professional service engineers.
Functions mentioned in this document work properly only when enabled in the
specified applicable scenarios (such as RAT and networking). If a function not
mentioned in this document is enabled or a function is enabled in a scenario not
specified as applicable, exceptions or other impacts may occur.
## Software Interfaces
Any parameters, alarms, counters, or managed objects (MOs) described in this
document apply only to the corresponding software release. For future software
releases, refer to the corresponding updated product documentation.
2.2 Applicable RAT
This document applies to FDD.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description2 About This Document
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.5

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LOFD-081206Uplink Coordinated
## Scheduling
## 4 UL CRA (FDD)
## 5 UL CPC (FDD)
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description2 About This Document
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.6

## 3 Overview
The uplink performance of LTE networks is determined by legacy algorithms such
as uplink scheduling and uplink power control. These algorithms operate
separately for different E-UTRAN cells and inter-cell impact is seldom considered.
However, inter-cell interference is a crucial issue affecting the overall performance
of intra-frequency LTE networks. The Uplink Coordinated Scheduling feature
introduces the following functions, which take the inter-cell interference into
consideration. They improve the way information is shared between cells and
enable the cells to cooperate with each other, promoting the overall uplink
performance of LTE networks. The shared information includes the interference on
each RB and uplink scheduling resources allocated for each UE.
## RAT
## Function
## Name
## Function Overview
FDDUplink
coordinated
resource
allocation (UL
## CRA)
UL CRA adjusts resource allocation for UEs in the
serving cell based on the exchange of interference and
load information between the serving cell and its
cooperating cells. This reduces the amount of
interference generated by high-interference UEs on
neighboring cells in interference-limited scenarios.
FDDUplink
coordinated
power control
## (UL CPC)
UL CPC determines how the power spectral density
(PSD) needs to be adjusted based on UE scheduling
information and interference on cooperating cells. This
decreases interference on networks with medium-to-
heavy load and improves the average user-perceived
throughput.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description3 Overview
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.7

## 4 UL CRA (FDD)
## 4.1 Principles
To use UL CRA for it to yield expected gains, the operator must first turn on the
UL CRA switch for all intra-frequency same-bandwidth cells in a planned area. This
minimizes the number of border cells. There are two terms of special relevance to
UL CRA as follows:
●  Border cell
A border cell is a cell with an excessively high proportion of neighboring cells
where UL CRA is not in effect in a UL CRA cluster.
●  UL CRA cluster
A UL CRA cluster of a cell is the set of all the neighboring cells cooperating
for UL CRA.
When the UL_COORD_RES_ALLOC_SWITCH option of the UlCsAlgoPara.
UlCsSw
parameter is selected, UL CRA is enabled, and the UL CRA procedure is performed,
as shown in Figure 4-1.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.8

Figure 4-1 UL CRA procedure
-  The eNodeB determines which cells will be in the UL CRA cluster of the local
cell.
The eNodeB selects cells that meet all of the following conditions:
–   The UL CRA switch is on.
–   The cells operate on the same frequency and have the same bandwidth
as the local cell.
–   The cells are not high-speed cells (cells configured for UEs moving at
high speed).
–   The cells are deployed on non-LBBPc baseband processing units (BBPs).
–   The cells are served by the same type of base stations as the local cell.
For example, if both the local cell and neighboring cells are served by
macro base stations, they are of the same type.
–   The cells are included in event A3 reports generated for UL CRA by UEs of
the local cell.
Except for the UlCsAlgoPara.
UlCsA3Offset parameter, event A3 for UL
CRA uses the same A3 parameters as those of event A3 for UL CoMP.
The eNodeB arranges the cells in descending order based on the differences
between their RSRP values and that of the local cell and selects cells to
generate the UL CRA cluster.
-  The eNodeB determines whether the CPU usage of its main control board has
reached the flow control threshold.
–   If it has, the eNodeB disables UL CRA and uses the basic scheduling
policy to allocate resources. For details about resource allocation
principles, see
## Scheduling.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.9

–   If it has not, the eNodeB proceeds with 3.
-  The eNodeB obtains the average load information of the local cell and
neighboring cells from the information exchanged in the UL CRA cluster. The
eNodeB compares the average cell load with the threshold configured using
UlCsAlgoPara.
UlCoResAllocRbLoadThld parameter.
–   If the load is less than or equal to the parameter value, the eNodeB
preferentially allocates resources within the service-protecting bands to
UEs. This reduces the probability of reallocating the same physical
resource block (PRB) resources for neighboring cells.
–   If the load is greater than the parameter value, the eNodeB allocates
resources within the service-protecting bands to interference-sensitive
UEs in the local cell to avoid resource allocation conflicts with the
corresponding high-interference UEs in neighboring cells. Interference-
sensitive UEs have low signal to interference plus noise ratio (SINR)
values and limited power. It is recommended that this policy be used in
high-load cells with more than 100 uplink-synchronized UEs.
Service-protecting bands are a part of the band where PUSCH PRB resources
are reserved for high-interference UEs and interference-sensitive UEs. The
positions of service-protecting bands are specified by the
UlCsAlgoPara.
UlCoResAllocBandMode parameter.
UL CRA generally does not take effect even if the
UL_COORD_RES_ALLOC_SWITCH option of the UlCsAlgoPara.UlCsSw parameter
is selected in RAN sharing with common carrier or hybrid RAN sharing modes. The
two modes are enabled by setting the
ENodeBSharingMode.
ENodeBSharingMode parameter to SHARED_FREQ or
HYBRID_SHARED, respectively. When the following conditions are met, however,
UL CRA can take effect:
●  The UlCsAlgoPara.
UlCraSupportMocnSwitch parameter is set to ON.
●  The CellAlgoSwitch.RanShareModeSwitch parameter is set to OFF and the
LicRatio.
TrafficSharingType parameter is set to SHARING.
## 4.2 Network Analysis
## 4.2.1 Benefits
UL CRA mitigates the impact of high-interference UEs on neighboring cells. It
increases the average uplink UE throughput by up to 5% and the average uplink
throughput of cell edge UEs by up to 30% when the following conditions are met:
The average uplink interference (L.UL.Interference.Avg) in the deployment area is
more than –110 dBm. The PUSCH resource block (RB) usage is more than 10%.
The average number of uplink synchronized UEs in a cell is less than 200.
The following are the main factors affecting UL CRA performance:
●  Number of uplink-synchronized UEs
Fewer uplink-synchronized UEs result in a lower load, less interference, and
lower gains.
●  Inter-site distance
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.10

A larger distance results in less interference and lower gains. In general, the
average inter-site distance tends to be less than 500 m.
●  Amount of uncontrollable interference
If there is strong uncontrollable interference, better resource allocation will be
unable to eliminate interference, so UL CRA will not yield gains in such
scenarios. Generally, the uncontrollable interference should be less than –115
dBm. Uncontrollable interference includes:
–   Inter-RAT interference
–   Interference generated by repeaters
–   Interference from cells where UL CRA is not in effect
–   Intermodulation interference
–   Intra-RAT adjacent-channel interference such as that caused by a Double
Deck cell group described in
Flexible Bandwidth based on Overlap
## Carriers Feature Parameter Description
●  Physical cell identifier (PCI)
When the UlCsAlgoPara.UlCoResAllocBandMode parameter is set to
INVALID, the eNodeB adaptively selects a service-protecting band mode to
determine the positions of service-protecting bands. When this setting is used,
UL CRA is less likely to be effective and UL CRA gains will be lower if the PCI
modulo 3 results of the local cell and its neighboring cells are more likely to
conflict.
## 4.2.2 Impacts
## Network Impacts
●  When the average uplink interference (L.UL.Interference.Avg) in the
deployment area is greater than –110 dBm, the average uplink MCS index is
greater than 15, and the uplink residual block error rate (RBLER) is relatively
high, the gains in the throughput calculated as follows may be negative:
(L.Thrp.bits.UL – L.Thrp.bits.UE.UL.LastTTI)/L.Thrp.Time.UE.UL.RmvLastTTI.
●  UL CRA relies on A3 reporting, and therefore there are the following
additional impacts:
–   New A3 reports increase the signaling processing overhead. The value of
L.Signal.Num.Uu will go up and the CPU usage of the main control
board will increase by within 5%.
–   User-plane resources will be preempted for A3 reporting. If the uplink and
downlink RBs and control channel elements (CCEs) are insufficient, the
Cell Downlink Average Throughput value will drop by within 5% and
the downlink packet delay will increase by within 5%.
Therefore, UL CRA is not recommended under any of the following conditions:
–   The downlink RB usage is over 90%.
–   The uplink RB usage is over 90%.
–   The CCE usage is more than 80%.
–   The CPU usage is more than 80%.
●  In relaxed backhaul scenarios, when UL CRA and other features involving the
coordination of multiple eNodeBs (such as UL CoMP and CA) are enabled
together, they share transmission bandwidths. If the transmission bandwidths
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.11

are insufficient, the delays increase and the gains of these features are
affected.
## Function Impacts
## Function
## Name
Function SwitchReferenceDescription
UL CoMP cellUlJointReceptionS-
witch,
UlJointReception-
PhaseIISwitch, and
UlHetnetJointRecep-
tionSwitch options of
the
CellAlgoSwitch.
## Uplin
kCompSwitch
parameter
UL CoMPUL CRA reduces inter-
cell interference by
adjusting resource
allocation based on
information
exchanged between
the cells. UL CoMP
further reduces UE-
level interference. The
total gains obtained
by using both features
are greater than when
only UL CRA or UL
CoMP is enabled, but
less than the sum of
the gains separately
obtained.
UL CoMP
based on
eNodeB
coordination
UlJointReceptionO-
verBBUsSwitch
option of the
ENodeBAlgoSwitch.O
verBBUsSwitch
parameter
UL CoMP
Inter-eNodeB
VoLTE CoMP
UlVoiceJROverRelax-
edBHSw option of the
ENodeBAlgoSwitch.O
verBBUsSwitch
parameter
VoLTE
Uplink CACaUl2CCSwitch
option of the
CaMgtCfg.CellCaAlgo
Switch parameter
## Carrier
## Aggregation
Heavy load or
interference limitation
seldom occurs in
secondary cells
(SCells) when uplink
carrier aggregation
(CA) is enabled.
Therefore, UL CRA is
currently not used for
SCells.
PAMCUlPAMCSwitch
option of the
CellAlgoSwitch.UlSch
ExtSwitch parameter
SchedulingIf UL CRA and the
PAMC function are
both enabled, the
number of
interference-sensitive
UEs will decrease,
reducing UL CRA
gains.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.12

## Function
## Name
Function SwitchReferenceDescription
## Manual
blocking of
PUSCH RBs
CellRbReserve.RbRsv
## Mode
SchedulingUL CRA does not take
effect when the
CellRbReserve.RbRsv
Mode parameter is
set to either
RB_MASKING or
## RB_MASKING_WITH_
## SRS.
## Flexible
bandwidth
based on
overlapping
carriers
NoneFlexible
## Bandwidth
based on
## Overlap
## Carriers
## (FDD)
UL CRA does not take
effect when PUSCH
resources are not
contiguous or the
available system
bandwidth is less than
5 MHz.
## Compact
bandwidth
NoneCompact
## Bandwidth
## (FDD)
## Superior
uplink
coverage
CellAlgoExtSwitch.Ul
CoverageEnhance-
mentSw
## Superior
## Uplink
## Coverage
## (FDD)
UEs under enhanced
coverage do not
support UL CRA or
use resources in
service-protecting
bands when UL CRA
takes effect.
## Intelligent
## PIM
interference
avoidance
## PIM_INTERF_SMART_
AVOID_SW option of
the PimInterfSmartA-
void.PimAlgoSwitch
parameter
## Interference
Detection and
## Suppression
When intelligent PIM
interference avoidance
and UL CRA are both
enabled, the resource
allocation direction in
uplink scheduling
depends on intelligent
PIM interference
avoidance.

## 4.3 Requirements
## 4.3.1 Licenses
Feature ID
Feature NameModelSales Unit
LOFD-081206Uplink Coordinated
## Scheduling
## LT1SICUAMC0
## 0
## Per Cell

eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.13

## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## Function
## Name
Function SwitchReferenceDescription
## Frequency
hopping
CellUlschAlgo.UlHop
pingType
NoneNone
In-band relayInBandRelayDeNbS-
witch and
InBandRelayReNbS-
witch options of the
CellAlgoSwitch.Relay
## Switch
parameter
RelayNone
High speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
The functions cannot
work with UL CRA.
This is because UL
CRA does not deliver
gains in high-speed
cells due to their
high-speed moving
UEs.
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
Cell radius
greater than
15 km
NoneExtended Cell
## Range
The functions cannot
work with UL CRA.
This is because UL
CRA does not deliver
gains in cells with a
radius exceeding 15
km due to their low
traffic volume and
limited coverage.
Cell radius
greater than
100 km
NoneExtended Cell
## Range
CDMA and
LTE Zero
## Bufferzone
## (LTE FDD)
AvoidCDMAInterfS-
witch option of the
CellAlgoSwitch.Avoid
InterfSwitch
parameter
CDMA and
LTE Zero
## Bufferzone
## None
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.14

## Function
## Name
Function SwitchReferenceDescription
## Flexible
## PUCCH
configuration
PucchFlexCfgSwitch
option of the
CellAlgoSwitch.Pucch
AlgoSwitch
parameter
## Physical
## Channel
## Resource
## Management
The functions cannot
work with UL CRA
because they affect
the positions of
allocated resources
and will cause UL CRA
performance to
deteriorate.
## PUSCH RB
reservation
for voice
service UEs
UlVoipRbRsvSwitch
option of the
CellAlgoSwitch.UlSch
ExtSwitch parameter
VoLTE
LTE FDD and
NR Uplink
## Spectrum
## Sharing
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_UPLINK_SPE
## CTRUM_SHR
LTE FDD and
NR Uplink
## Spectrum
## Sharing
## None
Hybrid DSS
Based on
## Asymmetric
## Bandwidth
## LNR_SPECTRUM_SHR
_ASYM_SW option of
the
SpectrumCloud.Spect
rumCloudEnhSwitch
parameter with
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_SPECTRUM_S
## HR
LTE FDD and
NR Spectrum
## Sharing
## None
LTE FDD and
NR Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_SPECTRUM_S
## HR
LTE FDD and
NR Spectrum
## Sharing
## None
Short TTISHORT_TTI_SW
option of the
CellShortTtiAlgo.Stti
AlgoSwitch
parameter
Short TTI
## (FDD)
## None
Uplink full-
antenna
reception
## UL_COVERAGE_BOOS
T_SW option of the
SectorSplitGroup.Sec
torSplitSwitch
parameter
## Massive
## MIMO (FDD)
When uplink joint
scheduling is enabled,
uplink coordinated
resource allocation
(UL CRA) cannot be
enabled
Uplink single-
side in-band
interference
management
UlInterfSuppressCfg.
UlSingleSideIntr-
fImpMitSw
## Interference
Detection and
## Suppression
## None
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.15


## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
For FDD, the following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  BTS3912E
## ●  BTS3911E
## Boards
Non-LBBPc BBPs
RF Modules
No requirements
## 4.3.4 Cells
●  The cell bandwidth is greater than or equal to 5 MHz.
●  The RX mode of the antenna is 1R, 2R, or 4R.
●  eNodeBs providing the cells in a cluster are all macro eNodeBs, micro
eNodeBs, or LampSite eNodeBs.
●  An X2 interface that supports coordination-based services in non-ideal
backhaul scenarios, or an eX2 interface, is available.
The one-way delay for the interface must be less than 50 ms. For details
about X2 interface support for coordination-based services in non-ideal
backhaul scenarios, see
S1 and X2 Self-Management.
In addition, IP Performance Monitor (PM) sessions of forward activation type
are recommended for delay detection.
Configuring an IP PM session of bidirectional activation at either end of an
eX2 interface needs to be avoided. This is because eNodeBs automatically
create IP PM sessions to detect eX2 link status. An IP PM session of
bidirectional activation type may conflict with an automatically created
session. If this is the case, the eX2 interface will fail to work properly.
●  There are no PCI conflicts.
PCI conflicts can occur when two involved cells have the same PCI. If there is
a PCI conflict, the eNodeB may incorrectly select a cell in the UL CRA cluster
because it cannot differentiate between the two cells based on the
measurement reports from the UE. You are advised to set the
ENodeBAlgoSwitch.
PciConflictAlmSwitch parameter to ON so that PCI
conflicts can be reported.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.16

●  There is no intermodulation interference.
If there is intermodulation interference, the eNodeB cannot eliminate the
interference or prevent its impact by using resource coordination.
## 4.3.5 Others
No requirements
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Table 4-1 and Table 4-2 describe the parameters used for function activation and
optimization.
Table 4-1 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
UL CS SwitchUlCsAlgoPara.UlCsSwUL_COORD_R
## ES_ALLOC_S
## WITCH
Select this option.

Table 4-2 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
## UL CS A3
## Offset
UlCsAlgoPara.UlCsA3
## Offset
Set this parameter to the
recommended value.
## UL
## Coordinated
## Resource
## Allocation
## Band Mode
UlCsAlgoPara.UlCoRe
sAllocBandMode
The value INVALID is recommended.
If this parameter is not set to
INVALID, set this parameter differently
for the local cell and its neighboring
cells.
## UL
## Coordinated
## Resource
Allocation RB
## Load Thld
UlCsAlgoPara.UlCoRe
sAllocRbLoadThld
Set this parameter to the
recommended value.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.17

## Parameter
## Name
Parameter IDSetting Notes
## UL
## Coordinated
## Resource
Alloc IN
## Threshold
UlCsAlgoPara.UlCraIn
## Thld
Set this parameter to the
recommended value.
UL CRA User
## Number
## Threshold
UlCsAlgoPara.UlCraU
serNumThld
Set this parameter to the
recommended value.

4.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
Before using MML commands, refer to 4.2.2 Impacts and 4.3.2 Software and
complete the parameter configurations for related functions based on the impact,
dependency, and mutually exclusive relationships between the functions, as well
as the actual network scenario.
//Turning on the UL CRA switch only when the configured cell radius is less than 15 km
MOD ULCSALGOPARA: LocalCellId=0, UlCsSw=UL_COORD_RES_ALLOC_SWITCH-1;
## Optimization Command Examples
The parameter specifying the A3 reporting interval and that specifying the number
of A3 reporting times are shared by UL CRA and other features such as UL CoMP,
UL CPC, adaptive ICIC, eICIC, DL CoMP, CSPC, and GSM and LTE FDD Dynamic
Spectrum Sharing. When these features are all disabled, the A3 reporting interval
can be increased or the number of A3 reporting times can be reduced to decrease
signaling overhead. When any of these features is enabled, the influences of A3-
related parameter settings on these features must be considered. For details, see
the related feature parameter descriptions.
//Setting the A3 reporting interval to 6 minutes
MOD CELLMCPARA: LocalCellId=0, ReportInterval=6min;
//Setting the number of A3 reporting times to one
MOD CELLMCPARA: LocalCellId=0, ReportAmount=r1;
The eNodeB obtains the average load information of the local cell and
cooperating neighboring cells according to the information exchanged in the
coordinated set and then determines the interference control resource allocation
policy.
//Setting UlCoResAllocBandMode and UlCoResAllocRbLoadThld
MOD ULCSALGOPARA: LocalCellId=0, UlCoResAllocBandMode=INVALID, UlCoResAllocRbLoadThld=40;
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.18

## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Turning off the UL CRA switch
MOD ULCSALGOPARA: LocalCellId=0, UlCsSw=UL_COORD_RES_ALLOC_SWITCH-0;
4.4.1.3 Using the MAE-Deployment
●  Fast batch activation
This function can be batch activated using the Feature Operation and
Maintenance function of the MAE-Deployment. For detailed operations, see
the following section in the MAE-Deployment product documentation or
online help: MAE-Deployment Operation and Maintenance > MAE-
## Deployment Guidelines > Enhanced Feature Management > Feature
Operation and Maintenance.
●  Single/Batch configuration
This function can be activated for a single base station or a batch of base
stations on the MAE-Deployment. For detailed operations, see Feature
Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
●  Run the DSP ULCSNCELLINFO command to query neighboring cells in the UL
CRA cluster.
If the cluster is not empty, UL CRA has been activated.
●  Check the value of the counter
L.ChMeas.PRB.UL.CoordResAllocProtectUser.Used.Avg. If the value is not 0,
UL CRA has taken effect.
## 4.4.3 Network Monitoring
Monitor the average uplink edge-user throughput and average uplink user
throughput.
●  Average uplink edge-user throughput
The average uplink edge-user throughput can be calculated using:
(L.Thrp.bits.UL.BorderUE – L.Thrp.bits.UL.SmallPkt.BorderUE)/
L.Thrp.Time.UL.RmvSmallPkt.BorderUE
This throughput is expected to increase after UL CRA is activated.
## NO TE
Before monitoring edge-user-related counters, turn on the A3-based edge-user
identification switch and set an A3 offset for edge-user identification.
●  This switch is specified by the BasedA3EdgeUserSwitch option of the
CellCounterParaGroup.
CellCounterAlgoSwitch parameter.
●  The A3 offset for edge-user identification is specified by the
CellCounterParaGroup.EdgeUserA3Offset parameter. It is recommended that this
parameter be set to the same value as the UlCsAlgoPara.
UlCsA3Offset parameter.
●  Average uplink user throughput
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.19

The average uplink user throughput can be calculated using:
(L.Thrp.bits.UL – L.Thrp.bits.UE.UL.SmallPkt)/
L.Thrp.Time.UE.UL.RmvSmallPkt
This throughput is expected to either remain the same or slightly increase
after UL CRA is activated.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description4 UL CRA (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.20

## 5 UL CPC (FDD)
## 5.1 Principles
To use UL CPC for it to yield expected gains, the operator must first turn on the UL
CPC switch for all intra-frequency same-bandwidth cells in a planned area. This
minimizes the number of border cells. There are two terms of special relevance to
UL CPC as follows:
●  Border cell
A border cell is a cell with an excessively high proportion of neighboring cells
where UL CPC is not in effect in a UL CPC cluster.
●  UL CPC cluster
A UL CPC cluster of a cell is the set of all the neighboring cells cooperating for
## UL CPC.
When the UL_COORD_PC_SWITCH option of the UlCsAlgoPara.UlCsSw
parameter is selected, UL CPC is enabled, and the UL CPC procedure is performed,
as shown in Figure 5-1.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.21

Figure 5-1 UL CPC procedure
-  The eNodeB determines which cells will be in the UL CPC cluster of the local
cell.
The eNodeB removes all cells from the UL CPC cluster if the local cell meets
either of the following conditions:
–   The cell is deployed on an LBBPc.
–   The cell is a single frequency network (SFN) or adaptive SFN cell.
The eNodeB obtains a list of candidate neighboring cells from event A3
reports and arranges the cells in descending order based on the number of
event A3 reports that contain each cell. From these cells, the eNodeB selects
up to 14 cells that meet all of the following conditions and adds them to the
UL CPC cluster:
–   The cells are served by the same type of eNodeB (for example macro
eNodeBs) as the local cell.
–   The cells operate on the same frequency and have the same bandwidth
as the local cell.
–   The UL CPC switch is on.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.22

–   The cells are deployed on non-LBBPc BBPs.
–   The serving eNodeBs of the cells are connected to the local eNodeB
through X2 or eX2 interfaces, on which the one-way delay is less than 8
ms. The X2 interfaces must be configured to support coordination-based
services in non-ideal backhaul scenarios.
–   The cells are not high-speed cells.
–   The cells are not SFN or adaptive SFN cells.
UL CPC uses the same event A3 parameters as those for UL CRA, including
the UlCsAlgoPara.UlCsA3Offset parameter.
-  The eNodeB determines whether the local cell meets the following UL CPC
conditions:
–   The cell is a hotspot cell or within the cluster of a hotspot cell.
A cell is a hotspot cell when both of the following conditions are met:
▪The number of UEs in the cell is greater than the
UlCsAlgoPara.UlCoPcUserNumThd parameter value.
▪The interference of the cell is higher than the
UlCsAlgoPara.UlCoPcInThd parameter value.
–   The CPU load on the main control board is low for the cell.
A low CPU load is one that meets the following conditions:
## ▪
The average CPU usage is less than 70%.
## ▪
The maximum CPU usage is less than 75%.
–   The cell is not a border cell.
If all of these conditions are met, the eNodeB proceeds with 3. If any of them
is not met, the eNodeB uses the PUSCH closed-loop power control policy to
adjust the power of UEs in the local cell. For details, see 4.
-  The eNodeB determines the power control policy for the UEs.
–   The eNodeB uses the PUSCH closed-loop power control policy to adjust
the power of:
## ▪
UEs that have not reported event A3
## ▪
UEs running guaranteed bit rate (GBR), Voice over Internet Protocol
(VoIP), or push to talk (PTT) services
–   The eNodeB uses UL CPC to adjust the power of other UEs.
eNodeBs exchange scheduling and measurement information for
cooperating cells through the X2 or eX2 interfaces. The serving eNodeB
determines whether to increase or decrease the power of UEs in the local
cell based on the exchanged information and then delivers the relevant
commands to the UEs. This optimizes the overall scheduling performance
of the cells in the cluster.
-  The eNodeB checks whether the PuschRsrpHighThdSwitch option of the
CellAlgoSwitch.UlPcAlgoSwitch parameter is selected.
If UL CPC is used, the eNodeB performs the following operations:
–   Option not selected
The procedure ends.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.23

–   Option selected
The eNodeB uses the CellPcAlgo.PuschRsrpHighThd parameter value as
the RSRP upper limit. This corresponds to upper limit c in Figure 5-1.
If UL CPC does not take effect in the local cell or the UEs in the local cell do
not meet UL CPC conditions, the eNodeB uses PUSCH closed-loop power
control and performs the following operations:
–   Option not selected
▪If there are no hotspot cells in the cluster, the procedure ends.
▪If there are hotspot cells in the cluster, the eNodeB uses the
UlCsAlgoPara.UlCoPcRbkRsrpThd parameter value as the RSRP
upper limit. This corresponds to upper limit b in Figure 5-1.
–   Option selected
▪If there are no hotspot cells in the cluster, the eNodeB uses the
CellPcAlgo.PuschRsrpHighThd parameter value as the RSRP upper
limit. This corresponds to upper limit c in Figure 5-1.
▪If there are hotspot cells in the cluster, the eNodeB uses the smaller
value between the CellPcAlgo.PuschRsrpHighThd and
UlCsAlgoPara.UlCoPcRbkRsrpThd parameter values as the RSRP
upper limit. This corresponds to upper limit a in Figure 5-1.
For details about the RSRP upper limit function, see
## Power Control.
## 5.2 Network Analysis
## 5.2.1 Benefits
UL CPC controls interference and increases the average uplink user-perceived
throughput by up to 20% when the average uplink IN is greater than –105 dBm
and there is a medium-to-heavy load. In hotspot cells where UL CPC has taken
effect, gains vary with the average uplink RB usage:
●  RB usage of approximately 40%
UL CPC increases the average uplink user-perceived throughput by
approximately 5%.
●  RB usage of approximately 80%
UL CPC increases the average uplink user-perceived throughput by
approximately 20%.
●  RB usage of greater than 90% and MCS index of 20 or higher selected for
more than 20% UEs
UL CPC increases the average uplink user-perceived throughput by up to 5%.
The following are the main factors affecting UL CPC performance:
●  Number of uplink-synchronized UEs
When there are fewer uplink-synchronized UEs, the load is lower and there is
less interference. The gains are lower because UL CPC is less likely take effect.
UL CPC is generally recommended only when there are:
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.24

–   Over 150 uplink-synchronized UEs and at least 10 MHz of bandwidth
–   Over 80 uplink-synchronized UEs and 5 MHz of bandwidth
–   Over 60 uplink-synchronized UEs and 3 MHz of bandwidth
–   Over 40 uplink-synchronized UEs and 1.4 MHz of bandwidth
●  Inter-site distance
When the sites are farther apart, there is less interference and the gains will
be lower because UL CPC is less likely to take effect. In general, the average
inter-site distance tends to be less than 500 m.
●  One-way delay
When the one-way delay over the X2 interface supporting coordination-based
services or eX2 interface is less than 8 ms for information exchange between
cells, a shorter delay indicates better UL CPC performance.
●  BBP capability
When the BBP is less powerful, UL CPC is less likely to take effect, which
lowers the gains.
●  Amount of uncontrollable interference
If there is strong uncontrollable interference, UL CPC cannot help reduce
interference through power control and therefore cannot yield gains.
Uncontrollable interference includes:
–   Inter-RAT interference
–   Interference generated by repeaters
–   Interference from cells where UL CPC does not take effect
–   Intermodulation interference
–   Intra-RAT adjacent-channel interference such as that caused by a Double
Deck cell group described in
Flexible Bandwidth based on Overlap
Carriers (FDD)
## 5.2.2 Impacts
## Network Impacts
●  The throughput decreases significantly because cell center user (CCU) power
drops in cells that meet all of the following conditions:
–   The cell causes interference on hotspot cells.
–   The sum of the values of the counters L.UL.RSRP.PUSCH.Index20 to
L.UL.RSRP.PUSCH.Index23 exceeds 80% of the values of all similar
counters.
–   The uplink PRB usage exceeds 90%.
In this situation, UL CPC does not necessarily increase the overall average
uplink user-perceived throughput of the UL CPC deployment area even if
average uplink user-perceived throughput increases significantly in hotspot
cells.
●  UL CPC relies on A3 reporting, and therefore there are the following
additional impacts:
–   New A3 reports increase the signaling processing overhead. The value of
L.Signal.Num.Uu will go up and the CPU usage of the main control
board will increase by less than 5%.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.25

–   User-plane resources will be preempted for A3 reporting. If the uplink and
downlink RBs and control channel elements (CCEs) are insufficient, the
Cell Downlink Average Throughput value will drop by less than 5% and
the downlink packet delay will increase by less than 5%.
●  In relaxed backhaul scenarios, when UL CPC and other features involving the
coordination of multiple eNodeBs (such as UL CoMP and CA) are enabled
together, they share transmission bandwidths. When the transmission
bandwidths are insufficient, the delays increase and the gains of these
features are affected.
## Function Impacts
## Function
## Name
Function SwitchReferenceDescription
Uplink MU-
## MIMO
UlVmimoSwitch
option of the
CellAlgoSwitch.UlSch
Switch parameter
MIMOUL CPC has a high
probability of
reducing the power of
the CCUs, and
therefore decreasing
the chance that UEs
will be paired for
multi-user multiple-
input multiple-output
## (MU-MIMO).
SFN cellCell.MultiRruCellMo
de
SFNUL CPC does not take
effect in SFN or
adaptive SFN cells.
This is because:
● SFN or adaptive
SFN is generally
used in low-load
scenarios, which
are not the target
application
scenarios of UL
## CPC.
● The uplink
interference
estimated by UL
CPC based on
event A3
measurement is
not accurate for
SFN or adaptive
SFN cells.
Therefore, the
percentage of SFN or
adaptive SFN cells in
the target area must
be less than 20%.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.26

## Function
## Name
Function SwitchReferenceDescription
## Automatic
congestion
handling
## FDD_ACH_SWITCH
option of the
ParaAutoOptCfg.Ach
EffectiveType
parameter
## Automatic
## Congestion
## Handling
If UL CPC and
limitation on PUSCH
power (an intelligent
optimization function
in automatic
congestion handling)
are both enabled, the
intelligent
optimization function
affects UL CPC
performance. This
occurs when the
ParaAutoOptCfg.
## PUS
CHRsrpHighThd4Aut
oOpt
parameter value
is less than –82 dBm.
A smaller parameter
value leads to a
greater impact, and
UL CPC will not take
effect when the
parameter is set to a
sufficiently small
value.
eMTC
introduction
CellEmtcAlgo.EmtcAl
goSwitch
eMTCUL CPC does not take
effect for eMTC UEs.
Uplink CACaUl2CCSwitch
option of the
CaMgtCfg.CellCaAlgo
Switch parameter
## Carrier
## Aggregation
Heavy load or
interference limitation
seldom occurs in
SCells when uplink CA
is enabled. Therefore,
UL CPC is currently
not used for SCells.

## 5.3 Requirements
## 5.3.1 Licenses
Feature ID
Feature NameModelSales Unit
LOFD-081206Uplink Coordinated
## Scheduling
## LT1SICUAMC0
## 0
## Per Cell

eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.27

## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## Function
## Name
Function SwitchReference
## Scheduler-
controlled
power
SchedulerCtrlPo-
werSwitch option of
the
CellAlgoSwitch.UlSch
Switch parameter
## Scheduling
## PUSCH
## Transmit
## Power
## Adjustment
with Dynamic
## Scheduling
## Applied
InnerLoopPuschS-
witch option of the
CellAlgoSwitch.UlPcA
lgoSwitch parameter
## Power Control

## Mutually Exclusive Functions
## Function
## Name
Function SwitchReferenceDescription
High speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
The functions cannot
work with UL CPC.
This is because UL
CPC does not deliver
gains in high-speed
cells due to their
high-speed moving
UEs.
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
Cell radius
greater than
15 km
NoneExtended Cell
## Range
The functions cannot
work with UL CPC.
This is because UL
CPC does not deliver
gains in cells with a
radius exceeding 15
km due to their low
traffic volume and
limited coverage.
Cell radius
greater than
100 km
NoneExtended Cell
## Range
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.28

## Function
## Name
Function SwitchReferenceDescription
In-band relayInBandRelayDeNbS-
witch and
InBandRelayReNbS-
witch options of the
CellAlgoSwitch.Relay
## Switch
parameter
RelayNone
LTE FDD and
NR Uplink
## Spectrum
## Sharing
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_UPLINK_SPE
## CTRUM_SHR
LTE FDD and
NR Uplink
## Spectrum
## Sharing
## None
Hybrid DSS
Based on
## Asymmetric
## Bandwidth
## LNR_SPECTRUM_SHR
_ASYM_SW option of
the
SpectrumCloud.Spect
rumCloudEnhSwitch
parameter with
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_SPECTRUM_S
## HR
LTE FDD and
NR Spectrum
## Sharing
## None
LTE FDD and
NR Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_SPECTRUM_S
## HR
LTE FDD and
NR Spectrum
## Sharing
## None
Short TTISHORT_TTI_SW
option of the
CellShortTtiAlgo.Stti
AlgoSwitch
parameter
Short TTI
## (FDD)
## None
Uplink single-
side in-band
interference
management
UlInterfSuppressCfg.
UlSingleSideIntr-
fImpMitSw
## Interference
Detection and
## Suppression
## None

## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.29

## Base Station Models
For FDD, the following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  BTS3912E
## ●  BTS3911E
## Boards
Non-LBBPc BBPs
RF Modules
No requirements
## 5.3.4 Cells
●  The RX mode of the antenna is 1R, 2R, or 4R.
●  eNodeBs providing the cells in a cluster are all macro eNodeBs, micro
eNodeBs, or LampSite eNodeBs.
●  An X2 interface that supports coordination-based services in non-ideal
backhaul scenarios, or an eX2 interface, is available.
The one-way delay for the interface must be less than 8 ms. For details about
X2 interface support for coordination-based services in non-ideal backhaul
scenarios, see
S1 and X2 Self-Management.
In addition, IP PM sessions of forward activation type are recommended for
delay detection.
Configuring an IP PM session of bidirectional activation at either end of an
eX2 interface needs to be avoided. This is because eNodeBs automatically
create IP PM sessions to detect eX2 link status. An IP PM session of
bidirectional activation type may conflict with an automatically created
session. If this is the case, the eX2 interface will fail to work properly.
●  There are no PCI conflicts.
PCI conflicts can occur when two involved cells have the same PCI. If there is
a PCI conflict, the eNodeB may incorrectly select a cell in the UL CPC cluster
because it cannot differentiate between the two cells based on the
measurement reports from the UE. You are advised to set the
ENodeBAlgoSwitch.
PciConflictAlmSwitch parameter to ON so that PCI
conflicts can be reported.
●  There is no intermodulation interference.
If there is intermodulation interference, the eNodeB cannot eliminate the
interference or prevent its impact by using resource coordination.
## 5.3.5 Others
No requirements
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.30

5.4 Operation and Maintenance
## 5.4.1 Data Configuration
## 5.4.1.1 Data Preparation
Table 5-1 and Table 5-2 describe the parameters used for function activation and
optimization.
Table 5-1 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
UL CS SwitchUlCsAlgoPara.UlCsSwUL_COORD_P
## C_SWITCH
Select this option.

Table 5-2 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
## UL
## Coordinated
## PC IN
## Threshold
UlCsAlgoPara.UlCoPc
InThd
Set this parameter to the
recommended value.
## UL
## Coordinated
PC User
## Number
## Threshold
UlCsAlgoPara.UlCoPc
UserNumThd
Set this parameter to the
recommended value.
## UL
## Coordinated
PC Rollback
## RSRP
## Threshold
UlCsAlgoPara.UlCoPc
RbkRsrpThd
Set this parameter to the
recommended value.
## UL CS A3
## Offset
UlCsAlgoPara.UlCsA3
## Offset
Set this parameter to the
recommended value.
## PUSCH RSRP
## High
## Threshold
CellPcAlgo.PuschRsrp
HighThd
If the PuschRsrpHighThdSwitch
option of the
CellAlgoSwitch.UlPcAlgoSwitch
parameter is selected, set this
parameter to –82 dBm or above to
reduce the impact of the RSRP upper
limit function on UL CPC.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.31


5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
Before using MML commands, refer to 5.2.2 Impacts and 5.3.2 Software and
complete the parameter configurations for related functions based on the impact,
dependency, and mutually exclusive relationships between the functions, as well
as the actual network scenario.
//Turning on the UL CPC switch only when the configured cell radius is less than 15 km
MOD ULCSALGOPARA: LocalCellId=0, UlCoPcInThd=-105, UlCoPcRbkRsrpThd=-96,
UlCoPcUserNumThd=150, UlCsA3Offset=-20, UlCsSw=UL_COORD_PC_SWITCH-1;
## Optimization Command Examples
The parameter specifying the A3 reporting interval and that specifying the number
of A3 reporting times are shared by UL CPC and other features such as UL CoMP,
UL CRA, adaptive ICIC, eICIC, DL CoMP, CSPC, and GSM and LTE FDD Dynamic
Spectrum Sharing. When these features (excluding UL CPC) are all disabled, the
A3 reporting interval can be increased or the number of A3 reporting times can be
reduced to decrease signaling overhead. When any of these features is enabled
together with UL CPC, the influences of A3-related parameter settings on these
features must be considered. For details, see the related feature parameter
descriptions.
//Setting the RSRP upper limit for the PUSCH
MOD CELLPCALGO: LocalCellId=0, PuschRsrpHighThd=-82;
//Setting the A3 reporting interval to 6 minutes
MOD CELLMCPARA: LocalCellId=0, ReportInterval=6min;
//Setting the number of A3 reporting times to 1
MOD CELLMCPARA: LocalCellId=0, ReportAmount=r1;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Turning off the UL CPC switch
MOD ULCSALGOPARA: LocalCellId=0, UlCsSw=UL_COORD_PC_SWITCH-0;
5.4.1.3 Using the MAE-Deployment
●  Fast batch activation
This function can be batch activated using the Feature Operation and
Maintenance function of the MAE-Deployment. For detailed operations, see
the following section in the MAE-Deployment product documentation or
online help: MAE-Deployment Operation and Maintenance > MAE-
## Deployment Guidelines > Enhanced Feature Management > Feature
Operation and Maintenance.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.32

●  Single/Batch configuration
This function can be activated for a single base station or a batch of base
stations on the MAE-Deployment. For detailed operations, see Feature
Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
●  Run the DSP ULCSNCELLINFO command to query neighboring cells in the UL
CPC cluster.
If the cluster is not empty, UL CPC has been activated.
●  Check the value of the counter L.ULCPC.User.Avg. If the value is not 0, UL
CPC has taken effect.
## 5.4.3 Network Monitoring
Monitor the uplink interference, RSRP, and throughput.
●  Uplink IN and RSRP
For long-term (≥ 24 hours) measurements using L.UL.Interference.Avg and
L.UL.Interference.Max, the average and maximum interference levels are
expected to decrease after UL CPC is activated.
The numbers of times the eNodeB detects UE-level RSRP within the ranges
(L.UL.RSRP.PUSCH.Index0 to L.UL.RSRP.PUSCH.Index23) with relatively large
indexes are expected to decrease.
●  Average uplink user-perceived throughput and uplink throughput distribution
in different ranges
–   Average uplink user-perceived throughput
The average uplink user-perceived throughput can be calculated using:
L.Thrp.bits.UE.UL.Experienced/L.Thrp.Time.UE.UL.Experienced
This throughput is expected to increase after UL CPC is activated.
–   Uplink throughput distribution in different ranges
The uplink throughput distribution in different ranges can be found using
the counters L.Thrp.UL.BitRate.Samp.Index0 through
L.Thrp.UL.BitRate.Samp.Index9.
In the measurement results, the number of samples is expected to
decrease in the ranges with relatively smaller indexes after UL CPC is
activated.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
Description5 UL CPC (FDD)
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.33

## 6 Parameters
The following hyperlinked EXCEL files of parameter documents match the
software version with which this document is released.
●  Node Parameter Reference: contains device and transport parameters.
●  eNodeBFunction Parameter Reference: contains all parameters related to
radio access functions, including air interface management, access control,
mobility control, and radio resource management.
●  eNodeBFunction Used Reserved Parameter List: contains the reserved
parameters that are in use and those that have been disused.
## NO TE
You can find the EXCEL files of parameter reference and used reserved parameter list for
the software version used on the live network from the product documentation delivered
with that version.
FAQ 1: How do I find the parameters related to a certain feature from
parameter reference?
Step 1Open the EXCEL file of parameter reference.
Step 2On the Parameter List sheet, filter the Feature ID column. Click Text Filters and
choose Contains. Enter the feature ID, for example, LOFD-001016 or
## TDLOFD-001016.
Step 3Click OK. All parameters related to the feature are displayed.
----End
FAQ 2: How do I find the information about a certain reserved parameter
from the used reserved parameter list?
Step 1Open the EXCEL file of the used reserved parameter list.
Step 2On the Used Reserved Parameter List sheet, use the MO, Parameter ID, and BIT
columns to locate the reserved parameter, which may be only a bit of a parameter.
View its information, including the meaning, values, impacts, and product version
in which it is activated for use.
----End
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description6 Parameters
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.34

## 7 Counters
The following hyperlinked EXCEL files of performance counter reference match the
software version with which this document is released.
●  Node Performance Counter Summary: contains device and transport counters.
●  eNodeBFunction Performance Counter Summary: contains all counters related
to radio access functions, including air interface management, access control,
mobility control, and radio resource management.
## NO TE
You can find the EXCEL files of performance counter reference for the software version used
on the live network from the product documentation delivered with that version.
FAQ: How do I find the counters related to a certain feature from
performance counter reference?
Step 1Open the EXCEL file of performance counter reference.
Step 2On the Counter Summary(En) sheet, filter the Feature ID column. Click Text
Filters and choose Contains. Enter the feature ID, for example, LOFD-001016 or
## TDLOFD-001016.
Step 3Click OK. All counters related to the feature are displayed.
----End
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description7 Counters
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.35

## 8 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description8 Glossary
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.36

## 9 Reference Documents
-  3GPP TS 36.331: "RRC Protocol Specification"
## 2.
UL CoMP
3.Scheduling
4.S1 and X2 Self-Management
5.Carrier Aggregation
6.High Speed Mobility
7.Physical Channel Resource Management
## 8.MIMO
9.VoLTE
10.Flexible Bandwidth based on Overlap Carriers (FDD)
11.Compact Bandwidth (FDD)
12.Extended Cell Range
13.CDMA and LTE Zero Bufferzone
14.Relay
15.Power Control
## 16.SFN
17.Automatic Congestion Handling
18.eMTC
19.Short TTI (FDD)
20.LTE FDD and NR Uplink Spectrum Sharing
21.Superior Uplink Coverage (FDD)
22.LTE FDD and NR Spectrum Sharing
23.Massive MIMO (FDD)
24.Interference Detection and Suppression
eRAN
## Uplink Coordinated Scheduling Feature Parameter
## Description9 Reference Documents
Issue 06 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.37