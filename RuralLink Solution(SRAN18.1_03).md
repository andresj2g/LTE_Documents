

SingleRAN
RuralLink Solution Guide
## Issue03
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
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 SRAN18.1 03 (2023-12-22)..................................................................................................................................................1
1.2 SRAN18.1 02 (2023-09-14)..................................................................................................................................................1
1.3 SRAN18.1 01 (2023-04-23)..................................................................................................................................................2
2 About This Document.............................................................................................................3
2.1 General Statements................................................................................................................................................................ 3
2.2 Applicable RAT......................................................................................................................................................................... 3
3 Principles................................................................................................................................... 4
3.1 Overview.................................................................................................................................................................................... 4
3.2 Equipment Requirements..................................................................................................................................................... 5
3.3 Application Scenarios.............................................................................................................................................................6
4 RuralLink Solution (LTE)........................................................................................................7
4.1 Principles.................................................................................................................................................................................... 7
4.2 Network Analysis.....................................................................................................................................................................8
4.2.1 Benefits....................................................................................................................................................................................8
4.2.2 Impacts.................................................................................................................................................................................... 8
4.3 Requirements......................................................................................................................................................................... 13
4.3.1 Licenses................................................................................................................................................................................. 13
4.3.2 Software................................................................................................................................................................................13
4.3.3 Hardware..............................................................................................................................................................................15
4.3.4 Networking.......................................................................................................................................................................... 16
4.3.5 Cells........................................................................................................................................................................................ 16
4.3.6 Others....................................................................................................................................................................................16
4.4 Operation and Maintenance.............................................................................................................................................16
4.4.1 Data Configuration........................................................................................................................................................... 16
4.4.1.1 Data Preparation............................................................................................................................................................ 16
4.4.1.2 Using MML Commands............................................................................................................................................... 17
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 18
4.4.2 Activation Verification......................................................................................................................................................18
4.4.3 Network Monitoring.........................................................................................................................................................18
4.4.4 Possible Issues.................................................................................................................................................................... 18
5 RuralLink Solution (UMTS).................................................................................................19
SingleRAN
RuralLink Solution GuideContents
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.iii

5.1 Principles.................................................................................................................................................................................. 19
5.2 Network Analysis.................................................................................................................................................................. 19
5.2.1 Benefits................................................................................................................................................................................. 19
5.2.2 Impacts..................................................................................................................................................................................19
5.3 Requirements......................................................................................................................................................................... 20
5.3.1 Licenses................................................................................................................................................................................. 20
5.3.2 Software................................................................................................................................................................................21
5.3.3 Hardware..............................................................................................................................................................................21
5.3.4 Networking.......................................................................................................................................................................... 21
5.3.5 Cells........................................................................................................................................................................................ 22
5.3.6 Others....................................................................................................................................................................................22
5.4 Operation and Maintenance.............................................................................................................................................22
5.4.1 Data Configuration........................................................................................................................................................... 22
5.4.1.1 Data Preparation............................................................................................................................................................ 22
5.4.1.2 Using MML Commands............................................................................................................................................... 22
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 23
5.4.2 Activation Verification......................................................................................................................................................23
5.4.3 Network Monitoring.........................................................................................................................................................23
5.4.4 Possible Issues.................................................................................................................................................................... 24
6 RuralLink Solution (GSM)...................................................................................................25
6.1 Principles.................................................................................................................................................................................. 25
6.2 Network Analysis.................................................................................................................................................................. 25
6.2.1 Benefits................................................................................................................................................................................. 25
6.2.2 Impacts..................................................................................................................................................................................25
6.3 Requirements......................................................................................................................................................................... 26
6.3.1 Licenses................................................................................................................................................................................. 26
6.3.2 Software................................................................................................................................................................................26
6.3.3 Hardware..............................................................................................................................................................................26
6.3.4 Networking.......................................................................................................................................................................... 27
6.3.5 Cells........................................................................................................................................................................................ 27
6.3.6 Others....................................................................................................................................................................................27
6.4 Operation and Maintenance.............................................................................................................................................27
6.4.1 Data Configuration........................................................................................................................................................... 27
6.4.1.1 Data Preparation............................................................................................................................................................ 28
6.4.1.2 Using MML Commands............................................................................................................................................... 28
6.4.1.3 Using the MAE-Deployment...................................................................................................................................... 29
6.4.2 Activation Verification......................................................................................................................................................29
6.4.3 Network Monitoring.........................................................................................................................................................29
6.4.4 Possible Issues.................................................................................................................................................................... 29
7 Parameters..............................................................................................................................30
8 Counters.................................................................................................................................. 31
SingleRAN
RuralLink Solution GuideContents
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.iv

9 Glossary................................................................................................................................... 32
10 Reference Documents........................................................................................................ 33
SingleRAN
RuralLink Solution GuideContents
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.v

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
## 1.1 SRAN18.1 03 (2023-12-22)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised the descriptions of microwave equipment requirements. For details, see
## 3.2 Equipment Requirements.
## 1.2 SRAN18.1 02 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions of the general principles. For details, see 3.1 Overview.
SingleRAN
RuralLink Solution Guide1 Change History
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.1

## 1.3 SRAN18.1 01 (2023-04-23)
This issue is the first release.
SingleRAN
RuralLink Solution Guide1 Change History
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.2

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
This document applies to GSM, UMTS, LTE FDD, and NB-IoT.
SingleRAN
RuralLink Solution Guide2 About This Document
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.3

## 3 Principles
## 3.1 Overview
Establishing a separate network in sparsely-populated areas not only wastes
resources but also increases costs. Therefore, existing spectrum resources are used
to transmit signals from the existing network to the target base stations, realizing
low-cost coverage for remote areas.
In a conventional solution, optical fibers are used to connect a baseband unit
(BBU) and remote radio units (RRUs) for good reliability. However, in scenarios
such as filling coverage holes in suburban areas, extending coverage in rural areas,
and providing offshore super-distance coverage, long optical fibers are required
once used, which involves long deployment period and in some conditions, optical
fibers are unreachable. As such, the wireless transmission solution is required. In
Huawei's previous wireless backhaul solutions, such as the LTE Relay solution (For
details, see
Relay in eRAN feature documentation), a complete base station still
needs to be set up remotely and an independent BBU is required. The RuralLink
solution uses the existing BBU on the network side to transmit signals between
microwave and RRUs. This solution addresses coverage problems in scenarios
where the optical fiber deployment distance or period is long, or optical fibers are
unreachable, and reduces costs.
Figure 3-1 shows the architectures of the optical fiber transmission, wireless
backhaul solution, and RuralLink solution.
SingleRAN
RuralLink Solution Guide3 Principles
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.4

Figure 3-1 Architectures of optical fiber transmission, wireless backhaul solution,
and RuralLink solution
The RuralLink solution uses the remote radio technology to transmit signals
between BBUs and RRUs using microwave. The BBU and RRU use common public
radio interface (CPRI) frames for transmission while the microwave uses Ethernet
frames for transmission. Therefore, COEs are added between the BBU and the
microwave equipment and between the microwave equipment and the RRU for
interface conversion. The RuralLink solution allows microwave equipment and
RRUs working on different frequency bands to be flexibly networked with BBUs to
implement wireless fronthaul. For details about the COE, see
COE5902 User Guide
in 3900 & 5900 Series Base Station Product Documentation.
Cells deployed with the RuralLink solution are referred to as RuralLink cells in this
document.
## 3.2 Equipment Requirements
## Microwave Equipment
The RuralLink solution must be used with Huawei RTN 320F microwave products.
For details about RTN 320F microwave products, see RTN 320&320F product
documentation.
When the RuralLink solution is used, microwave equipment must meet the
following requirements:
●  All microwave equipment must be configured to work in low-latency mode.
●  The RuralLink solution is deployed in areas with good weather conditions
without rainstorms. Otherwise, the cells may be activated and deactivated
repeatedly.
SingleRAN
RuralLink Solution Guide3 Principles
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.5

●  The bandwidth notification function is enabled and set to periodic reporting
on all microwave equipment that is directly connected to the COE. The
microwave bandwidth notification value must be greater than the bandwidth
planned for the base station. Otherwise, the base station cannot detect the
microwave bandwidth. Consequently, the links may be unreachable.
●  All microwave equipment must be synchronized with the COE on the BBU
side. Otherwise, alarms may be generated and links may be unreachable.
## NO TE
For details about the medium- and low-latency mode, bandwidth notification function, and
clock status check related to the RTN 320F, see RTN 320&320F product documentation.
## Base Station
The introduction of microwave and COEs will cause an extra delay equivalent to
20 km in transmission distance. In addition, the maximum air-interface distance
between microwave equipment is 20 km. Therefore, the distance between the RRU
and the BBU must be greater than or equal to 40 km.
## 3.3 Application Scenarios
The RuralLink solution supports single-mode and multimode scenarios.
Single-Mode Scenario
The RuralLink solution supports the following single-mode scenarios:
## ●  GSM
## ●  UMTS
## ●  LTE FDD
●  NB-IoT
## Multimode Scenario
The RuralLink solution supports multiple modes. It is recommended that the
following multi-mode scenarios be preferentially considered:
## ●  GSM+UMTS
## ●  GSM+LTE FDD
## ●  GSM+UMTS+LTE FDD
## ●  UMTS+LTE FDD
SingleRAN
RuralLink Solution Guide3 Principles
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.6

4 RuralLink Solution (LTE)
## 4.1 Principles
The RuralLink solution is controlled by the CellTypeExt.
WirelessFhCellFlag
parameter.
●  If this parameter is set to TRUE, the RuralLink solution is used for LTE cells.
●  If this parameter is set to FALSE, the RuralLink solution is not used for LTE
cells.
The RuralLink solution applies to rural networks. To reduce the requirements for
microwave transmission bandwidth, a higher CPRI compression ratio is supported
when some RRUs are used. For details, see Table 4-1. The CPRI compression ratio
is specified by the Cell.
CPRICompression parameter.
Table 4-1 Maximum CPRI compression ratio
## Cell
## Bandwidth
Cell TX/RX
## Mode
Maximum CPRI
## Compression Ratio
Supported by the
RuralLink Solution
Maximum CPRI
## Compression Ratio
Supported by a
## Common Cell
1.4 MHz and
3 MHz
## 1T1R, 1T2R,
2T2R, and
## 2T4R
No compressionNo compression
5 MHz1T1R, 1T2R,
2T2R, and
## 2T4R
2:1No compression
10 MHz, 15
MHz, and 20
MHz
## 1T1R, 1T2R,
2T2R, and
## 2T4R
## 4:13:1

For details about CPRI compression, see
CPRI Compression in eRAN feature
documentation.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.7

## 4.2 Network Analysis
## 4.2.1 Benefits
●  This solution is mainly used to address coverage problems in scenarios where
the optical fiber deployment distance or period is long, or optical fibers are
unreachable. The performance of microwave transmission varies greatly due
to the environment, weather, season, and blocking area.
●  Sites where the RuralLink solution is deployed use the BBUs of existing sites,
eliminating the need to install new BBUs and reducing costs.
## 4.2.2 Impacts
## Network Impacts
The base station reserves dedicated bandwidth for GSM. When a GSM cell is
added or removed, the LTE cells will be reestablished. For details about the
dedicated bandwidth reserved for GSM, see 6.1 Principles.
## Function Impacts
## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
## CSI-RS
configuration
CellCsiRsParaCfg.CsiR
sSwitch
NoneTM9 is not
recommended for
RuralLink cells.
Therefore, it is
recommended that
the
CellCsiRsParaCfg.
CsiR
sSwitch parameter be
set to NOT_CFG.
Mode of
Multi-RRU
## Cell
Cell.MultiRruCellMo
de set to
## TWO_RRU_COMBINA
## TION
NoneIf the
Cell.MultiRruCellMo
de parameter is set to
## TWO_RRU_COMBINA
TION, the RuralLink
cells will fail to be
activated.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.8

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
## Carrier
aggregation
●CaGroupCell.Local
CellId
●CaGroupSCellCfg.S
CellLocalCellId
●FreqCfgSwitch
and
HoWithSccCfgSwi
tch options of the
ENodeBAlgoSwitc
h.
CaAlgoSwitch
parameter
## Carrier
## Aggregation
RuralLink cells do not
support carrier
aggregation.
● If there is an X2
interface between
base stations, a
RuralLink cell
needs to broadcast
information that it
does not support
CA through the X2
interface but the
broadcast is
delayed. Before the
broadcast is
complete, CA-
capable
neighboring cells
are not informed of
the RuralLink cell's
incompatibility
with CA. If a CA UE
is handed over to
the RuralLink cell
for PCC anchoring,
CA stops taking
effect for the UE
and the SCells of
the UE are
released. In this
case, the CA UE
becomes a non-CA
## UE.
● If there is no X2
interface between
base stations, CA-
capable
neighboring cells
cannot be
informed of
RuralLink cells'
incompatibility
with CA. If a CA UE
is handed over to
the RuralLink cell
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.9

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
for PCC anchoring,
CA stops taking
effect for the UE
and the SCells of
the UE are
released. In this
case, the CA UE
becomes a non-CA
## UE.
● If CA fails between
an inter-base-
station neighboring
cell that serves as
the PCell and a
RuralLink cell that
serves as an SCell,
the CA capacity
consumed by the
inter-base-station
neighboring cell
will be released
after a period of
time, which is
specified by the
CaMgtCfg.
SCellAg
ingTime
parameter.
## Flexible
bandwidth
based on
overlapping
carriers
●DdCellGroup.Local
CellId1
●DdCellGroup.Local
CellId2
●DdCellGroup.DdBa
ndwidth
## Flexible
## Bandwidth
based on
## Overlap
## Carriers
## (FDD)
RuralLink cells do not
support flexible
bandwidth based on
overlapping carriers.
## Zero Guard
## Band
## Between
## Contiguous
Intra-Band
## Carriers
## CONTIG_INTRA_BAN
D_CARR_SW option
of the
ContigIntraBand-
Carr.ContigIntraBand
CarrSw
parameter
## Seamless
Intra-Band
## Carrier
Joining (FDD)
RuralLink cells do not
support Zero Guard
## Band Between
Contiguous Intra-Band
## Carriers.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.10

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
Intra-BBP UL
CoMP
## ● Macro-macro
CoMP and micro-
micro CoMP:
UlJointReceptionS
witch option of the
CellAlgoSwitch.
## Up
linkCompSwitch
parameter
## ● Macro-micro
CoMP:
UlJointReceptionS
witch and
UlHetnetJointRe-
ceptionSwitch
options of the
CellAlgoSwitch.
## Up
linkCompSwitch
parameter
UL CoMPRuralLink cells do not
support intra-BBP UL
CoMP.
Intra-eNodeB
inter-BBP UL
CoMP
## ● Macro-macro
CoMP and micro-
micro CoMP:
UlJointReception-
PhaseIISwitch
option of the
CellAlgoSwitch.
## Up
linkCompSwitch
parameter
## ● Macro-micro
CoMP:
UlJointReception-
PhaseIISwitch and
UlHetnetJointRe-
ceptionSwitch
options of the
CellAlgoSwitch.
## Up
linkCompSwitch
parameter
UL CoMPRuralLink cells do not
support intra-eNodeB
inter-BBP UL CoMP.
3-cell UL
CoMP
UlJointReception3Cel
lSwitch option of the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
UL CoMPRuralLink cells do not
support 3-cell UL
CoMP.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.11

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
## Neighboring
cell addition
for SRS
measurement
for UL CoMP
UlHetnetCompManu
alNcellCfgSw option
of the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
UL CoMPRuralLink cells do not
support neighboring
cell selection for UL
CoMP-specific SRS
measurement.
UL CoMP-
specific SRS
measurement
UlHetnetCompOnUlR
srpSw option of the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
UL CoMPRuralLink cells do not
support UL CoMP-
specific SRS
measurement.
Type-2 intra-
eNodeB inter-
BBP UL CoMP
UlCompInterBoard-
Type2Sw option of
the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
UL CoMPRuralLink cells do not
support type-2 intra-
eNodeB inter-BBP UL
CoMP.
Inter-eNodeB
UL CoMP for
video services
UlCompForVideoS-
witch option of the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
## Video
## Experience
## Optimization
RuralLink cells do not
support inter-eNodeB
UL CoMP for video
services.
CoMP scope
expansion
WideRangeCompSwi
tch option of the
CellAlgoSwitch.Uplin
kCompSwitch
parameter
NoneRuralLink cells do not
support CoMP scope
expansion.
DL CoMP with
## TM10
FDDHomNetDlComp
Switch and
FDDHetNetDlCompS-
witch options of the
CellAlgoSwitch.DlCo
mpSwitch
parameter
DL CoMP
## (FDD)
RuralLink cells do not
support DL CoMP with
## TM10.
Uplink joint
interference
locating
## UL_JOINT_INTRF_PO
SITION_SW option of
the
UlInterfSuppressCfg.
UlJointIntrfManage-
mentSw
parameter
NoneRuralLink cells do not
support uplink joint
interference locating.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.12

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
Uplink joint
interference
suppression
## UL_JOINT_INTRF_SU
PPRESS_SW option of
the
UlInterfSuppressCfg.
UlJointIntrfManage-
mentSw
parameter
## Interference
Detection and
## Suppression
RuralLink cells do not
support uplink joint
interference
suppression.
## Narrowband
interference
scheduling
optimization
## UL_NARROWBAND_I
## NTRF_SCH_OPT_SW
option of the
UlInterfSuppressCfg.
UlJointIntrfManage-
mentSw
parameter
## Interference
Detection and
## Suppression
RuralLink cells do not
support narrowband
interference
scheduling
optimization.
DL 64QAMNoneNoneWhen the CPRI
compression ratio is
4:1 in a RuralLink cell
with a bandwidth of
10 MHz, 15 MHz, or
20 MHz, the DL
64QAM function may
not provide optimal
gains.

## 4.3 Requirements
## 4.3.1 Licenses
There are no license requirements for basic functions.
## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.13

## Mutually Exclusive Functions
## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
High speed
mobility
Cell.HighSpeedFlag
set to HIGH_SPEED
## High Speed
## Mobility
For RuralLink cells, the
Cell.HighSpeedFlag
parameter must be
set to LOW_SPEED.
Ultra high
speed
mobility
Cell.HighSpeedFlag
set to
## ULTRA_HIGH_SPEED
## High Speed
## Mobility
For RuralLink cells, the
Cell.HighSpeedFlag
parameter must be
set to LOW_SPEED.
CRS Port
## Number
Cell.CrsPortNumNoneFor RuralLink cells, if
the Cell.TxRxMode
parameter is set to
1T1R, 1T2R, 2T2R, or
2T4R, the
## Cell.
CrsPortNum
parameter cannot be
set to CRS_PORT_4.
Flag of multi-
RRU cell
Cell.MultiRruCellFlagNoneFor RuralLink cells, the
Cell.MultiRruCellFlag
parameter must be
set to
## BOOLEAN_FALSE.
Inter-eNodeB
SFN based on
eNodeB
coordination
Cell.EuCellStandbyM
ode
SFNFor RuralLink cells, the
Cell.EuCellStandbyM
ode parameter must
be set to ACTIVE.
## Multi Cell
## Share Mode
Cell.MultiCellShareM
ode
NoneFor RuralLink cells, the
Cell.MultiCellShareM
ode parameter must
be set to NORMAL.
Virtual 4T4RVirtual4T4RSwitch
option of the
CellAlgoSwitch.Emim
oSwitch parameter
Virtual 4T4R
## (FDD)
RuralLink cells do not
support virtual 4T4R.
## Network-
assisted
interference
cancellation
and
suppression
CellAlgoSwitch.Naics
## Switch
## Network
## Assisted
## Interference
## Cancellation
RuralLink cells do not
support network-
assisted interference
cancellation and
suppression.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.14

## Function
## Name
Function SwitchReference
(eRAN
## Feature
## Documentati
on)
## Description
eICICCellAlgoSwitch.EicicS
witch
NoneFor RuralLink cells, the
CellAlgoSwitch.EicicS
witch parameter must
be set to OFF.
FeICICCellAlgoSwitch.Feicic
## Switch
TDM eICIC
## (FDD)
For RuralLink cells, the
CellAlgoSwitch.Feicic
Switch parameter
must be set to OFF.
NB-IoT
network
deployment
Prb.DeployModeNB-IoT Basics
## (FDD)
NB-IoT Basics
## (FDD)
For a RuralLink cell,
the Prb.DeployMode
parameter cannot be
set to IN_BAND.
Short TTISHORT_TTI_SW
option of the
CellShortTtiAlgo.Stti
AlgoSwitch
parameter
Short TTI
## (FDD)
RuralLink cells do not
support short TTI.

## 4.3.3 Hardware
The hardware described in this section must support FDD, and the configured
work modes must include FDD.
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
5900 series base stations (macro base stations)
BBUs
Only the BBU5900 and BBU5900A support this function.
## Boards
●  Main control board: Only the UMPTa, UMPTb, UMPTe, UMPTg, and UMPTga
series boards are supported.
●  Baseband processing unit: Only the UBBPe and UBBPg series boards are
supported.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.15

RF Modules
●  Only 5000 series RRUs support this function.
●  Only the RRU5304w (700 MHz) and RRU5909 (900 MHz PGSM and 900 MHz
EGSM) support 2:1 compression for the 5 MHz bandwidth and 4:1
compression for the 10 MHz, 15 MHz, and 20 MHz bandwidths. For details
about other CPRI compression ratios, see
CPRI Compression in eRAN feature
documentation.
## 4.3.4 Networking
●  Only the chain topology is supported. In each sector, only one RRU can be
connected to the COE, and a maximum of three RRUs can be cascaded.
●  The maximum air-interface distance between microwave equipment is 20 km.
●  The BBU/RRU/microwave equipment is connected to the COE through optical
fibers and the total length of the four-segment optical fibers cannot exceed
160 m.
●  RRU combination is not supported.
●  Before applying microwave equipment, you need to calculate the CPRI
payload and CPRI control word data volume based on the required RATs and
cell configuration, and convert the data volume into the data volume of
Ethernet frames to be transmitted to determine the theoretical minimum
transmission capability provided by microwave.
## 4.3.5 Cells
The TX/RX mode of the cell is 1T1R, 1T2R, 2T2R, or 2T4R.
## 4.3.6 Others
## None
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
For details about parameters related to cell setup, see
Cell Management in eRAN
feature documentation. Table 4-2 describes the parameters used for function
activation.
Table 4-2 Parameters used for activation
## Parameter Name
Parameter IDSetting Notes
Protocol TypeRRUCHAIN.PROTOCO
## L
Set this parameter to CPRI.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.16

Parameter NameParameter IDSetting Notes
CPRI Line RateRRUCHAIN.CRSet this parameter to 1.25 or
## 2.5.
CXU TypeCXU.CXUTYPESet this parameter to COE.
Local Cell IDCellTypeExt.LocalCell
## Id
The value of
CellTypeExt.LocalCellId must
be the same as that of
Cell.LocalCellId.
## Wireless Fronthaul
## Cell Flag
CellTypeExt.Wireless
FhCellFlag
Set this parameter to TRUE
for RuralLink cells.

4.4.1.2 Using MML Commands
Before using MML commands, refer to 4.2.2 Impacts and 4.3.2 Software and
complete the parameter configurations for related functions based on the impact
and mutually exclusive relationships between the functions, as well as the actual
network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Adding an RRU chain or ring
## ADD RRUCHAIN: RCN=1, TT=CHAIN, BM=COLD, AT=LOCALPORT, HSRN=0, HSN=3, HPN=1,
## PROTOCOL=CPRI, CR=1.25;
//Adding COE equipment
## ADD CXU: SRN=60, CXUTYPE=COE, PS=0, RCN=1;
## ADD CXU: SRN=61, CXUTYPE=COE, PS=1, RCN=1;
//Adding an RRU
ADD RRU: CN=0, SRN=62, SN=0, TP=TRUNK, RCN=1, PS=2, RT=MRRU, RS=LO, RXNUM=2, TXNUM=2,
## SCR=AUTO, MNTMODE=NORMAL;
//Adding a sector
ADD SECTOR: SECTORID=0, SECNAME="huawei", LOCATIONNAME="huawei", ANTNUM=2, ANT1CN=0,
## ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANT2CN=0, ANT2SRN=62, ANT2SN=0, ANT2N=R0B,
## CREATESECTOREQM=FALSE;
//Adding sector equipment
## ADD SECTOREQM: SECTOREQMID=0, SECTORID=0, ANTCFGMODE=ANTENNAPORT, ANTNUM=2,
ANT1CN=0, ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANTTYPE1=RXTX_MODE, ANT2CN=0, ANT2SRN=62,
## ANT2SN=0, ANT2N=R0B, ANTTYPE2=RXTX_MODE;
//Adding a cell
ADD CELL: LocalCellId=0, CellName="LTE", FreqBand=8, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=3600,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, CPRICompression=QUADPLEX_COMPRESSION, TxRxMode=2T2R;
//Adding operator information
ADD CELLOP: LocalCellId=0, TrackingAreaId=0;
//Enabling the RuralLink solution for the cell
MOD CELLTYPEEXT: LocalCellId=0, WirelessFhCellFlag=TRUE;
//Associating the cell sector equipment
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0;
//Activating the cell
ACT CELL: LocalCellId=0;
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.17

## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Deactivating the cell
DEA CELL: LocalCellId=0;
//Configuring the cell to use traditional optical transmission
MOD CELLTYPEEXT: LocalCellId=0, WirelessFhCellFlag=FALSE;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
-  Run the DSP CELL command to check the cell status.
If the Cell instance state parameter is Normal, the cell has been activated.
-  Verify cell activation.
Run the DSP CELLUECNT command. If the value of Cell Total Counter in the
command output is not 0, the UE accesses the cell successfully, indicating that
the cell works properly.
## 4.4.3 Network Monitoring
This solution solves only transmission problems and does not require independent
monitoring.
## 4.4.4 Possible Issues
●  During cell activation, the CellTypeExt.
WirelessFhCellFlag and
CXU.CXUTYPE parameters are checked. If the
CellTypeExt.
WirelessFhCellFlag parameter is set to FALSE but the
CXU.CXUTYPE parameter is set to COE, the cell fails to be activated and
ALM-29240 Cell Unavailable is reported with "Specific Problem" being "Invalid
parameter setting".
●  After the cell is successfully activated, the microwave equipment notifies the
COE of the actual rate capability. The COE then reports the actual rate
capability to the base station, which calculates the available bandwidth and
the bandwidth occupied by the activated carriers, and compares them. If the
bandwidth required by wireless fronthaul exceeds the microwave transmission
capability, the base station deactivates the cell or the cell capability degrades.
In addition, the base station reports ALM-29240 Cell Unavailable or
ALM-29243 Cell Capability Degraded with "Specific Problem" being
"Insufficient CPRI bandwidth".
●  Foolproof mechanism: After the cell is activated, if the value of the
CellTypeExt.
WirelessFhCellFlag parameter is changed from TRUE to FALSE,
a configuration error message is displayed, and the value TRUE takes effect
for the CellTypeExt.
WirelessFhCellFlag parameter.
SingleRAN
RuralLink Solution Guide4 RuralLink Solution (LTE)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.18

5 RuralLink Solution (UMTS)
## 5.1 Principles
The RuralLink solution uses the ADD CXU command to control whether to use
microwave for wireless fronthaul. When CXU.
CXUTYPE is set to COE, the UMTS
cell uses the RuralLink solution.
## 5.2 Network Analysis
## 5.2.1 Benefits
●  This solution is mainly used to address coverage problems in scenarios where
the optical fiber deployment distance or period is long, or optical fibers are
unreachable. The performance of microwave transmission varies greatly due
to the environment, weather, season, and blocking area.
●  Sites where the RuralLink solution is deployed use the BBUs of existing sites,
eliminating the need to install new BBUs and reducing costs.
## 5.2.2 Impacts
## Network Impacts
The base station reserves dedicated bandwidth for GSM. When a GSM cell is
added or removed, the UMTS cells will be reestablished. For details about the
dedicated bandwidth reserved for GSM, see 6.1 Principles.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.19

## Function Impacts
## Function
## Name
Function SwitchReference
## (RAN
## Feature
## Documentati
on)
## Description
MIMO PrimeULOCELL.VAMMIMO PrimeRuralLink cells do not
support VAM.
## Cell Digital
## Combination
and Split
## ULOCELL.LOCELLTYP
E set to DIST_CELL
Multiple RRUs
in One Cell
RuralLink cells must
be configured as
common cells.
## 0.5/0.5
## Configuration
## ULOCELL.LOCELLTYP
E set to
## HALFFREQ_CELL
Multiple RRUs
in One Cell
RuralLink cells must
be configured as
common cells.
## Independent
## Demodulation
of Signals
from Multiple
RRUs in One
## Cell
## ULOCELL.LOCELLTYP
E set to
## MULTIRRU_CELL
Multiple RRUs
in One Cell
RuralLink cells must
be configured as
common cells.
Cold backupSECTOREQM.TXBKP
## MODE1
## SECTOREQM.TXBKP
## MODE2
NoneFor RuralLink cells, it
is recommended that
the corresponding
sector equipment be
configured with one
transmit antenna and
the
## SECTOREQM.
## TXBKP
## MODE1
parameter
needs to be set to
## MASTER.
RF Connect
## Type
RRU.RFCONNTYPENoneThe
## RRU.RFCONNTYPE
parameter must be
set to NULL for
RuralLink cells.

## 5.3 Requirements
## 5.3.1 Licenses
There are no license requirements for basic functions.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.20

## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 5.3.3 Hardware
The hardware described in this section must support UMTS, and the configured
work modes must include UMTS.
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
5900 series base stations (macro base stations)
BBUs
Only the BBU5900 and BBU5900A support this function.
## Boards
●  Main control boards: Only the UMPTb, UMPTe, UMPTg, and UMPTga series
boards are supported.
●  Baseband processing units: Only the UBBPd, UBBPe, and UBBPg series boards
are supported.
RF Modules
Only 5000 series RRUs support this function.
## 5.3.4 Networking
●  Only the chain topology is supported. In each sector, only one RRU can be
connected to the COE, and a maximum of three RRUs can be cascaded.
●  The maximum air-interface distance between microwave equipment is 20 km.
●  The BBU/RRU/microwave equipment is connected to the COE through optical
fibers and the total length of the four-segment optical fibers cannot exceed
160 m.
●  RRU combination is not supported.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.21

●  Before applying microwave equipment, you need to calculate the CPRI
payload and CPRI control word data volume based on the required RATs and
cell configuration, and convert the data volume into the data volume of
Ethernet frames to be transmitted to determine the theoretical minimum
transmission capability provided by microwave.
## 5.3.5 Cells
The cells need to work in 1T2R mode. For details, see NodeB Carrier Management
in RAN Feature Documentation.
## 5.3.6 Others
## None
5.4 Operation and Maintenance
## 5.4.1 Data Configuration
## 5.4.1.1 Data Preparation
For details about parameters related to cell setup, see NodeB Carrier Management
in
RAN Feature Documentation. Table 5-1 describes the parameters used for
function activation.
Table 5-1 Parameters used for activation
## Parameter Name
Parameter IDSetting Notes
Protocol TypeRRUCHAIN.PROTOCO
## L
Set this parameter to CPRI.
CPRI Line RateRRUCHAIN.CRSet this parameter to 1.25 or
## 2.5.
CXU TypeCXU.CXUTYPESet this parameter to COE.
Local Cell TypeULOCELL.LOCELLTYP
## E
Set this parameter to
## NORMAL_CELL.

5.4.1.2 Using MML Commands
Before using MML commands, refer to 5.2.2 Impacts and complete the parameter
configurations for related functions based on the impact relationships between the
functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.22

## Activation Command Examples
●On the NodeB side
//Adding an RRU chain or ring
## ADD RRUCHAIN: RCN=1, TT=CHAIN, BM=COLD, AT=LOCALPORT, HSRN=0, HSN=3, HPN=1,
## PROTOCOL=CPRI, CR=1.25;
//Adding COE equipment
## ADD CXU: SRN=60, CXUTYPE=COE, PS=0, RCN=1;
## ADD CXU: SRN=61, CXUTYPE=COE, PS=1, RCN=1;
//Adding an RRU
ADD RRU: CN=0, SRN=62, SN=0, TP=TRUNK, RCN=1, PS=2, RT=MRRU, RS=UO, RXNUM=2, TXNUM=2,
## SCR=AUTO, MNTMODE=NORMAL;
//Adding a sector
ADD SECTOR: SECTORID=0, SECNAME="huawei", LOCATIONNAME="huawei", ANTNUM=2,
## ANT1CN=0, ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANT2CN=0, ANT2SRN=62, ANT2SN=0,
## ANT2N=R0B, CREATESECTOREQM=FALSE;
//Adding sector equipment
## ADD SECTOREQM: SECTOREQMID=0, SECTORID=0, ANTCFGMODE=ANTENNAPORT, ANTNUM=2,
## ANT1CN=0, ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANTTYPE1=RXTX_MODE, ANT2CN=0,
## ANT2SRN=62, ANT2SN=0, ANT2N=R0B, ANTTYPE2=RX_MODE;
//Adding a local cell
ADD ULOCELL: ULOCELLID=0, LOCELLTYPE=NORMAL_CELL, SECTOREQMNUM=1, SECTOREQMID1=0,
## TTW=FALSE, ULFREQ=9612, DLFREQ=10562, MAXPWR=430, HISPM=FALSE, RMTCM=FALSE,
## VAM=FALSE;
●On the RNC side
//Activating the logical cell
ACT UCELL: CellId=0;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
●On the RNC side
//Deactivating the cell
DEA UCELL: CellId=0;
●On the NodeB side
//Removing the local cell and performing reconfigurations based on live network conditions
## RMV ULOCELL: ULOCELLID=0;
5.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
Run the DSP ULOCELL command to check the cell status.
●  If the value of Local Cell Status is Local Cell Available, this function has
taken effect.
●  If the value of Cell Operation Status is Enabled, the logical cell has been
activated.
## 5.4.3 Network Monitoring
This solution solves only transmission problems and does not require independent
monitoring.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.23

## 5.4.4 Possible Issues
●  If a CXU is configured and CXU.CXUTYPE is set to COE, the local cell becomes
unavailable and ALM-28203 Local Cell Unusable is reported with "Specific
Problem" being "Incorrect cell networking" when a function in Function
Impacts is enabled for the local cell.
●  ALM-28203 Local Cell Unusable is reported with "Specific Problem" being
"Insufficient uplink CPRI bandwidth" or "Insufficient downlink CPRI
bandwidth" in any of the following scenarios:
–   The remaining CPRI bandwidth is insufficient to support UMTS cells.
–   Due to weather reasons, the microwave equipment decreases the
transmission bandwidth, which does not meet the bandwidth
requirements for activating cells on the remote RRU.
SingleRAN
RuralLink Solution Guide5 RuralLink Solution (UMTS)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.24

6 RuralLink Solution (GSM)
## 6.1 Principles
The RuralLink solution uses the ADD CXU command to control whether to use
microwave for wireless fronthaul. When CXU.
CXUTYPE is set to COE, the GSM cell
uses the RuralLink solution.
The base station reserves dedicated bandwidth for GSM in any of the following
scenarios:
●  The working mode of the RF unit (specified by the RRU.
RS parameter)
includes GSM.
●  A GSM cell is added to the base station (using the ADD GLOCELL command).
## 6.2 Network Analysis
## 6.2.1 Benefits
●  This solution is mainly used to address coverage problems in scenarios where
the optical fiber deployment distance or period is long, or optical fibers are
unreachable. The performance of microwave transmission varies greatly due
to the environment, weather, season, and blocking area.
●  Sites where the RuralLink solution is deployed use the BBUs of existing sites,
eliminating the need to install new BBUs and reducing costs.
## 6.2.2 Impacts
## Network Impacts
## None
SingleRAN
RuralLink Solution Guide6 RuralLink Solution (GSM)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.25

## Function Impacts
## Function
## Name
Function SwitchReference
## (GBSS
## Feature
## Documentati
on)
## Description
## Dynamic
power sharing
## GCELLCHMGAD.QTR
## UPWRSHARE
GSM Dynamic
## Power
## Sharing
It is not recommended
that inter-module
dual-PA power
sharing be configured
for RuralLink cells.
Multi-site CellGLOCELL.LOCELLTYP
## E
Multi-site CellIt is not recommended
that RuralLink cells
and multi-site cells be
configured at the
same time.

## 6.3 Requirements
## 6.3.1 Licenses
There are no license requirements for basic functions.
## 6.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 6.3.3 Hardware
The hardware described in this section must support GSM, and the configured
work modes must include GSM.
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
SingleRAN
RuralLink Solution Guide6 RuralLink Solution (GSM)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.26

## Base Station Models
5900 series base stations
BBUs
Only the BBU5900 and BBU5900A support this function.
## Boards
●  Main control boards: Only the UMPTb, UMPTe, UMPTg, and UMPTga series
boards are supported.
●  Baseband processing units: Only the UBBPd, UBBPe, and UBBPg series boards
are supported.
RF Modules
Only 5000 series RRUs support this function.
## 6.3.4 Networking
●  Only the chain topology is supported. In each sector, only one RRU can be
connected to the COE, and a maximum of three RRUs can be cascaded.
●  The maximum air-interface distance between microwave equipment is 20 km.
●  The BBU/RRU/microwave equipment is connected to the COE through optical
fibers and the total length of the four-segment optical fibers cannot exceed
160 m.
●  RRU combination is not supported.
●  Before applying microwave equipment, you need to calculate the CPRI
payload and CPRI control word data volume based on the required RATs and
cell configuration, and convert the data volume into the data volume of
Ethernet frames to be transmitted to determine the theoretical minimum
transmission capability provided by microwave.
## 6.3.5 Cells
Due to limited microwave bandwidth, CPRI links that use COE and microwave for
transmission support a maximum of 12 GSM 1T2R TRXs. If transmit diversity or 4-
way receive diversity is used, the TRX specifications will be halved.
## 6.3.6 Others
## None
6.4 Operation and Maintenance
## 6.4.1 Data Configuration
SingleRAN
RuralLink Solution Guide6 RuralLink Solution (GSM)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.27

## 6.4.1.1 Data Preparation
Table 6-1 describes the parameters used for function activation. The following
uses COE addition to CPRI link 0 as an example.
Table 6-1 Parameters used for activation
Parameter NameParameter IDSetting Notes
Protocol TypeRRUCHAIN.PROTOCO
## L
Set this parameter to CPRI.
CPRI Line RateRRUCHAIN.CRSet this parameter to 1.25 or
## 2.5.
CXU TypeCXU.CXUTYPESet this parameter to COE.

6.4.1.2 Using MML Commands
Before using MML commands, refer to 6.2.2 Impacts and complete the parameter
configurations for related functions based on the impact relationships between the
functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
●On the eGBTS side
//Adding an RRU chain or ring
## ADD RRUCHAIN: RCN=1, TT=CHAIN, BM=COLD, AT=LOCALPORT, HSRN=0, HSN=3, HPN=1,
## PROTOCOL=CPRI, CR=1.25;
//Adding COE equipment
## ADD CXU: SRN=60, CXUTYPE=COE, PS=0, RCN=1;
## ADD CXU: SRN=61, CXUTYPE=COE, PS=1, RCN=1;
//Adding an RRU
ADD RRU: CN=0, SRN=62, SN=0, TP=TRUNK, RCN=1, PS=2, RT=MRRU, RS=GO, RXNUM=2, TXNUM=2,
## SCR=AUTO, MNTMODE=NORMAL;
//Adding a sector
ADD SECTOR: SECTORID=0, SECNAME="huawei", LOCATIONNAME="huawei", ANTNUM=2,
## ANT1CN=0, ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANT2CN=0, ANT2SRN=62, ANT2SN=0,
## ANT2N=R0B, CREATESECTOREQM=FALSE;
//Adding sector equipment
## ADD SECTOREQM: SECTOREQMID=0, SECTORID=0, ANTCFGMODE=ANTENNAPORT, ANTNUM=2,
## ANT1CN=0, ANT1SRN=62, ANT1SN=0, ANT1N=R0A, ANTTYPE1=RXTX_MODE, ANT2CN=0,
## ANT2SRN=62, ANT2SN=0, ANT2N=R0B, ANTTYPE2=RX_MODE;
//Adding a cell
## ADD GLOCELL: GLOCELLID=0, BASEBANDPOLICY=EMBEDBBONLY, BASEBANDEQMID=255;
//Adding a TRX group
## ADD GTRXGROUP: GTRXGROUPID=0, GLOCELLID=0;
//Adding the binding relationship between the TRX group and sector equipment
## ADD GTRXGROUPSECTOREQM: GTRXGROUPID=0, SECTOREQMID=0;
●On the BSC side
//Activating the cell
## ACT GCELL: IDTYPE=BYID, CELLID=0;
SingleRAN
RuralLink Solution Guide6 RuralLink Solution (GSM)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.28

## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
●On the BSC side
//Deactivating the cell
## DEA GCELL: IDTYPE=BYID, CELLID=0;
●On the eGBTS side
//Removing the binding relationship between the TRX group and sector equipment
## RMV GTRXGROUPSECTOREQM: GTRXGROUPID=0, SECTOREQMID=0;
//Removing the TRX group
## RMV GTRXGROUP: GTRXGROUPID=0;
//Removing the cell
## RMV GLOCELL: GLOCELLID=0;
6.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 6.4.2 Activation Verification
-  Run the DSP GLOCELL command to check the cell status.
If the value of Local Cell Status is Available, the cell has been activated.
-  Verify cell activation.
Use an MS to make a call in the test cell. If the call is normal, this function
works properly.
## 6.4.3 Network Monitoring
This solution solves only transmission problems and does not require independent
monitoring.
## 6.4.4 Possible Issues
After the cell is activated, if the number of GSM TRXs exceeds the RuralLink link
specifications, the GSM cell capability degrades. In addition, ALM-28017 GSM
Local Cell Capability Decline is reported with "Specific Problem" being "Insufficient
CPRI bandwidth".
SingleRAN
RuralLink Solution Guide6 RuralLink Solution (GSM)
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.29

## 7 Parameters
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
SingleRAN
RuralLink Solution Guide7 Parameters
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.30

## 8 Counters
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
SingleRAN
RuralLink Solution Guide8 Counters
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.31

## 9 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
SingleRAN
RuralLink Solution Guide9 Glossary
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.32

## 10 Reference Documents
1.Relay
2.High Speed Mobility
3.Cell Management
## 4.SFN
5.Flexible Bandwidth based on Overlap Carriers (FDD)
6.Seamless Intra-Band Carrier Joining (FDD)
7.Virtual 4T4R (FDD)
8.Network Assisted Interference Cancellation
9.TDM eICIC (FDD)
10.UL CoMP
11.Video Experience Optimization
12.DL CoMP (FDD)
13.Interference Detection and Suppression
14.Carrier Aggregation
15.NB-IoT Basics (FDD)
16.Short TTI (FDD)
17.CPRI Compression
18.MIMO Prime
19.Multiple RRUs in One Cell
20.NodeB Carrier Management
21.GSM Dynamic Power Sharing
22.Multi-site Cell
SingleRAN
RuralLink Solution Guide10 Reference Documents
Issue 03 (2023-12-22)Copyright © Huawei Technologies Co., Ltd.33