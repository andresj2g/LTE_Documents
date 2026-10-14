

eRAN
Short TTI (FDD) Feature Parameter
## Description
## Issue04
## Date2023-09-14
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
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 04 (2023-09-14)..................................................................................................................................................1
1.2 eRAN18.1 03 (2023-04-23)..................................................................................................................................................1
1.3 eRAN18.1 02 (2023-02-01)..................................................................................................................................................2
1.4 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.5 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 2
2 About This Document.............................................................................................................3
2.1 General Statements................................................................................................................................................................ 3
2.2 Applicable RAT......................................................................................................................................................................... 4
2.3 Features in This Document.................................................................................................................................................. 4
3 Overview....................................................................................................................................5
4 Short TTI....................................................................................................................................6
4.1 Principles.................................................................................................................................................................................... 6
4.2 Network Analysis.................................................................................................................................................................. 10
4.2.1 Benefits................................................................................................................................................................................. 10
4.2.2 Impacts..................................................................................................................................................................................10
4.3 Requirements......................................................................................................................................................................... 15
4.3.1 Licenses................................................................................................................................................................................. 15
4.3.2 Software................................................................................................................................................................................15
4.3.3 Hardware..............................................................................................................................................................................20
4.3.4 Others....................................................................................................................................................................................20
4.4 Operation and Maintenance.............................................................................................................................................21
4.4.1 Data Configuration........................................................................................................................................................... 21
4.4.1.1 Data Preparation............................................................................................................................................................ 21
4.4.1.2 Using MML Commands............................................................................................................................................... 23
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 24
4.4.2 Activation Verification......................................................................................................................................................24
4.4.3 Network Monitoring.........................................................................................................................................................24
5 Parameters..............................................................................................................................25
6 Counters.................................................................................................................................. 26
7 Glossary................................................................................................................................... 27
eRAN
Short TTI (FDD) Feature Parameter DescriptionContents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iii

8 Reference Documents...........................................................................................................28
eRAN
Short TTI (FDD) Feature Parameter DescriptionContents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 04 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
●  Removed the reference document for GSM and LTE Zero Bufferzone from
4.3.2 Software because the document
GSM and LTE Zero Bufferzone is
deleted from the documentation.
●  Removed the reference document for GSM and LTE FDD Dynamic Spectrum
Sharing from 4.3.2 Software because the document
GSM and LTE FDD
## Dynamic Spectrum Sharing
is deleted from the documentation.
●  Revised descriptions in this document.
1.2 eRAN18.1 03 (2023-04-23)
This issue includes the following changes.
eRAN
Short TTI (FDD) Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.1

## Technical Changes
Change DescriptionParameter ChangeBase Station Model
Added a mutually
exclusive relationship
between short TTI and
the RuralLink solution.
For details, see 4.3.2
## Software.
None5900 series base
stations (macro
base stations)

## Editorial Changes
Revised descriptions in this document.
1.3 eRAN18.1 02 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.5 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 01 (2021-03-05).
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
Short TTI (FDD) Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.2

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
## Trial Features
Trial features are features that are not yet ready for full commercial release for
certain reasons. For example, the industry chain (terminals/CN) may not be
sufficiently compatible. However, these features can still be used for testing
purposes or commercial network trials. Anyone who desires to use the trial
eRAN
Short TTI (FDD) Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.3

features shall contact Huawei and enter into a memorandum of understanding
(MoU) with Huawei prior to an official application of such trial features. Trial
features are not for sale in the current version but customers may try them for
free.
Customers acknowledge and undertake that trial features may have a certain
degree of risk due to absence of commercial testing. Before using them, customers
shall fully understand not only the expected benefits of such trial features but also
the possible impact they may exert on the network. In addition, customers
acknowledge and undertake that since trial features are free, Huawei is not liable
for any trial feature malfunctions or any losses incurred by using the trial features.
Huawei does not promise that problems with trial features will be resolved in the
current version. Huawei reserves the rights to convert trial features into
commercial features in later R/C versions. If trial features are converted into
commercial features in a later version, customers shall pay a licensing fee to
obtain the relevant licenses prior to using the said commercial features. If a
customer fails to purchase such a license, the trial feature(s) will be invalidated
automatically when the product is upgraded.
2.2 Applicable RAT
This document applies to FDD.
2.3 Features in This Document
This document describes the following FDD features.
Feature ID
Feature NameChapter/Section
LNOFD-150301Short TTI (Trial)4 Short TTI
eRAN
Short TTI (FDD) Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.4

## 3 Overview
LTE networks have evolved, and millisecond-level end-to-end (E2E) service latency
is now possible. New services, such as ultra-reliable low-latency communication
(URLLC) services, require a lower latency. To meet the latency requirements of
these services, short transmission time interval (TTI) has been introduced as a key
technology to guarantee a low latency on LTE networks.
eRAN
Short TTI (FDD) Feature Parameter Description3 Overview
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.5

4 Short TTI
## 4.1 Principles
In a conventional LTE system, 1 ms subframes are transmitted over the air
interface. When normal cyclic prefixes (CPs) are used, each subframe contains 14
orthogonal frequency division multiplexing (OFDM) symbols. With short TTI, a 1-
ms subframe can be subdivided into shorter TTI lengths. A short TTI can contain
just two or three symbols. This decreases the latency over the air interface and the
total E2E latency. There are two structures (as shown in Figure 4-1 and Figure
4-2) for downlink short TTI subframes and one structure (as shown in Figure 4-3)
for uplink short TTI subframes.
Figure 4-1 Downlink short TTI subframe structure 1
Figure 4-2 Downlink short TTI subframe structure 2
Figure 4-3 Uplink short TTI subframe structure
In the preceding structures, os stands for an OFDM symbol, and sTTI stands for a
short TTI. A normal 1-ms TTI is also called an nTTI.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.6

Which downlink subframe structure is used depends on the index of the start
symbol of the first Short PDSCH (sPDSCH). Table 4-1 lists which structure is used
for each index.
Table 4-1 Index of the start symbol of the first sPDSCH and the corresponding
downlink subframe structure
Index of the Start SymbolDownlink Short TTI Subframe
## Structure
1 or 3Structure 1
2Structure 2

Workflow of Short TTI
Short TTI enables OFDM-symbol-level data transmission. New physical channels
are introduced, including Short PDCCH (sPDCCH), Short PUCCH (sPUCCH),
sPDSCH, and Short PUSCH (sPUSCH). The eNodeB supports mixed scheduling of
UEs in short TTI and normal TTI modes. The scheduled UEs can also dynamically
switch between short TTI and normal TTI modes. Figure 4-4 shows the procedure
for short TTI scheduling.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.7

Figure 4-4 Procedure for short TTI scheduling
-  The eNodeB checks whether the short TTI switch (controlled by the
SHORT_TTI_SW option of the CellShortTtiAlgo.
SttiAlgoSwitch parameter) is
turned on.
a.  If it is turned on, the eNodeB proceeds with 2.
b.  If it is not turned on, the eNodeB schedules the UE in normal TTI mode.
-  The eNodeB determines whether the UE to be scheduled supports short TTI.
a.  If it supports short TTI, the eNodeB proceeds with 3. For details about the
requirements for UE capabilities, see 4.3.4 Others.
b.  If it does not support short TTI, the eNodeB schedules the UE in normal
TTI mode.
-  The eNodeB checks whether the UE meets the conditions for entering the
short TTI scheduling.
a.  If all of the following conditions are met, the eNodeB proceeds with 4:
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.8

▪The uplink signal to interference plus noise ratio (SINR) of the UE is
higher than the value of the CellShortTtiAlgo.SttiEntryUlSinrThld
parameter.
▪A bearer with a QCI whose CellQciPara.LowLatencyFlag parameter
is TRUE has been set up for the UE.
▪The uplink resource block (RB) usage of the cell that serves the UE
does not exceed the value of the
CellShortTtiAlgo.SttiEntryUlRbUsageThld parameter.
▪The downlink RB usage of the cell that serves the UE does not
exceed the value of the CellShortTtiAlgo.SttiEntryDlRbUsageThld
parameter.
b.  If any of the preceding conditions is not met, the eNodeB schedules the
UE in normal TTI mode.
-  The eNodeB schedules the UE in short TTI mode.
RBs Available for Short TTI
The number of RBs available for short TTI can be dynamically adjusted or
statically configured, depending on the setting of the
CellShortTtiAlgo.
NttiSttiRbAdjStrategy parameter.
●  If this parameter is set to DYNAMIC, the maximum number of RBs available
for short TTI is dynamically adjusted by the eNodeB.
●  If this parameter is set to STATIC:
–   For uplink scheduling, the number of uplink short resource block groups
(sRBGs) reserved for UEs scheduled in short TTI mode is specified by the
CellShortTtiAlgo.
UlSrbgCntReservedForStti parameter. These reserved
resources cannot be used for uplink scheduling for UEs in normal TTI
mode. No additional resources can be used for uplink scheduling for UEs
in short TTI mode.
–   For downlink scheduling, the number of downlink sRBGs reserved for UEs
scheduled in short TTI mode is specified by the
CellShortTtiAlgo.
DlSrbgCntReservedForStti parameter. These reserved
resources cannot be used for downlink scheduling for UEs in normal TTI
mode. No additional resources can be used for downlink scheduling for
UEs in short TTI mode.
Preallocation in Short TTI Mode
Preallocation can be performed for UEs scheduled in short TTI mode. Uplink
preallocation for UEs scheduled in short TTI mode is enabled when the
SHORT_TTI_PREALLOCATION_SW option of the
CellShortTtiAlgo.
SttiAlgoSwitch parameter is selected and the
CellShortTtiAlgo.
SttiPreallocationDuration parameter is set to a value greater
than 0. In this case:
●  The preallocation interval is specified by the
CellShortTtiAlgo.
SttiPreallocationMinPeriod parameter.
●  The duration of each preallocation is specified by the
CellShortTtiAlgo.
SttiPreallocationDuration parameter.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.9

●  The size of data in each preallocation is specified by the
CellShortTtiAlgo.SttiPreallocationSize parameter.
sPDCCH Resource Configuration
The resources occupied by the sPDCCH depend on the value of the
CellShortTtiAlgo.
SpdcchRbCnt parameter. A larger parameter value indicates
more resources and a higher maximum aggregation level available to the sPDCCH
and a larger coverage of the sPDCCH. No sPDCCH resources are available for
subframe 0 in short TTI mode. In subframe 0, control channel elements (CCEs)
must be reserved for the PDCCH. The upper limit of the reserved CCEs is specified
by the CellShortTtiAlgo.
PdcchCceCntReservedForStti parameter.
sPDCCH Boundary Power Control
The sPDCCH boundary power control function can be enabled to ensure the
coverage of the sPDCCH. This function is controlled by the
SPDCCH_BOUNDARY_POWER_CTRL_SW option of the
CellShortTtiAlgo.
SttiAlgoSwitch parameter. If this option is selected, power can
be increased (assuming there is sufficient power available) to hold the sPDCCH
block error rate under control when the maximum aggregation level is in use.
## 4.2 Network Analysis
## 4.2.1 Benefits
UEs performing small-packet services (such as online gaming or web browsing)
enjoy a lower air interface latency and accordingly a lower E2E latency in short TTI
mode than in normal TTI mode.
## 4.2.2 Impacts
## Network Impacts
Short TTI has the following impacts on the network:
●  The Cell Uplink Average Throughput may decrease slightly. This is because
scheduling of short TTI subframes increases the header overhead of transport
blocks, uplink demodulation reference signal (DMRS) overhead, and symbol-
level interference to neighboring cells.
●  The Cell Downlink Average Throughput may decrease slightly. This is
because short TTI increases the header overhead of transport blocks, and the
sPDCCH occupies a large number of downlink resources.
●  The downlink peak throughput of the short TTI UEs decreases. This is because
a low code rate is selected during transport block size (TBS) index selection in
short TTI mode.
## Function Impacts
●  Basic functions
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.10

## Function
## Name
Function SwitchReferenceDescription
## Uplink
frequency
selective
scheduling
UlEnhancedFssS
witch option of
the
CellAlgoSwitch.
UlSchSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
uplink frequency
selective scheduling.
## Downlink
frequency
selective
scheduling
FreqSelSwitch
option of the
CellAlgoSwitch.
DlSchSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
downlink frequency
selective scheduling.
PAMCUlPAMCSwitch
option of the
CellAlgoSwitch.
UlSchExtSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
## PAMC.
TBS index
rise for
downlink
## HARQ
retransmissio
ns
PreciseMcsAdap
tSwitch option
of the
CellAlgoSwitch.
CqiAdjAlgoSwit
ch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
TBS index rise for
downlink HARQ
retransmissions.
## Downlink
non-GBR
packet
bundling
NonGbrBundlin
gSwitch option
of the
CellAlgoSwitch.
DlSchSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
downlink non-GBR
packet bundling.
Uplink target
## IBLER
adaptation
UlIblerAdjustSw
itch option of
the
CellAlgoSwitch.
UlSchSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
uplink target IBLER
adaptation.
## Optimized
scheduling
upon full
uplink power
UlSchRbAllocOp
tSw option of
the
CellAlgoSwitch.
UlSchExtSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
optimized scheduling
upon full uplink power.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.11

## Function
## Name
Function SwitchReferenceDescription
UL Multi-
## Cluster
UlMultiClusterS
witch option of
the
CellAlgoSwitch.
UlSchExtSwitch
parameter
SchedulingUEs scheduled in short
TTI mode do not support
UL Multi-Cluster.
Uplink short-
interval SPS
CellUlschAlgo.In
tvlOfUlSpsWith
## Skipping
SchedulingUEs scheduled in short
TTI mode do not support
uplink short-interval SPS.
## CQI
adjustment
CqiAdjAlgoSwit
ch option of the
CellAlgoSwitch.
CqiAdjAlgoSwit
ch parameter
## Channel
## State
## Management
UEs scheduled in short
TTI mode use a unique
set of CQI adjustment
values different from
those used for UEs
scheduled in normal TTI
mode.
## Optimized
## CQI
adjustment
value
PreciseMcsAdap
tSwitch option
of the
CellAlgoSwitch.
CqiAdjAlgoSwit
ch
parameter
## Channel
## State
## Management
UEs scheduled in short
TTI mode do not support
CQI adjustment value
optimization.
## PDCCH
## Power
## Control
## Enhancemen
t
CellPdcchAlgo.P
dcchPowerEnha
ncedSwitch
## Physical
## Channel
## Resource
## Management
UEs scheduled in short
TTI mode do not support
PDCCH power control
enhancement.
DL 256QAMCellAlgoSwitch.
Dl256QamAlgoS
witch
## Modulation
## Schemes
UEs scheduled in short
TTI mode do not support
## DL 256QAM.
## UL 256QAMUL_256QAM_S
WITCH option of
the
PUSCHCfg.Ul25
6QamAlgoSwitc
h
parameter
## Modulation
## Schemes
UEs scheduled in short
TTI mode do not support
## UL 256QAM.

●  Other related functions
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.12

## Function
## Name
Function SwitchReferenceDescription
CA cellNoneCarrier
## Aggregation
If the SHORT_TTI_SW
option of the
CellShortTtiAlgo.SttiAlg
oSwitch parameter is
selected, CA will not be
performed for UEs
capable of short TTI.
Support of
VoLTE
ENodeBAlgoSwi
tch.EutranVoipS
upportSwitch
VoLTEThe eNodeB does not
schedule a UE in short
TTI mode if a voice
bearer has been set up
for this UE. If a voice
bearer is set up during
short TTI scheduling, the
eNodeB immediately
stops short TTI
scheduling for this UE.
UL CoMP cellUlJointReceptio
nSwitch option
of the
CellAlgoSwitch.
UplinkCompSwi
tch
parameter
UL CoMPUEs scheduled in short
TTI mode do not support
UL CoMP.
DL CoMP cellFDDHomNetDlC
ompSwitch and
FDDHetNetDlCo
mpSwitch
options of the
CellAlgoSwitch.
DlCompSwitch
parameter
DL CoMP
## (FDD)
UEs scheduled in short
TTI mode do not support
DL CoMP.
Video TTI
bundling
TtiBundlingForV
ideoSwitch
option of the
CellAlgoSwitch.
UlSchSwitch
parameter
## Video
## Experience
## Optimization
Video TTI bundling does
not take effect for UEs
scheduled in short TTI
mode.
Uplink SU-
## MIMO
ULSUMIMO2Lay
ersSwitch option
of the
CellAlgoSwitch.
UlSuMimoAlgoS
witch
parameter
MIMOUEs scheduled in short
TTI mode do not support
uplink SU-MIMO.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.13

## Function
## Name
Function SwitchReferenceDescription
DRXCellDrxPara.Drx
AlgSwitch
DRX and
## Signaling
## Control
UEs scheduled in short
TTI mode do not support
discontinuous reception
## (DRX).
Support for
## PTT
NonePTTThe eNodeB does not
schedule a UE in short
TTI mode if a push-to-
talk (PTT) bearer has
been set up for this UE.
If a PTT bearer is set up
during short TTI
scheduling, the eNodeB
immediately stops short
TTI scheduling for this
## UE.
## SRLTE
optimization
CellSrlte.SrlteS
witch
## SRLTE
## Optimization
UEs scheduled in short
TTI mode do not support
SRLTE optimization.
## TA
enhancemen
t
TimeAlignment
Timer.TaEnhanc
e
## Uplink
## Timing
## Control
## (FDD)
UEs scheduled in short
TTI mode do not support
TA enhancement.
Inter-eNodeB
uplink
interference
cancellation
UlInterSiteIcSwi
tch option of the
CellAlgoSwitch.
UplinkIcSwitch
parameter
## Uplink
## Interference
## Cancellation
## (FDD)
UEs scheduled in short
TTI mode do not support
inter-eNodeB uplink
interference cancellation.
## Turbo
receiver
CellAlgoSwitch.
TurboReceiverS
witch
## Turbo
## Receiver
UEs scheduled in short
TTI mode do not support
the turbo receiver.
## Superior
uplink
coverage
CellAlgoExtSwit
ch.UlCoverageE
nhancementSw
## Superior
## Uplink
## Coverage
## (FDD)
Short TTI scheduling
cannot be performed for
UEs under coverage
enhancement.
## TDMTDM_SWITCH
option of the
NsaDcMgmtConf
ig.NsaDcAlgoSw
itch
parameter
## NSA
## Networking
based on
## EPC
Short TTI and TDM
cannot take effect
simultaneously. When
one of the functions is in
effect, the other does
not take effect.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.14

## Function
## Name
Function SwitchReferenceDescription
## Breathing
## Pilot
BreathingPilotS-
witch option of
the
CellDlschAlgo.Br
eathingPilotAlg
oSwitch
parameter
## Breathing
## Pilot
UEs scheduled in short
TTI mode do not support
## Breathing Pilot.
TM9TM9Switch
option of the
CellAlgoSwitch.
EnhMIMOSwitc
h parameter
eMIMO
## (FDD)
UEs scheduled in short
TTI mode do not support
## TM9.

## 4.3 Requirements
## 4.3.1 Licenses
There are no license requirements for trial functions. For details, see 2.1 General
## Statements.
## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
●  Basic functions
## Function
## Name
Function SwitchReference
## UL CRAUL_COORD_RES_ALLOC_SWITC
H option of the
UlCsAlgoPara.UlCsSw
parameter
## Uplink Coordinated
## Scheduling
UL CPCUL_COORD_PC_SWITCH option
of the UlCsAlgoPara.UlCsSw
parameter
## Uplink Coordinated
## Scheduling
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.15

## Function
## Name
Function SwitchReference
ePDCCHCellPdcchAlgo.EpdcchAlgoSwit
ch
## Physical Channel
## Resource Management
Extended CPCell.UlCyclicPrefix and
Cell.DlCyclicPrefix
Extended CP

●  Functions related to interference suppression
## Function
## Name
Function SwitchReference
## Advanced
## Receiver
## (PSIC)
MumimoPuschPsicSwitch
option of the
CellAlgoSwitch.PsicSwitch
parameter
PSIC Receiver
SFN cellCell.MultiRruCellModeSFN
## Dynamic
TDM eICIC
CellAlgoSwitch.EicicSwitch
parameter with the value of
## DYNAMIC
TDM eICIC (FDD)
## Downlink
interference
randomizatio
n
CellAlgoSwitch.InterfRandSwit
ch parameter with the value of
## ENB_BASED
## ICIC
## High-order
UL CoMP in
4R cells
## UL_HIGH_ORDER_COMP_FOR_
4R_SW option of the
CellUlCompAlgo.UlCompAlgoS
witch parameter
UL CoMP

●  Functions related to MIMO
## Function
## Name
Function SwitchReference
Uplink MU-
## MIMO
UlVmimoSwitch option of the
CellAlgoSwitch.UlSchSwitch
parameter
## MIMO
Virtual 4T4RVirtual4T4RSwitch option of
the
CellAlgoSwitch.EmimoSwitch
parameter
Virtual 4T4R (FDD)
## 3D
beamformin
g
eUCellSectorEqm.CellBeamMo
de parameter with the value of
MASSIVE_MIMO_Ph1 or
MASSIVE_MIMO_Ph2
3D Beamforming (FDD)
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.16

## Function
## Name
Function SwitchReference
## Massive
## MIMO
introduction
eUCellSectorEqm.CellBeamMo
de parameter with the value of
MASSIVE_MIMO_Ph1 or
MASSIVE_MIMO_Ph2
Massive MIMO (FDD)
## Static
## Multiple
## Beam
NoneSmart 8T8R (FDD)
## Dynamic
## Massive
## Beam
NoneSmart 8T8R (FDD)

●  Functions related to CloudAIR
## Function
## Name
Function SwitchReference
UMTS and
## LTE
## Spectrum
## Sharing
SpectrumCloud.SpectrumCloud
Switch parameter with the
value of
## UL_SPECTRUM_SHARING
UMTS and LTE Spectrum
## Sharing
GSM and LTE
## Spectrum
## Concurrency
SpectrumCloud.SpectrumCloud
Switch parameter with the
value of
## GL_SPECTRUM_CONCURRENCY
GSM and LTE Spectrum
## Concurrency
LTE FDD and
NR Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.SpectrumCloud
Switch parameter with the
value of
## LTE_NR_SPECTRUM_SHR
LTE FDD and NR
## Spectrum Sharing
LTE FDD and
NR Uplink
## Spectrum
## Sharing
SpectrumCloud.SpectrumCloud
Switch parameter with the
value of
## LTE_NR_UPLINK_SPECTRUM_S
## HR
LTE FDD and NR Uplink
## Spectrum Sharing
Hybrid DSS
Based on
## Asymmetric
## Bandwidth
SpectrumCloud.SpectrumCloud
Switch parameter set to
LTE_NR_SPECTRUM_SHR, and
## LNR_SPECTRUM_SHR_ASYM_S
W option of the
SpectrumCloud.
SpectrumCloud
EnhSwitch parameter selected
LTE FDD and NR
## Spectrum Sharing

●  Functions related to power control
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.17

## Function
## Name
Function SwitchReference
CSPCCspcAlgoPara.CspcAlgoSwitchCSPC
eCSPCCellCspcPara.CelleCspcSwitchCSPC
Intra-eNodeB
## CSPC
CellCspcPara.IntraEnbCspcSwCSPC

●  Functions related to mobility management
## Function
## Name
Function SwitchReference
High speed
mobility
Cell.HighSpeedFlagHigh Speed Mobility
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh Speed Mobility

●  Functions related to coverage improvement
## Function
## Name
Function SwitchReference
Cell radius
greater than
15 km
NoneExtended Cell Range
Cell radius
greater than
100 km
NoneExtended Cell Range

●  Other related functions
## Function
## Name
Function SwitchReference
eMTC
introduction
EMTC_SWITCH option of the
CellEmtcAlgo.EmtcAlgoSwitch
parameter
eMTC
NB-IoT
network
deployment
NoneNB-IoT Basics (FDD)
## Single-carrier
power
sharing for
## 4T
## SINGLE_CA_PWR_SHARE_SW_F
OR_4T option of the
PDSCHCfg.TxChnPowerCfgSw
parameter
## None
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.18

## Function
## Name
Function SwitchReference
In-band relayInBandRelayDeNbSwitch and
InBandRelayReNbSwitch
options of the
CellAlgoSwitch.RelaySwitch
parameter
## Relay
## Uplink
frequency
hopping
CellUlschAlgo.UlHoppingTypeNone
## Compact
bandwidth
Cell.CustomizedBandWidthCf-
gInd
## Compact Bandwidth
## (FDD)
GSM and LTE
## FDD
## Dynamic
## Spectrum
## Sharing
GLDynSpectrumShareSwitch
option of the
CellAlgoSwitch.DynSpectrumS
hareSwitch parameter
## None
GSM and LTE
## Zero
## Bufferzone
GLZeroBufferZoneSwitch
option of the
CellAlgoSwitch.DynSpectrumS
hareSwitch parameter
## None
RF channel
dynamic
muting
## RF_CHN_DYN_MUTING_SW
option of the
CellRfChnDynMut-
ing.RfChnDynMutingAlgoS-
witch
parameter
Energy Conservation and
## Emission Reduction
CRS dynamic
muting
## CRS_DYNAMIC_MUTING_SW
option of the
SymbolPwrSaving.SymbolShut
downEnhancedSw parameter
Energy Conservation and
## Emission Reduction
## Dynamic
carrier
shutdown
## CARRIER_DYN_SHUTDOWN_S
W option of the
CellShutdown.CarrierShutdow
nEnhancedSw parameter
Energy Conservation and
## Emission Reduction
TM4 and
## TM6
## Adaptation
## CL_TM_ADAPTATION_OPT_SW
option of the
CellMimoParaCfg.MimoSwitch
parameter
Low-Band Booster
RuralLink
solution
CellTypeExt.WirelessFhCellFlagRuralLink Solution

eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.19

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
3900 and 5900 series base stations (macro base stations)
## Boards
The baseband processing unit must be a UBBPe in any of the following models:
●  UBBPe1
●  UBBPe2
●  UBBPe3
●  UBBPe4
●  UBBPe5
●  UBBPe6
## NO TE
If short TTI is enabled for an LTE FDD cell established on a BBP, non-FDD cells cannot be
set up on this BBP.
The main control board must be a UMPT.
RF Modules
The RF modules must support a TX/RX capability of no higher than 4T4R.
## Cells
●  The cell bandwidth must be at least 10 MHz.
●  The TX/RX mode of the cell must be 2T2R, 2T4R, or 4T4R.
## 4.3.4 Others
UEs must support short TTI. The requirements for reported UE capabilities are as
follows:
●  The IE "STTI-SupportedCombinations-r15.combination-22-r15" for the
corresponding band is {1,1}. This indicates that the UE supports single-carrier
short TTI.
●  The IE "min-Proc-TimelineSubslot-r15" is {set1,set1,set1}.
●  The IE "ue-CategoryUL" is not UL Category M1, UL Category M2, UL Category
0, or UL Category 1bis.
●  The IE "ue-CategoryDL" is not DL Category M1, DL Category M2, DL Category
0, or DL Category 1bis.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.20

4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Table 4-2 and Table 4-3 describe the parameters used for function activation and
optimization, respectively.
Table 4-2 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
Short TTI
## Algorithm
## Switch
CellShortTtiAlgo.S
ttiAlgoSwitch
## SHORT_TTI_S
## W
You are advised to
select this option.

Table 4-3 Parameters used for optimization
## Parameter
## Name
Parameter IDOptionSetting Notes
Short TTI
## Algorithm
## Switch
CellShortTtiAlgo.S
ttiAlgoSwitch
## SHORT_TTI_PR
## EALLOCATION
## _SW
Select this option
when preallocation for
short TTI is required.
Short TTI
## Algorithm
## Switch
CellShortTtiAlgo.S
ttiAlgoSwitch
## SPDCCH_BOU
## NDARY_POWE
## R_CTRL_SW
Select this option
when sPDCCH
boundary power
control is required.
DL Scheduling
## Extension Switch
CellAlgoSwitch.Dl
SchExtSwitch
## PUSCH_1X_SW
## ITCH
Select this option
when the short TTI
function is enabled.
Normal TTI and
Short TTI RB
## Adjustment
## Strategy
CellShortTtiAlgo.
NttiSttiRbAdjStrat
egy
NoneSet this parameter to
its recommended
value.
Short TTI Entry
UL RB Usage
## Threshold
CellShortTtiAlgo.S
ttiEntryUlRbUsa-
geThld
NoneSet this parameter to
its recommended
value.
Short TTI Entry
DL RB Usage
## Threshold
CellShortTtiAlgo.S
ttiEntryDlRbUsa-
geThld
NoneSet this parameter to
its recommended
value.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.21

## Parameter
## Name
Parameter IDOptionSetting Notes
Short TTI Entry
## UL SINR
## Threshold
CellShortTtiAlgo.S
ttiEntryUlSinrThld
NoneSet this parameter to
its recommended
value.
Short TTI Entry
DCCH Quality
## Hysteresis
CellShortTtiAlgo.S
ttiEntryDcchQua-
lityHyst
NoneSet this parameter to
its recommended
value.
Short TTI
## Preallocation
## Minimum Period
CellShortTtiAlgo.S
ttiPreallocation-
MinPeriod
NoneSet this parameter to
its recommended
value.
Short TTI
## Preallocation
## Duration
CellShortTtiAlgo.S
ttiPreallocation-
## Duration
NoneSet this parameter to
its recommended
value.
Short TTI
## Preallocation
## Size
CellShortTtiAlgo.S
ttiPreallocation-
## Size
NoneSet this parameter to
its recommended
value.
Short TTI UL
## HARQ
## Maximum
## Transmission
## Count
CellShortTtiAlgo.S
ttiUlHarqMaxTxC
nt
NoneSet this parameter to
its recommended
value.
Short TTI DL
## HARQ
## Maximum
## Transmission
## Count
CellShortTtiAlgo.S
ttiDlHarqMaxTxC
nt
NoneSet this parameter to
its recommended
value.
Short TTI SRI
## Period
CellShortTtiAlgo.S
ttiSriPeriod
NoneSet this parameter to
its recommended
value.
DeltaF for
SPUCCH Format
1 and 1a
CellShortTtiAlgo.S
pucchFormat1And
1aDeltaF
NoneSet this parameter to
its recommended
value.
DeltaF for
SPUCCH Format
## 1b
CellShortTtiAlgo.S
pucchFormat1bDe
ltaF
NoneSet this parameter to
its recommended
value.
DL SRBG Count
Reserved for
Short TTI
CellShortTtiAlgo.
DlSrbgCntReserve
dForStti
NoneSet this parameter to
its recommended
value.
UL SRBG Count
Reserved for
Short TTI
CellShortTtiAlgo.
UlSrbgCntReserve
dForStti
NoneSet this parameter to
its recommended
value.
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.22

## Parameter
## Name
Parameter IDOptionSetting Notes
## PDCCH CCE
## Count Reserved
for Short TTI
CellShortTtiAlgo.P
dcchCceCntReser-
vedForStti
NoneSet this parameter to
its recommended
value.
## SPUCCH RB
## Count
CellShortTtiAlgo.S
pucchRbCnt
NoneSet this parameter to
its recommended
value.
## SPDCCH RB
## Count
CellShortTtiAlgo.S
pdcchRbCnt
NoneSet this parameter to
its recommended
value.
## Low Latency
## Flag
CellQciPara.LowL
atencyFlag
NoneSet this parameter
based on the network
plan.
Short TTI RLC
## Parameter
Group ID
QciPara.ShortTtiR
lcParamGroupId
NoneSet this parameter to
its recommended
value.

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
//Enabling short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, SttiAlgoSwitch=SHORT_TTI_SW-1;
## Optimization Command Examples
//Setting aperiodic CQI reporting for short TTI
MOD CELLALGOSWITCH: LocalCellId=0, DlSchExtSwitch=PUSCH_1X_SWITCH-1;
//Setting the QCI for the cell with short TTI enabled
MOD CELLQCIPARA: LocalCellId=0, Qci=3, LowLatencyFlag=TRUE;
//Setting the policy of RB adjustment in the normal and short TTI modes
MOD CELLSHORTTTIALGO: LocalCellId=0, NttiSttiRbAdjStrategy=DYNAMIC;
//Setting the conditions for entering the short TTI mode
MOD CELLSHORTTTIALGO: LocalCellId=0, SttiEntryUlSinrThld=5, SttiEntryDlRbUsageThld=50,
SttiEntryUlRbUsageThld=50, SttiEntryDcchQualityHyst=0;
//Setting the numbers of uplink and downlink sRBGs reserved for short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, DlSrbgCntReservedForStti=1, UlSrbgCntReservedForStti=1;
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.23

//Setting preallocation parameters for short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0,
SttiAlgoSwitch=SHORT_TTI_PREALLOCATION_SW-1,SttiPreallocationMinPeriod=5,
SttiPreallocationDuration=20, SttiPreallocationSize=80;
//Setting the maximum numbers of uplink and downlink HARQ retransmissions for short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, SttiUlHarqMaxTxCnt=N10, SttiDlHarqMaxTxCnt=N10;
//Setting the sPUCCH parameters for short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, SpucchRbCnt=1, SttiSriPeriod=MS1,
SpucchFormat1And1aDeltaF=DB_5;
//Setting the sPDCCH parameters for short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, SttiAlgoSwitch=SPDCCH_BOUNDARY_POWER_CTRL_SW-1,
PdcchCceCntReservedForStti=16, SpdcchRbCnt=RB_16;
//Setting the short TTI RLC parameter group ID to 167 for QCI 3
MOD QCIPARA: Qci=3, ShortTtiRlcParamGroupId=167;
## Deactivation Command Examples
//Disabling short TTI
MOD CELLSHORTTTIALGO: LocalCellId=0, SttiAlgoSwitch=SHORT_TTI_SW-0;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
## None
## 4.4.3 Network Monitoring
## None
eRAN
Short TTI (FDD) Feature Parameter Description4 Short TTI
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.24

## 5 Parameters
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
Short TTI (FDD) Feature Parameter Description5 Parameters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.25

## 6 Counters
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
Short TTI (FDD) Feature Parameter Description6 Counters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.26

## 7 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
Short TTI (FDD) Feature Parameter Description7 Glossary
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.27

## 8 Reference Documents
1.Scheduling
2.Channel State Management
3.Physical Channel Resource Management
4.Breathing Pilot
5.Modulation Schemes
6.eMIMO (FDD)
7.Carrier Aggregation
8.VoLTE
9.UL CoMP
10.DL CoMP (FDD)
11.Video Experience Optimization
## 12.MIMO
13.DRX and Signaling Control
## 14.PTT
15.SRLTE Optimization
16.Uplink Timing Control (FDD)
17.Uplink Interference Cancellation (FDD)
18.Turbo Receiver
19.Uplink Coordinated Scheduling
## 20.CSPC
21.Extended CP
22.PSIC Receiver
## 23.SFN
24.Extended Cell Range
25.Virtual 4T4R (FDD)
26.3D Beamforming (FDD)
27.Massive MIMO (FDD)
28.Compact Bandwidth (FDD)
eRAN
Short TTI (FDD) Feature Parameter Description8 Reference Documents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.28

29.UMTS and LTE Spectrum Sharing
30.GSM and LTE Spectrum Concurrency
31.TDM eICIC (FDD)
32.High Speed Mobility
33.eMTC
34.NB-IoT Basics (FDD)
## 35.ICIC
36.Relay
37.NSA Networking based on EPC
38.Superior Uplink Coverage (FDD)
39.LTE FDD and NR Spectrum Sharing
40.Smart 8T8R (FDD)
41.Energy Conservation and Emission Reduction
42.Low-Band Booster
43.LTE FDD and NR Uplink Spectrum Sharing
44.RuralLink Solution
eRAN
Short TTI (FDD) Feature Parameter Description8 Reference Documents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.29