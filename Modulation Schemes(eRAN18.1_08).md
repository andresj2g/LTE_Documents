

eRAN
## Modulation Schemes Feature
## Parameter Description
## Issue08
## Date2024-06-21
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
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 08 (2024-06-21)..................................................................................................................................................1
1.2 eRAN18.1 07 (2023-12-22)..................................................................................................................................................1
1.3 eRAN18.1 06 (2023-09-14)..................................................................................................................................................2
1.4 eRAN18.1 05 (2023-04-23)..................................................................................................................................................2
1.5 eRAN18.1 04 (2023-02-01)..................................................................................................................................................3
1.6 eRAN18.1 03 (2022-10-25)..................................................................................................................................................3
1.7 eRAN18.1 02 (2022-08-25)..................................................................................................................................................3
1.8 eRAN18.1 01 (2022-03-08)..................................................................................................................................................3
1.9 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 4
2 About This Document.............................................................................................................6
2.1 General Statements................................................................................................................................................................ 6
2.2 Applicable RAT......................................................................................................................................................................... 6
2.3 Features in This Document.................................................................................................................................................. 7
3 Overview....................................................................................................................................8
3.1 Background................................................................................................................................................................................8
3.2 Basic Concepts..........................................................................................................................................................................9
4 Basic Modulation Functions................................................................................................12
4.1 Principles.................................................................................................................................................................................. 12
4.2 Network Analysis.................................................................................................................................................................. 12
4.2.1 Benefits................................................................................................................................................................................. 12
4.2.2 Impacts..................................................................................................................................................................................13
4.3 Requirements......................................................................................................................................................................... 13
4.3.1 Licenses................................................................................................................................................................................. 13
4.3.2 Software................................................................................................................................................................................13
4.3.3 Hardware..............................................................................................................................................................................13
4.3.4 Cells........................................................................................................................................................................................ 14
4.3.5 Others....................................................................................................................................................................................14
4.4 Operation and Maintenance.............................................................................................................................................14
4.4.1 Data Configuration........................................................................................................................................................... 14
4.4.1.1 Data Preparation............................................................................................................................................................ 14
4.4.1.2 Using MML Commands............................................................................................................................................... 14
eRAN
Modulation Schemes Feature Parameter DescriptionContents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iii

4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 15
4.4.2 Activation Verification......................................................................................................................................................15
4.4.3 Network Monitoring.........................................................................................................................................................15
5 Enhanced Modulation Functions.......................................................................................16
5.1 UL 64QAM...............................................................................................................................................................................16
5.1.1 Principles.............................................................................................................................................................................. 16
5.1.2 Network Analysis...............................................................................................................................................................16
5.1.2.1 Benefits.............................................................................................................................................................................. 16
5.1.2.2 Impacts.............................................................................................................................................................................. 17
5.1.3 Requirements...................................................................................................................................................................... 18
5.1.3.1 Licenses..............................................................................................................................................................................18
5.1.3.2 Software............................................................................................................................................................................ 18
5.1.3.3 Hardware.......................................................................................................................................................................... 18
5.1.3.4 Others................................................................................................................................................................................ 19
5.1.4 Operation and Maintenance......................................................................................................................................... 19
5.1.4.1 Data Configuration........................................................................................................................................................19
5.1.4.1.1 Data Preparation.........................................................................................................................................................19
5.1.4.1.2 Using MML Commands............................................................................................................................................19
5.1.4.1.3 Using the MAE-Deployment................................................................................................................................... 20
5.1.4.2 Activation Verification.................................................................................................................................................. 20
5.1.4.3 Network Monitoring..................................................................................................................................................... 20
5.2 UL 256QAM............................................................................................................................................................................ 20
5.2.1 Principles.............................................................................................................................................................................. 20
5.2.2 Network Analysis...............................................................................................................................................................23
5.2.2.1 Benefits.............................................................................................................................................................................. 23
5.2.2.2 Impacts.............................................................................................................................................................................. 24
5.2.3 Requirements...................................................................................................................................................................... 26
5.2.3.1 Licenses..............................................................................................................................................................................26
5.2.3.2 Software............................................................................................................................................................................ 26
5.2.3.3 Hardware.......................................................................................................................................................................... 27
5.2.3.4 Cells.....................................................................................................................................................................................27
5.2.3.5 Others................................................................................................................................................................................ 27
5.2.4 Operation and Maintenance......................................................................................................................................... 27
5.2.4.1 Data Configuration........................................................................................................................................................27
5.2.4.1.1 Data Preparation.........................................................................................................................................................27
5.2.4.1.2 Using MML Commands............................................................................................................................................28
5.2.4.1.3 Using the MAE-Deployment................................................................................................................................... 29
5.2.4.2 Activation Verification.................................................................................................................................................. 29
5.2.4.3 Network Monitoring..................................................................................................................................................... 30
5.3 DL 256QAM............................................................................................................................................................................ 30
5.3.1 Principles.............................................................................................................................................................................. 30
5.3.2 Network Analysis...............................................................................................................................................................33
eRAN
Modulation Schemes Feature Parameter DescriptionContents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iv

5.3.2.1 Benefits.............................................................................................................................................................................. 33
5.3.2.2 Impacts.............................................................................................................................................................................. 34
5.3.3 Requirements...................................................................................................................................................................... 37
5.3.3.1 Licenses..............................................................................................................................................................................37
5.3.3.2 Software............................................................................................................................................................................ 37
5.3.3.3 Hardware.......................................................................................................................................................................... 37
5.3.3.4 Cells.....................................................................................................................................................................................38
5.3.3.5 Others................................................................................................................................................................................ 38
5.3.4 Operation and Maintenance......................................................................................................................................... 39
5.3.4.1 Data Configuration........................................................................................................................................................39
5.3.4.1.1 Data Preparation.........................................................................................................................................................39
5.3.4.1.2 Using MML Commands............................................................................................................................................40
5.3.4.1.3 MAE-Deployment (FDD)..........................................................................................................................................40
5.3.4.2 Activation Verification.................................................................................................................................................. 41
5.3.4.3 Network Monitoring..................................................................................................................................................... 43
6 Parameters..............................................................................................................................44
7 Counters.................................................................................................................................. 45
8 Glossary................................................................................................................................... 46
9 Reference Documents...........................................................................................................47
eRAN
Modulation Schemes Feature Parameter DescriptionContents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.v

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 08 (2024-06-21)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Added descriptions of the impacts of the eNodeB always selecting the MCS table
with 256QAM for UEs. For details, see 5.2.1 Principles.
Added descriptions of the impacts of the eNodeB always selecting the CQI table
with 256QAM for UEs. For details, see 5.3.1 Principles.
1.2 eRAN18.1 07 (2023-12-22)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Modified the activation verification method for UL 256QAM. For details, see
## 5.2.4.2 Activation Verification.
eRAN
## Modulation Schemes Feature Parameter Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.1

Revised descriptions in this document.
1.3 eRAN18.1 06 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
●  Added descriptions of the impact relationship between UL 256QAM and
Support of VoLTE. For details, see 5.2.2.2 Impacts.
●  Revised the impact analysis of UL 256QAM. For details, see 5.2.2.2 Impacts.
●  Revised the impact analysis of DL 256QAM. For details, see 5.3.2.2 Impacts.
●  Revised descriptions in this document.
1.4 eRAN18.1 05 (2023-04-23)
This issue includes the following changes.
## Technical Changes
## Change Description
## Parameter
## Change
RATBase Station
## Model
Added RB resource
allocation optimization for
UL 256QAM when the CSS
is used. For details, see:
## ●5.2.1 Principles
## ●5.2.2 Network
## Analysis
## ●5.2.4.1.1 Data
## Preparation
●5.2.4.1.2 Using MML
## Commands
Activated the
reserved
parameter:
BIT13 of the
eNBCellRsvdPara.
RsvdSwPara8
parameter
FDD● 3900 and
5900 series
base
stations
## (macro
base
stations)
## ● DBS3900
LampSite
and
## DBS5900
LampSite

## Editorial Changes
Revised descriptions in this document.
Added the descriptions of the impact relationships of DL 256QAM with energy
saving based on flexible frequency-domain scheduling and RF channel dynamic
muting in TM9. For details, see 5.3.2.2 Impacts.
eRAN
## Modulation Schemes Feature Parameter Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.2

1.5 eRAN18.1 04 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.6 eRAN18.1 03 (2022-10-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.7 eRAN18.1 02 (2022-08-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.8 eRAN18.1 01 (2022-03-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
## Modulation Schemes Feature Parameter Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.3

1.9 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 05 (2021-11-27).
## Technical Changes
Change DescriptionParameter ChangeRATBase Station Model
Added support for UL
256QAM. For details,
see 5.2 UL 256QAM.
Added parameters:
●UeCompat.Ul256Q
amUeConfigIndex
●Ul256QamUePara.
Ul256QamUeConfi
gIndex
●Ul256QamUePara.
Ul256QamCssMcs
## Tab
●Ul256QamUePara.
Ul256QamEstdPo
wReductValue
Changed the
applicable RATs of the
following parameters:
## ●UL_256QAM_SWIT
CH option of the
PUSCHCfg.
Ul256Q
amAlgoSwitch
parameter
●PUSCHCfg.
Ul256Q
amMcsTblCfgStrat
egy
●PUSCHCfg.Ul256Q
amMcsTblAdpPeri
od
## FDD
● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
Added the impact
relationship between
DL 256QAM and
flexible TM4 MU-
MIMO. For details, see
## 5.3.2.2 Impacts.
NoneFDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E
eRAN
## Modulation Schemes Feature Parameter Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.4

Change DescriptionParameter ChangeRATBase Station Model
Added the impact
relationship between
DL 256QAM and
downlink intelligent
joint adaptive
modulation and
coding (JAMC). For
details, see 5.3.2.2
## Impacts.
NoneFDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E

## Editorial Changes
Revised descriptions in this document.
eRAN
## Modulation Schemes Feature Parameter Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.5

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
## Modulation Schemes Feature Parameter Description2 About This Document
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.6

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-001005Modulation: DL/UL
## QPSK, DL/UL
## 16QAM, DL 64QAM
## 4 Basic Modulation Functions
## LOFD-001006UL 64QAM5.1 UL 64QAM
## LEOFD-110301DL 256QAM5.3 DL 256QAM
## LEOFD-180301UL 256QAM5.2 UL 256QAM
eRAN
## Modulation Schemes Feature Parameter Description2 About This Document
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.7

## 3 Overview
## 3.1 Background
In digital communications systems, modulation is the process of varying the
amplitude, frequency, or phase of a carrier signal with a digital baseband signal to
convey information using the carrier signal, as shown in Figure 3-1.
## Figure 3-1 Modulation
To clearly compare different modulation schemes, this document defines the
efficiency of modulation schemes using the number of bits that can be carried on
each orthogonal frequency division multiplexing (OFDM) symbol. A more efficient
modulation scheme modulates more bits of information into each carrier signal.
Table 3-1 lists the typical modulation schemes used in Long Term Evolution (LTE).
eRAN
## Modulation Schemes Feature Parameter Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.8

Table 3-1 Typical modulation schemes
## Modulation
## Scheme
Bits of
Information (N)
## Efficiency
## (log
## 2
## N)
## Carrier Signal
## Change Item
QPSK42Phase
16QAM164Amplitude and
phase
64QAM646Amplitude and
phase
256QAM2568Amplitude and
phase

Huawei eNodeBs support basic and enhanced modulation schemes based on live
network applications.
●  Basic modulation schemes are commonly used and take effect by default in
LTE. For details, see 4 Basic Modulation Functions.
–   Uplink (UL) and downlink (DL) quadrature phase shift keying (QPSK)
–   UL and DL 16 quadrature amplitude modulation (16QAM)
## –   DL 64QAM
●  Enhanced modulation schemes in LTE are used to help increase UL or DL
transmission efficiency for UEs with good channel quality, thereby meeting
service rate requirements. For details, see 5 Enhanced Modulation Functions.
## –   UL 64QAM
–   UL and DL 256QAM
A more efficient modulation scheme has higher requirements on channel quality
to ensure that the signal to interference plus noise ratio (SINR) is high enough at
the receive end for correct demodulation.
## 3.2 Basic Concepts
This section describes the basic concepts and conventions involved in this
document.
## CQI
CQI is short for channel quality indicator. In the DL, data is terminated in UEs
instead of eNodeBs. Therefore, eNodeBs cannot measure the DL SINR for
evaluating DL channel quality. UEs report CQIs to eNodeBs to indicate the DL
channel quality of services from the eNodeBs. The eNodeBs then determine which
modulation and coding scheme (MCS) to use based on these CQIs. CQIs are
indexed from 0 to 15. The larger the CQI index, the better the channel quality.
eRAN
## Modulation Schemes Feature Parameter Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.9

CQI Table
A CQI table maps CQI indexes to modulation schemes. For details, see section
7.2.3 "Channel Quality Indicator (CQI) definition" in 3GPP TS 36.213 V16.5.0. In
this section:
●Table 7.2.3-1: 4-bit CQI Table provides the CQI table without 256QAM.
●Table 7.2.3-2: 4-bit CQI Table 2 provides the CQI table with 256QAM.
## MCS
MCS is short for modulation and coding scheme. eNodeBs use different MCSs to
ensure transmission quality and efficiency of UE services. If the channel quality is
good, an eNodeB selects an MCS with a more efficient modulation scheme and a
higher code rate. If the channel quality is poor, the eNodeB selects one with a less
efficient modulation scheme and a lower code rate (by inserting more redundant
bits).
MCS Table
An MCS table maps MCS indexes to combinations of modulation orders
(indicating modulation schemes) and transport block size (TBS) indexes. For UL
and DL MCS tables, see sections 8.6.1 "Modulation order and redundancy version
determination" and 7.1.7.1 "Modulation order and redundancy version
determination", respectively, in 3GPP TS 36.213 V16.5.0. In these sections:
## ●  UL
–Table 8.6.1-1: Modulation, TBS index and redundancy version table
for PUSCH provides the MCS table without UL 256QAM.
–Table 8.6.1-3: Modulation, TBS index and redundancy version table
for PUSCH provides the MCS table with UL 256QAM.
## ●  DL
–Table 7.1.7.1-1: Modulation and TBS index table for PDSCH provides
the MCS table without DL 256QAM.
–Table 7.1.7.1-1A: Modulation and TBS index table 2 for PDSCH
provides the MCS table with DL 256QAM.
TBS Index
A TBS index determines the size of a single transport block given a specific
number of physical resource blocks (PRBs). The better the channel conditions, the
larger the TBS index that can be selected by the eNodeB for a UE, and the higher
the peak UE throughput. For details about how to select TBSs for the UL and DL,
see sections 8.6.2 "Transport block size determination" and 7.1.7.2.1 "Transport
blocks not mapped to two or more layer spatial multiplexing", respectively, in
## 3GPP TS 36.213 V16.5.0.
According to 3GPP specifications, TBS indexes for the DL are optimized as follows:
●  New TBS indexes are now available for UEs for which transmission mode 9
(TM9) or transmission mode 10 (TM10) is used. The highest TBS indexes for
TM9/TM10-capable UEs used to be 25 and 32 in cells with certain bandwidth
and cell-specific reference signal (CRS) port configurations. This is because
eRAN
## Modulation Schemes Feature Parameter Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.10

fewer resource elements (REs) can be used for data transmission due to RE
consumption by channel state information-reference signals (CSI-RSs) and
demodulation reference signals (DMRSs). For this scenario, 3GPP Release 12
has defined TBS indexes 26A and 33A. These two indexes are used for TM9/
TM10-capable UEs at the cell center, increasing the DL peak throughput of
these UEs.
–   TBS index 26A is added to the MCS table without DL 256QAM.
–   TBS index 33A is added to the MCS table with DL 256QAM.
●  3GPP Release 14 has defined TBS index 33B, which is added to the MCS table
with DL 256QAM. This new index is used for TM1/TM2/TM3/TM4/TM6/TM7-
capable UEs at the cell center, increasing the DL peak throughput of these
UEs.
eRAN
## Modulation Schemes Feature Parameter Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.11

## 4 Basic Modulation Functions
## 4.1 Principles
Basic modulation functions include:
●  UL and DL QPSK, UL and DL 16QAM, and DL 64QAM
These basic modulation schemes are not under switch control. The eNodeB
selects an appropriate UL or DL modulation scheme for each UE based on the
UL or DL channel quality of the UE during scheduling. For details about these
modulation schemes, see sections 5.3.2 "Modulation" and 6.3.2 "Modulation"
in 3GPP TS 36.211 V16.5.0.
●  DL TBS index optimization with index 26A introduced
Assume that only a small number of TBS indexes can be selected for TM9/
TM10-capable UEs and these UEs meet channel condition requirements.
When this function is enabled, the eNodeB sends RRC messages to inform
these UEs that the TBS of index 26A can be used, and also uses this TBS for
DL data transmission. This function is controlled by the
MIMO_TBSIZE_OPT_SWITCH option of the CellAlgoSwitch.
DlSchExtSwitch
parameter. For details about scenarios where only a small number of TBS
indexes can be selected for TM9/TM10-capable UEs, see TBS Index.
## 4.2 Network Analysis
## 4.2.1 Benefits
These functions offer the following benefits:
●  UL and DL QPSK, UL and DL 16QAM, and DL 64QAM
The base station selects an appropriate UL or DL modulation scheme for each
UE based on the UL or DL channel quality of the UE to ensure that the UE
can obtain optimal service experience that matches the channel quality.
●  DL TBS index optimization with index 26A introduced
This function increases the DL peak throughput of TM9/TM10-capable UEs at
the cell center by 2%–5%.
eRAN
## Modulation Schemes Feature Parameter Description4 Basic Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.12

## 4.2.2 Impacts
## Network Impacts
## None
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDeMTC
introduction
## EMTC_SWITCH
option of the
CellEmtcAlgo.E
mtcAlgoSwitch
parameter
eMTCAs defined in 3GPP TS
36.321, eMTC UEs and
CE UEs support only
QPSK and 16QAM.

## 4.3 Requirements
## 4.3.1 Licenses
There are no license requirements for basic functions.
## 4.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
●  UL and DL QPSK, UL and DL 16QAM, and DL 64QAM: no requirements
●  DL TBS index optimization with index 26A introduced: Only 3900 and 5900
series base stations (macro base stations) are compatible with this function.
## Boards
No requirements
eRAN
## Modulation Schemes Feature Parameter Description4 Basic Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.13

RF Modules
No requirements
## 4.3.4 Cells
●  UL and DL QPSK, UL and DL 16QAM, and DL 64QAM: no requirements
●  DL TBS index optimization with index 26A introduced: This function is
supported only in cells with a 10 MHz, 15 MHz, or 20 MHz bandwidth.
## 4.3.5 Others
●  UL and DL QPSK, UL and DL 16QAM, and DL 64QAM: no requirements
●  DL TBS index optimization with index 26A introduced: UEs must comply with
3GPP Release 12 or later. That is, the value of alternativeTBS-Indices-r12 in
the UE capability message must be supported.
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
UL and DL QPSK, UL and DL 16QAM, and DL 64QAM take effect by default and
do not require data configuration. Table 4-1 describes the parameters used for
activating DL TBS index optimization with index 26A introduced.
Table 4-1 Parameters used for activation
## RA
## T
## Parameter
## Name
Parameter IDOptionSetting Notes
## FD
## D
DL Scheduling
## Extension
## Switch
CellAlgoSwitc
h.DlSchExtSwi
tch
## MIMO_TBSIZE_
## OPT_SWITCH
It is recommended
that this option be
selected when only a
small number of TBS
indexes can be
selected for TM9/
TM10-capable UEs.

4.4.1.2 Using MML Commands
Before using MML commands, refer to 4.2.2 Impacts and complete the parameter
configurations for related functions based on the impact relationships between the
functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
eRAN
## Modulation Schemes Feature Parameter Description4 Basic Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.14

Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//UL and DL QPSK, UL and DL 16QAM, and DL 64QAM do not require activation.
//(Optional) Enabling DL TBS index optimization with index 26A introduced when a small number of TBS
indexes can be selected for TM9/TM10-capable UEs
MOD CELLALGOSWITCH: LocalCellId=0, DlSchExtSwitch=MIMO_TBSIZE_OPT_SWITCH-1;
## Deactivation Command Examples
//UL and DL QPSK, UL and DL 16QAM, and DL 64QAM do not require deactivation.
//Disabling DL TBS index optimization with index 26A introduced
MOD CELLALGOSWITCH: LocalCellId=0, DlSchExtSwitch=MIMO_TBSIZE_OPT_SWITCH-0;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
UL and DL QPSK, UL and DL 16QAM, and DL 64QAM
These basic functions ensure basic service performance. They take effect by
default and do not require activation verification.
DL TBS Index Optimization with Index 26A Introduced
Perform the following steps to check whether TBS index optimization with 26A
introduced has taken effect, by tracing air interface signaling on the MAE-Access.
Step 1On the MAE-Access, start a Uu interface tracing task by choosing Monitor >
Signaling Trace > Signaling Trace Management > LTE > Application Layer > Uu
## Interface Trace.
Step 2Check the RRC_CONN_RECFG message in the Uu interface tracing result. If the
PDSCH-Config IE in the message contains the PDSCH-ConfigDedicated-v1280 field
whose value is a26, DL TBS index optimization with index 26A introduced has
taken effect.
----End
## 4.4.3 Network Monitoring
This function ensures basic service performance. Separate monitoring is not
required.
eRAN
## Modulation Schemes Feature Parameter Description4 Basic Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.15

## 5 Enhanced Modulation Functions
## 5.1 UL 64QAM
## 5.1.1 Principles
UL 64QAM is an enhanced UL modulation scheme. For details, see section 5.3.2
"Modulation" in 3GPP TS 36.211 V16.5.0. This function is enabled if the
PUSCHCfg.
Qam64Enabled parameter is set to BOOLEAN_TRUE. With this
function, the eNodeB enables UL 64QAM-capable UEs whose UL channel quality is
favorable to use this modulation scheme.
Assume that UL 64QAM is enabled. If the PUSCHCfg.R12Qam64Enabled
parameter is set to BOOLEAN_TRUE, the eNodeB is allowed to solve compatibility
issues of certain UEs that comply with 3GPP Release 12 or later. For details, see
section 6.3.2 ''Radio resource control information elements'' in 3GPP TS 36.331
V16.4.0. If the PUSCHCfg.R12Qam64Enabled parameter is set to
BOOLEAN_FALSE, the proportion of times UL 64QAM is selected for UEs is
extremely low in the case that there are a large number of UEs that comply with
3GPP Release 12 or later. In addition, UE compatibility issues cause the values of
related performance indicators to deteriorate. For example, the initial block error
rate (IBLER) and residual block error rate (RBLER) increase.
## 5.1.2 Network Analysis
## 5.1.2.1 Benefits
UL 64QAM is recommended when the channel quality is favorable, for example,
when the proportion of times MCS index 24 is selected for scheduling on the
PUSCH (indicated by L.ChMeas.PUSCH.MCS.24) is more than 5% within 24 hours.
In this case, this function provides the following benefits:
●  The UL spectral efficiency for UEs at the cell center or at a medium distance
from the cell center increases, thereby increasing the average UL user-
perceived throughput for these UEs by up to 39%.
●  The UL peak cell throughput increases by up to 39%.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.16

When the channel quality is poor, UL 64QAM cannot be selected for most UEs in
the cell. In this case, UL 64QAM cannot achieve the optimal gains, but will not
bring extra negative impacts.
## NO TE
Average UL user-perceived throughput = L.Thrp.bits.UE.UL.Experienced/
L.Thrp.Time.UE.UL.Experienced
## 5.1.2.2 Impacts
## Network Impacts
After UL 64QAM is enabled, interference to neighboring cells slightly increases.
The higher the proportion of times UL 64QAM takes effect for cell-center UEs, the
higher the interference to neighboring cells, and the lower the Cell Uplink
Average Throughput of the neighboring cells.
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDeMTC
introduction
## EMTC_SWITCH
option of the
CellEmtcAlgo.E
mtcAlgoSwitch
parameter
eMTCAs defined in 3GPP TS
36.321, eMTC UEs and
CE UEs do not support
uplink 64QAM.
FDDUMTS and
## LTE
## Spectrum
## Sharing
SpectrumClou
d.SpectrumClo
udSwitch set
to
## UL_SPECTRUM
## _SHARING
UMTS and
LTE Spectrum
## Sharing
With UMTS and LTE
Spectrum Sharing, the
LTE system is exposed
to interference from
the UMTS system. The
interference may
cause decreases in the
proportion of times
UL 64QAM is selected
and also in the gains
provided by UL
## 64QAM.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.17

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDGSM and
## LTE
## Spectrum
## Concurrency
SpectrumClou
d.SpectrumClo
udSwitch set
to
## GL_SPECTRUM
## _CONCURREN
## CY
GSM and LTE
## Spectrum
## Concurrency
With GSM and LTE
## Spectrum
Concurrency, the LTE
system is exposed to
interference from the
GSM system. The
interference may
cause decreases in the
proportion of times
UL 64QAM is selected
and also in the gains
provided by UL
## 64QAM.

## 5.1.3 Requirements
## 5.1.3.1 Licenses
## RAT
Feature IDFeature
## Name
ModelSales Unit
FDDLOFD-001006UL 64QAMLT1SU64QAM00per cell

## 5.1.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 5.1.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
For FDD, the following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.18

●  DBS3900 LampSite and DBS5900 LampSite
## ●  BTS3912E
## ●  BTS3911E
## ●  BTS3203E
## Boards
No requirements
RF Modules
No requirements
## 5.1.3.4 Others
UEs must support UL 64QAM. A UE supports UL 64QAM if the value of
ul-64QAM-r12 in the UE capability message is supported.
5.1.4 Operation and Maintenance
## 5.1.4.1 Data Configuration
## 5.1.4.1.1 Data Preparation
Table 5-1 describes the parameters used for function activation.
Table 5-1 Parameters used for activation
## RAT
## Parameter
## Name
Parameter IDSetting Notes
FDDQam64
enabled
PUSCHCfg.Q
am64Enabled
To enable UL 64QAM in a cell,
set this parameter to
## BOOLEAN_TRUE.
## FDDR12 UL
## 64QAM
## Enabled
PUSCHCfg.R1
2Qam64Enab
led
Set the
PUSCHCfg.R12Qam64Enable
d parameter to
BOOLEAN_TRUE if the
PUSCHCfg.Qam64Enabled
parameter is set to
## BOOLEAN_TRUE.

5.1.4.1.2 Using MML Commands
Before using MML commands, refer to 5.1.2.2 Impacts and complete the
parameter configurations for related functions based on the impact relationships
between the functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.19

Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Enabling UL 64QAM
MOD PUSCHCFG: LocalCellId=0, Qam64Enabled=BOOLEAN_TRUE;
//Enabling compatibility resolution for UEs that comply with 3GPP Release 12 or later
MOD PUSCHCFG: LocalCellId=0, R12Qam64Enabled=BOOLEAN_TRUE;
## Deactivation Command Examples
//Disabling compatibility resolution for UEs that comply with 3GPP Release 12 or later
MOD PUSCHCFG: LocalCellId=0, R12Qam64Enabled=BOOLEAN_FALSE;
//Disabling UL 64QAM
MOD PUSCHCFG: LocalCellId=0, Qam64Enabled=BOOLEAN_FALSE;
5.1.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.1.4.2 Activation Verification
Monitor the L.Traffic.UL.SCH.64QAM.TB counter. If this counter produces a non-
zero value, UL 64QAM has taken effect.
## 5.1.4.3 Network Monitoring
Compare the average UL user-perceived throughputs before and after UL 64QAM
is enabled to monitor the function benefits.
## 5.2 UL 256QAM
## 5.2.1 Principles
For the procedure for UL 256QAM to take effect, see UL 256QAM. For the MCS
table selection policy, see MCS Table Selection Policy.
## UL 256QAM
Figure 5-1 shows the procedure for UL 256QAM to take effect.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.20

Figure 5-1 UL 256QAM-related procedure
-  The eNodeB checks whether the UL_256QAM_SWITCH option of the
PUSCHCfg.
Ul256QamAlgoSwitch parameter is selected.
–   If this option is selected, the eNodeB goes to 2.
–   If this option is deselected, the procedure ends. The eNodeB selects QPSK,
16QAM, or 64QAM for UEs based on channel quality.
-  The eNodeB checks whether a UE meets the requirements for UL 256QAM
described in 5.2.3.5 Others.
–   If the UE meets the requirements, the eNodeB goes to 3.
–   If the UE does not meet the requirements, the procedure ends. The
eNodeB selects QPSK, 16QAM, or 64QAM for the UE based on channel
quality.
-  The eNodeB checks whether fixed MCS table selection is enabled. For details
about the MCS table selection policy, see MCS Table Selection Policy.
–   If the PUSCHCfg.Ul256QamMcsTblCfgStrategy parameter is set to
FIXED_CONFIGURATION, the eNodeB always selects the MCS table with
UL 256QAM for UEs.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.21

–   If the PUSCHCfg.Ul256QamMcsTblCfgStrategy parameter is set to
ADAPTIVE_CONFIGURATION, the eNodeB selects an appropriate MCS
table based on channel quality at an interval specified by the
PUSCHCfg.Ul256QamMcsTblAdpPeriod parameter.
▪The shorter the interval, the better the selected MCS table matches
channel quality changes, and the higher the UL rates. However, RRC
connection reconfiguration messages are sent more frequently,
increasing the probability of service drops.
▪The longer the interval, the worse the selected MCS table matches
channel quality changes, and the lower the UL rates. However, RRC
connection reconfiguration messages are sent less frequently,
reducing the probability of service drops.
-  The eNodeB performs uplink scheduling by selecting an appropriate
modulation scheme for the UE based on channel quality and the selected
MCS table.
In FDD, the PUSCHCfg.
EstdPowerReductValue256Qam parameter specifies
the estimated power reduction value used in MCS index selection for UEs
supporting UL 256QAM. This function reduces the impact of power reduction
of UEs on the uplink user-perceived rate.
–   A smaller value of this parameter results in a higher probability that UL
256QAM takes effect for UEs and a higher BLER when UL 256QAM takes
effect.
–   A larger value of this parameter results in a lower probability that UL
256QAM takes effect for UEs and a lower BLER when UL 256QAM takes
effect.
In FDD, power reduction estimation is supported by whitelisted UEs
supporting UL 256QAM. The configuration index for whitelisted UEs is
specified by the Ul256QamUePara.
Ul256QamUeConfigIndex parameter, and
the estimated power reduction for whitelisted UEs supporting UL 256QAM is
specified by the Ul256QamUePara.
Ul256QamEstdPowReductValue
parameter. This function takes effect when the
UeCompat.Ul256QamUeConfigIndex parameter value is consistent with the
Ul256QamUePara.Ul256QamUeConfigIndex parameter value for whitelisted
UEs. For details about whitelisted UEs, see
## Terminal Awareness
## Differentiation.
In FDD, RB resource allocation can be optimized for UL 256QAM when the
common search space (CSS) is used. This function is controlled by BIT13 of
the reserved parameter eNBCellRsvdPara.
RsvdSwPara8. For details about
this reserved parameter, see 6 Parameters. When this function is enabled,
PUSCH RB allocation is optimized for UL 256QAM-capable UEs when they are
using the CSS.
MCS Table Selection Policy
3GPP defines two MCS tables based on whether 256QAM is included. For details,
see MCS Table.
During UL scheduling, the eNodeB selects an appropriate MCS table based on the
PUSCHCfg.
Ul256QamMcsTblCfgStrategy parameter setting. Table 5-2 describes
the MCS table selection policy.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.22

Table 5-2 MCS table selection policy
Value of
PUSCHCfg.Ul256QamMcsTblCfgStrat
egy
MCS Table Selection Policy
## ADAPTIVE_CONFIGURATION
a
The eNodeB adaptively selects the
MCS table without UL 256QAM or the
MCS table with UL 256QAM for UEs
based on channel quality.
FIXED_CONFIGURATIONThe eNodeB always selects the MCS
table with UL 256QAM
b
for UEs.
a. This policy is recommended. If channel quality becomes poor, the eNodeB
adaptively switches to the MCS table without UL 256QAM for the UEs,
maintaining the UL rates of QPSK-based services for the UEs. As the eNodeB
must use RRC signaling to notify UEs of the selected MCS table, this policy
increases RRC signaling overhead.
b. The MCS table with UL 256QAM references fewer low-order TBSs (TBSs with
indexes 1, 3, 5, 7, and 9 are not supported) than the MCS table without UL
256QAM. Therefore, this policy may result in decreases in the UL rates of QPSK-
based services for 256QAM-capable UEs and increases in their RBLERs and
service drop risks.

In FDD, an MCS table with UL 256QAM can be specified for whitelisted UEs. The
configuration index for whitelisted UEs is specified by the
Ul256QamUePara.
Ul256QamUeConfigIndex parameter, and the MCS table with
UL 256QAM for whitelisted UEs is specified by the
Ul256QamUePara.
Ul256QamCssMcsTab parameter. This function takes effect
when the UeCompat.
Ul256QamUeConfigIndex parameter value is consistent
with the Ul256QamUePara.
Ul256QamUeConfigIndex parameter value for
whitelisted UEs. For details about whitelisted UEs, see
## Terminal Awareness
## Differentiation
## .
## 5.2.2 Network Analysis
## 5.2.2.1 Benefits
The benefits of UL 256QAM vary depending on radio channel quality, the error
vector magnitude (EVM) of RF signals sent by UEs, and the EVM of signals
received by eNodeBs. This function is recommended when radio conditions are
favorable, for example, when the proportion of times MCS index 28 is selected for
scheduling on the PUSCH (indicated by L.ChMeas.PUSCH.MCS.28) is more than
30% of scheduling occasions, according to 24-hour statistics. In this scenario, UL
256QAM offers the following benefits:
●  The Cell Uplink Average Throughput increases by up to 40%.
●  The UL peak UE throughput increases by 10% to 40%.
If the preceding conditions are not met, UL 256QAM cannot be selected for most
UEs in the cell. In this case, UL 256QAM cannot achieve the optimal gains.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.23

In FDD, the average UL user-perceived throughput increases when MCS table
selection and power reduction estimation for whitelisted UEs supporting UL
256QAM are enabled.
Average UL user-perceived throughput = L.Thrp.bits.UE.UL.Experienced/
L.Thrp.Time.UE.UL.Experienced
In FDD, RB resource allocation optimization for UL 256QAM when the CSS is used
increases the uplink PRB usage, number of successful SCell additions for CA UEs
and average number of downlink CA UEs (indicated by L.CA.DLSCell.Add.Succ
and L.Traffic.User.PCell.DL.Avg), and the E-RAB Setup Success Rate, and
decreases the service drop rate of UEs.
Uplink PRB usage = L.ChMeas.PRB.UL.Used.Avg/L.ChMeas.PRB.UL.Avail
## 5.2.2.2 Impacts
## Network Impacts
When the eNodeB selects the MCS table with UL 256QAM for UEs, the number of
times MCSs indicating UL 256QAM are selected is measured by counters
L.ChMeas.PUSCH.256QAM.MCS.0 to L.ChMeas.PUSCH.256QAM.MCS.31 and
L.ChMeas.PUSCH.MCS.0 to L.ChMeas.PUSCH.MCS.31. As a TBS index
corresponds to a lower MCS index when the MCS table with UL 256QAM is
selected than when the MCS table without UL 256QAM is selected, the average
MCS index calculated by using counters L.ChMeas.PUSCH.MCS.0 to
L.ChMeas.PUSCH.MCS.31 slightly decreases.
In FDD, if UL 256QAM is enabled, the number of times MCS index 0 is used
(indicated by L.ChMeas.PUSCH.MCS.0) may account for a larger proportion and
the values of counters such as L.Traffic.UL.SCH.QPSK.TB may increase.
In FDD, RB resource allocation optimization for UL 256QAM when the CSS is used
may change the average uplink MCS index, uplink IBLER, uplink RBLER, average
uplink SUNPT in a cell (L.Traffic.SUNPT.UL.Avg), number of uplink TBs, average
uplink cell throughput (Cell Uplink Average Throughput), and average uplink
user-perceived throughput. Specifically:
●  Average uplink MCS index = (L.ChMeas.PUSCH.MCS.0 x 0 +
L.ChMeas.PUSCH.MCS.1 x 1 + ... + L.ChMeas.PUSCH.MCS.28 x 28)/Sum of
L.ChMeas.PUSCH.MCS.0 through L.ChMeas.PUSCH.MCS.28
●  Uplink IBLER = (L.Traffic.UL.SCH.QPSK.ErrTB.Ibler +
L.Traffic.UL.SCH.16QAM.ErrTB.Ibler + L.Traffic.UL.SCH.64QAM.ErrTB.Ibler +
L.Traffic.UL.SCH.256QAM.ErrTB.Ibler)/(L.Traffic.UL.SCH.QPSK.TB +
L.Traffic.UL.SCH.16QAM.TB + L.Traffic.UL.SCH.64QAM.TB +
L.Traffic.UL.SCH.256QAM.TB)
●  Uplink RBLER = (L.Traffic.UL.SCH.QPSK.ErrTB.Rbler +
L.Traffic.UL.SCH.16QAM.ErrTB.Rbler + L.Traffic.UL.SCH.64QAM.ErrTB.Rbler
+ L.Traffic.UL.SCH.256QAM.ErrTB.Rbler)/(L.Traffic.UL.SCH.QPSK.TB +
L.Traffic.UL.SCH.16QAM.TB + L.Traffic.UL.SCH.64QAM.TB +
L.Traffic.UL.SCH.256QAM.TB)
●  Number of uplink TBs = L.Traffic.UL.SCH.QPSK.TB +
L.Traffic.UL.SCH.16QAM.TB + L.Traffic.UL.SCH.64QAM.TB +
L.Traffic.UL.SCH.256QAM.TB
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.24

●  Average UL user-perceived throughput = L.Thrp.bits.UE.UL.Experienced/
L.Thrp.Time.UE.UL.Experienced
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDExtended CPCell.UlCyclicPr
efix
Extended CPExtended CP takes
precedence over UL
## 256QAM.
FDDeMTC
introduction
## EMTC_SWITCH
option of the
CellEmtcAlgo.E
mtcAlgoSwitch
parameter
eMTCUL 256QAM does not
take effect for eMTC
UEs and CE UEs.
FDDShort TTISHORT_TTI_S
W option of
the
CellShortTtiAl
go.SttiAlgoSwi
tch
parameter
Short TTI
## (FDD)
UL 256QAM does not
take effect for short
TTI UEs.
FDDNB-IoTCell.NbCellFla
g
NB-IoT Basics
## (FDD)
UL 256QAM does not
take effect for NB-IoT
UEs.
FDDHigh speed
mobility
Cell.HighSpeed
## Flag
## High Speed
## Mobility
UL 256QAM does not
take effect in cells
enabled with high
speed mobility.
FDDUltra high
speed
mobility
Cell.HighSpeed
## Flag
## High Speed
## Mobility
UL 256QAM does not
take effect in cells
enabled with ultra
high speed mobility.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.25

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDSupport of
VoLTE
ENodeBAlgoS
witch.EutranV
oipSupportSwi
tch
VoLTEWhen UL 256QAM
takes effect for voice
service UEs, the uplink
IBLER may increase.
As a result, the packet
loss rate of these UEs
may increase. To
prevent the impact,
uplink modulation
scheme restriction for
voice service UEs
(controlled by the
## VOLTE_FORBID_UL_2
56_QAM_SW option
of the
VolteAlgoConfig.
## Volt
eOptSwitch
parameter) can be
enabled to prohibit UL
256QAM for these
UEs.

## 5.2.3 Requirements
## 5.2.3.1 Licenses
## RAT
Feature IDFeature NameModelSales Unit
## FDDLEOFD-1803
## 01
## UL 256QAMLT1SUL256QA
## M
per cell

## 5.2.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.26

## 5.2.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
For FDD, the following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## Boards
For FDD, only the UBBPg board is compatible with this function.
RF Modules
For FDD, there are no requirements for RF modules.
## 5.2.3.4 Cells
For FDD, there are no requirements.
## 5.2.3.5 Others
UL 256QAM requires that UEs meet all of the following conditions:
●  For MR-DC UEs: The value of ul-256QAM-r15 in the UE capability message is
supported.
●  For other UEs: The value of ul-256QAM-r14 or ul-256QAM-perCC-InfoList-
r14 in the UE capability message is supported.
5.2.4 Operation and Maintenance
## 5.2.4.1 Data Configuration
## 5.2.4.1.1 Data Preparation
Table 5-3 describes the parameters used for function activation.
Table 5-3 Parameters used for activation
## RAT
## Parameter
## Name
Parameter IDSetting Notes
## FDDUL 256QAM
## Algorithm
## Switch
PUSCHCfg.Ul
256QamAlgo
## Switch
To enable UL 256QAM, select
the UL_256QAM_SWITCH
option.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.27

RATParameter
## Name
Parameter IDSetting Notes
## FDDUL 256QAM
MCS Table
## Configuration
## Strategy
PUSCHCfg.Ul
256QamMcsT
blCfgStrateg
y
Set this parameter to its
recommended value.
## FDDUL 256QAM
MCS Table
## Adaptive
## Period
PUSCHCfg.Ul
256QamMcsT
blAdpPeriod
Set this parameter to its
recommended value.
FDDEstimated
## 256QAM
## Power
## Reduction
## Value
PUSCHCfg.Es
tdPowerRedu
ctValue256Q
am
Set this parameter to its
recommended value.
## FDDUL 256QAM
## UE
## Configuration
## Index
Ul256QamUe
Para.Ul256Q
amUeConfigI
ndex
Set this parameter based on
the network plan.
## FDDCSS MCS
Table for UL
## 256QAM UE
Ul256QamUe
Para.Ul256Q
amCssMcsTa
b
Set this parameter based on
the network plan.
FDDEstimated
## Power Reduct
Value for UL
## 256QAM UE
Ul256QamUe
Para.Ul256Q
amEstdPowR
eductValue
Set this parameter based on
the network plan.
FDDRsvSw8eNBCellRsvd
Para.RsvdSw
## Para8
Select BIT13 of this parameter
to enable RB resource
allocation optimization for UL
256QAM when the CSS is
used.

5.2.4.1.2 Using MML Commands
Before using MML commands, refer to 5.2.2.2 Impacts and complete the
parameter configurations for related functions based on the impact relationships
between the functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Enabling UL 256QAM
MOD PUSCHCFG: LocalCellId=0, Ul256QamAlgoSwitch=UL_256QAM_SWITCH-1;
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.28

//Enabling adaptive configuration of the MCS table with UL 256QAM
MOD PUSCHCFG: LocalCellId=0, Ul256QamMcsTblCfgStrategy=ADAPTIVE_CONFIGURATION;
//Setting the interval for adaptive selection of the MCS table with UL 256QAM to 10s
MOD PUSCHCFG: LocalCellId=0, Ul256QamMcsTblAdpPeriod=10;
//Setting the estimated power reduction value to 3 dB for UEs on which UL 256QAM takes effect
MOD PUSCHCFG: LocalCellId=0, EstdPowerReductValue256Qam=30;
//Setting the 64QAM MCS table as the table to be used by whitelisted UL 256QAM UEs and the estimated
power reduction value for UL 256QAM to 3 dB
ADD UL256QAMUEPARA: Ul256QamUeConfigIndex=0, Ul256QamEstdPowReductValue=30,
Ul256QamCssMcsTab=64QAM_TABLE;
//Enabling RB resource allocation optimization for UL 256QAM when the CSS is used
MOD ENBCELLRSVDPARA: LocalCellId=0, RsvdSwPara8=BIT13-1;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Disabling RB resource allocation optimization for UL 256QAM when the CSS is used
MOD ENBCELLRSVDPARA: LocalCellId=0, RsvdSwPara8=BIT13-0;
//Disabling UL 256QAM
MOD PUSCHCFG: LocalCellId=0, Ul256QamAlgoSwitch=UL_256QAM_SWITCH-0;
5.2.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.2.4.2 Activation Verification
If the value of at least one of the counters listed in Table 5-4 is greater than 0, UL
256QAM has taken effect.
Table 5-4 Counters related to UL 256QAM
Counter ID
## Counter Name
1526749492 to
## 1526749523
L.ChMeas.PUSCH.256QAM.MCS.0 to
L.ChMeas.PUSCH.256QAM.MCS.31
1526749524L.Traffic.UL.SCH.256QAM.TB

In FDD, to check how long the eNodeB uses the MCS table with UL 256QAM for a
specific UE, perform the following steps:
Step 1Check RRC connection reconfiguration messages sent by the eNodeB to the UE.
Find the message in which the IE PUSCH-ConfigDedicated-v1430 is contained and
the value of the IE enable256QAM-r14 is "setup". This message indicates that the
eNodeB starts using the MCS table with UL 256QAM for the UE. Record the time
point as A.
Step 2Check RRC connection reconfiguration messages sent by the eNodeB to the UE
after the previous message. Find the message in which the IE PUSCH-
ConfigDedicated-v1430 is contained and the value of the IE enable256QAM-r14 is
"release". This message indicates that the eNodeB stops using the MCS table with
UL 256QAM and starts to use the MCS table without UL 256QAM for the UE.
Record the time point as B.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.29

Step 3Calculate the period within which the MCS table with UL 256QAM is used for the
UE by subtracting A from B.
Step 4Take the sum of such periods as the total duration.
----End
## 5.2.4.3 Network Monitoring
Before activating UL 256QAM, operators can predict the proportion of times UL
256QAM will be selected by calculating the total proportion of times MCSs 27 and
28 indicating UL 64QAM have been selected. This is because, according to 3GPP
TS 36.213, these two proportions are expected to be similar. Note that the UEs for
which MCS 28 has been selected will benefit the most from UL 256QAM.
After UL 256QAM is activated in a cell, the probabilities of UL UE throughput in
high throughput ranges and Cell Uplink Average Throughput will increase with
the proportion of times UL 256QAM is selected for scheduling.
●  Proportion of times UL 256QAM is selected for scheduling
Proportion of times UL 256QAM is selected for scheduling =
L.Traffic.UL.SCH.256QAM.TB/(L.Traffic.UL.SCH.256QAM.TB +
L.Traffic.UL.SCH.64QAM.TB + L.Traffic.UL.SCH.16QAM.TB +
L.Traffic.UL.SCH.QPSK.TB)
●  Probability of UL UE throughput in each throughput range
Probability of UL UE throughput in throughput range
n =
L.Thrp.UL.BitRate.Samp.Indexn/sum(L.Thrp.UL.BitRate.Samp.Index0 to
L.Thrp.UL.BitRate.Samp.Index9), where
n is in the range of 0 to 9
In FDD, the average UL user-perceived throughput increases when MCS table
selection and power reduction estimation for whitelisted UEs for which UL
256QAM takes effect are enabled.
Average UL user-perceived throughput = L.Thrp.bits.UE.UL.Experienced/
L.Thrp.Time.UE.UL.Experienced
## 5.3 DL 256QAM
## 5.3.1 Principles
DL 256QAM incorporates the following functions:
●  Basic functions of DL 256QAM (see Basic Functions of DL 256QAM). For
details about the CQI table selection policy, see CQI Table Selection Policy.
●  DL TBS index optimization (see DL TBS Index Optimization)
Basic Functions of DL 256QAM
Figure 5-2 shows the procedure for DL 256QAM to take effect.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.30

Figure 5-2 DL 256QAM-related procedure
-  The eNodeB checks whether the Dl256QamSwitch option of the
CellAlgoSwitch
.Dl256QamAlgoSwitch parameter is selected.
–   If this option is selected, the eNodeB goes to 2.
–   If this option is deselected, the procedure ends. The eNodeB selects QPSK,
16QAM, or 64QAM for UEs based on channel quality.
-  The eNodeB checks whether a UE meets the requirements for DL 256QAM,
which are described in 5.3.3.5 Others.
–   If the UE meets the requirements, the eNodeB goes to 3.
–   If the UE does not meet the requirements, the procedure ends. The
eNodeB selects QPSK, 16QAM, or 64QAM for the UE based on channel
quality.
-  The eNodeB checks whether fixed CQI table selection is enabled. For details
about the CQI table selection policy, see CQI Table Selection Policy.
–   If the CellDlschAlgo.Dl256QamCqiTblCfgStrategy parameter is set to
FIX_CONFIG, the eNodeB always selects the CQI table with 256QAM for
UEs.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.31

–   If the CellDlschAlgo.Dl256QamCqiTblCfgStrategy parameter is set to a
value other than FIX_CONFIG, the eNodeB selects an appropriate CQI
table based on channel quality at an interval specified by the
CellDlschAlgo.Dl256QamCqiTblAdpPeriod parameter.
▪The shorter the interval, the better the selected CQI table matches
channel quality changes, and the higher the DL rates. However, RRC
connection reconfiguration messages are sent more frequently,
increasing the probability of service drops.
▪The longer the interval, the worse the selected CQI table matches
channel quality changes, and the lower the DL rates. However, RRC
connection reconfiguration messages are sent less frequently,
reducing the probability of service drops.
-  The eNodeB selects an appropriate modulation scheme for downlink
scheduling of the UE based on channel quality and the selected CQI table.
## NO TE
The highest-order modulation scheme for evolved multimedia broadcast/multicast service
(eMBMS) in the DL is 64QAM. Therefore, the CQI table without 256QAM is used during
scheduling of eMBMS services.
DL TBS Index Optimization
To further increase DL peak UE throughput, DL 256QAM supports DL TBS index
optimization with indexes 33A and 33B introduced.
●  DL TBS index optimization with index 33A introduced
DL TBS index optimization with index 33A introduced is enabled if the
MIMO_TBSIZE_OPT_SWITCH option of the CellAlgoSwitch.
DlSchExtSwitch
parameter is selected. For TM9/TM10-capable UEs that meet channel
condition requirements, the eNodeB sends RRC messages to inform these UEs
that the TBS of index 33A can be used, and also uses this TBS for DL data
transmission.
●  DL TBS index optimization with index 33B introduced
DL TBS index optimization with index 33B introduced is enabled if the
Dl256QamTbsIndexExtSwitch option of the
CellAlgoSwitch.
Dl256QamAlgoSwitch parameter is selected. For
TM1/TM2/TM3/TM4/TM6/TM7-capable UEs that meet channel condition
requirements, the eNodeB sends RRC messages to inform these UEs that the
TBS of index 33B can be used, and also uses this TBS for DL data
transmission.
CQI Table Selection Policy
3GPP defines two CQI tables based on whether 256QAM is included. For details,
see CQI Table.
During DL scheduling, the eNodeB selects an appropriate CQI table based on the
CellDlschAlgo.
Dl256QamCqiTblCfgStrategy parameter setting. Table 5-5
describes the CQI table selection policy.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.32

Table 5-5 CQI table selection policy
Value of
CellDlschAlgo.Dl256QamCqiTblCfgSt
rategy
CQI Table Selection Policy
## ADAPTIVE_CONFIG
a
The eNodeB adaptively selects the CQI
table without 256QAM or the CQI
table with 256QAM for UEs based on
the MCS.
## CQI_BASED_ADAPTIVE_CONFIG
a
The eNodeB adaptively selects the CQI
table without 256QAM or the CQI
table with 256QAM for UEs based on
the CQI and MCS.
FIX_CONFIGThe eNodeB always selects the CQI
table with 256QAM
b
for UEs.
a. If channel quality becomes poor, the eNodeB adaptively switches to the CQI
table without 256QAM for the UEs, maintaining the DL rates of QPSK-based
services for the UEs. As the eNodeB must use RRC signaling to notify UEs of the
selected CQI table, this policy increases RRC signaling overhead.
b. The CQI table with 256QAM references fewer low-order TBSs (TBSs with
indexes 1, 3, 5, 7, and 9 are not supported) than the CQI table without 256QAM.
Therefore, this policy may result in decreases in the DL rates of QPSK-based
services for 256QAM-capable UEs and increases in their RBLERs and service drop
risks.

## 5.3.2 Network Analysis
## 5.3.2.1 Benefits
These functions offer the following benefits:
●  Basic functions of DL 256QAM
The benefits of DL 256QAM vary depending on radio channel quality, the
EVM of RF signals sent by eNodeBs, and the EVM of signals received by UEs.
These functions are recommended when radio conditions are favorable, for
example, when the proportion of times MCS index 28 is selected for
scheduling on the PDSCH (indicated by L.ChMeas.PDSCH.MCS.28) is more
than 30% within 24 hours. They provide the following benefits:
–   The DL modulation efficiency for UEs at the cell center increases, thereby
increasing the User Downlink Average Throughput for these UEs by 0%
to 30%.
–   The DL peak cell throughput increases by 0% to 30%.
If the preceding conditions are not met, DL 256QAM cannot be selected for
most UEs in the cell. In this case, DL 256QAM cannot achieve the optimal
gains, but will not bring extra negative impacts.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.33

●  DL TBS index optimization
–   DL TBS index optimization with index 33A introduced increases the DL
peak throughput of TM9/TM10-capable UEs at the cell center by 3%–5%.
–   DL TBS index optimization with index 33B introduced increases the DL
peak throughput of TM1/TM2/TM3/TM4/TM6/TM7-capable UEs at the
cell center by 0.4% to 3%.
## 5.3.2.2 Impacts
## Network Impacts
DL 256QAM has impacts on the following KPIs and counters:
●  Impact on User Downlink Average Throughput
The User Downlink Average Throughput may decrease at locations where
the SINR reaches a certain value when DL 256QAM is enabled, because TBS
indexes newly defined in 3GPP specifications are nonlinear in the overlapping
areas where DL 256QAM and 64QAM take effect.
Assume that the cell bandwidth is 20 MHz, the PDCCH occupies one symbol,
the CQI table without 256QAM and the MCS table without DL 256QAM are
used for DL 64QAM at a location where the SINR reaches a certain value, the
TBS index can be 26, and the TBS is 75,376 bits. In this case, no block error
occurs. After DL 256QAM is enabled and the CQI table with 256QAM and
MCS table with DL 256QAM are used, TBS index 26 cannot be selected
because it is unavailable. In this case, TBS index 29 can be selected, but the
TBS is 73,712 bits and there are erroneous blocks, resulting in a decrease of
approximately 4% in the DL throughput.
●  Impact on the average CQI and average MCS index
When the CellDlschAlgo.
Dl256QamCqiTblCfgStrategy parameter is set to a
value other than FIX_CONFIG and the eNodeB selects the CQI table with
256QAM for UEs:
–   The number of periodic and aperiodic CQI reports sent by UEs for which
DL 256QAM is used is measured by counters
L.ChMeas.DL.256QAM.CQI.DL.0 to L.ChMeas.DL.256QAM.CQI.DL.15
and the number of periodic CQI reports sent by these UEs is also
measured by counters L.ChMeas.CQI.DL.0 to L.ChMeas.CQI.DL.15. Given
the same modulation scheme, the CQI indexes reported by UEs according
to the 3GPP-defined CQI table with 256QAM are smaller than those
reported according to the CQI table without 256QAM. As a result, the
average CQI index calculated by using counters L.ChMeas.CQI.DL.0 to
L.ChMeas.CQI.DL.15 decreases slightly.
–   The number of times MCSs indicating 256QAM are selected for these UEs
is measured by counters L.ChMeas.PDSCH.DL.256QAM.MCS.0 to
L.ChMeas.PDSCH.DL.256QAM.MCS.31 instead of
L.ChMeas.PDSCH.MCS.0 to L.ChMeas.PDSCH.MCS.31. As UEs with high
MCS indexes are more likely to switch to 256QAM, counters
L.ChMeas.PDSCH.MCS.0 to L.ChMeas.PDSCH.MCS.31 measure a smaller
number of times high MCS indexes are used. As a result, the average
MCS index calculated by using counters L.ChMeas.PDSCH.MCS.0 to
L.ChMeas.PDSCH.MCS.31 decreases slightly.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.34

The decreases are determined by the proportion of times DL 256QAM is
selected. The higher the proportion, the larger the decreases.
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDownlink
4x4 MIMO
NoneMIMOFor UEs that support
both DL 4x4 MIMO
and DL 256QAM,
enabling both
functions has an
impact on the
function effects
a
## .
FDDUltra high
speed
mobility
Cell.HighSpeed
## Flag
## High Speed
## Mobility
DL 256QAM does not
take effect in cells
enabled with ultra
high speed mobility.
FDDUMTS and
## LTE
spectrum
sharing
SpectrumClou
d.SpectrumClo
udSwitch set
to
## UL_SPECTRUM
## _SHARING
UMTS and
LTE Spectrum
## Sharing
With UMTS and LTE
Spectrum Sharing, the
LTE system is exposed
to interference from
the UMTS system. The
interference may
cause decreases in the
proportion of times
DL 256QAM is
selected and also in
the gains provided by
## DL 256QAM.
FDDGSM and
## LTE
spectrum
concurrency
SpectrumClou
d.SpectrumClo
udSwitch set
to
## GL_SPECTRUM
## _CONCURREN
## CY
GSM and LTE
## Spectrum
## Concurrency
With GSM and LTE
## Spectrum
Concurrency, the LTE
system is exposed to
interference from the
GSM system. The
interference may
cause decreases in the
proportion of times
DL 256QAM is
selected and also in
the gains provided by
## DL 256QAM.
FDDShort TTISHORT_TTI_S
W option of
the
CellShortTtiAl
go.SttiAlgoSwi
tch
parameter
Short TTI
## (FDD)
UEs scheduled in
short TTI mode do not
support DL 256QAM.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.35

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDL CoMP
cell
FDDHomNetDl
CompSwitch,
FDDHetNetDlC
ompSwitch,
and
Tm9JtSwitch
options of the
CellAlgoSwitch
## .
DlCompSwitch
parameter
DL CoMP
## (FDD)
If fixed CQI table
selection does not
take effect for the
serving cell
b
## , DL
256QAM-capable
non-JT UEs cannot be
selected as JT UEs.
## FDDCRS
dynamic
muting
## CRS_DYNAMIC
## _MUTING_SW
option of the
SymbolPwrSav
ing.SymbolShu
tdownEnhance
dSw
parameter
## Energy
## Conservation
and Emission
## Reduction
CRS muting reduces
inter-cell interference
and increases the
proportion of
occasions where
256QAM is selected.
FDDFlexible
## TM4 MU-
## MIMO
## FLEX_TM4_MU
## _MIMO_SW
option of the
CellMimoPara
Cfg.MimoSwitc
h
parameter
Low-Band
## Booster
Enabling DL 256QAM
will lower the
probability of UE
pairing for MU-MIMO.
FDDDownlink
intelligent
## JAMC
## CELL_DL_JOIN
## T_INTEL_AMC_
SW option of
the
CellIntelAmcC
onfig.
## Intellige
ntAmcSwitch
parameter
Smart 8T8R
## (FDD)
If downlink intelligent
JAMC is enabled and
then DL 256QAM is
enabled, the
conditions for
entering and exiting
DL 256QAM will be
changed and the
gains of DL 256QAM
will be affected.
FDDEnergy
saving
based on
flexible
frequency-
domain
scheduling
## FLEX_FREQ_SC
## H_ENERGY_SA
## VING_SW
option of the
CellPwrSaving
## Algo.
PwrSavin
gAlgoSwitch
parameter
## Energy
## Conservation
and Emission
## Reduction
Energy saving based
on flexible frequency-
domain scheduling
cannot take effect for
256QAM-capable UEs.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.36

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDRF channel
dynamic
muting in
## TM9
## TM9_TTI_CHN_
## DYN_MUTING_
SW option of
the
CellRfChnDyn
## Muting.
RfChn
DynMutingAlg
oSwitch
parameter
## Energy
## Conservation
and Emission
## Reduction
When there are
256QAM-capable UEs
in a cell, RF channel
dynamic muting in
TM9 cannot take
effect for the cell in
the current TTI.
a: For UEs that support both DL 4x4 MIMO and DL 256QAM, DL 256QAM will
offer lower gains or no gains if the UEs do not meet the conditions for DL
256QAM to take effect after they enter DL 4x4 MIMO mode. In addition, after
DL 256QAM is enabled, the threshold for adaptive switching between
transmission modes may be modified. As a result, the proportions of TM3 and
TM9 may change, leading to changes in the proportions of rank 3 and rank 4.
b: Fixed CQI table selection does not take effect when the
CellDlschAlgo.
Dl256QamCqiTblCfgStrategy parameter is set to
ADAPTIVE_CONFIG or CQI_BASED_ADAPTIVE_CONFIG.

## 5.3.3 Requirements
## 5.3.3.1 Licenses
## RAT
Feature IDFeature
## Name
ModelSales Unit
FDDLEOFD-110301DL 256QAMLT1SDL256QAMper cell

## 5.3.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 5.3.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.37

## Base Station Models
●  Basic functions of DL 256QAM
For FDD, the following base stations are compatible with these functions:
–   3900 and 5900 series base stations (macro base stations)
–   DBS3900 LampSite and DBS5900 LampSite
## –   BTS3912E
## –   BTS3911E
DL 256QAM does not work with the Radio Frequency Access (RFA)
application in which LTE RF signals are input into DBS3900 LampSite and
DBS5900 LampSite base stations.
●  DL TBS index optimization
–   DL TBS index optimization with index 33A introduced: Only 3900 and
5900 series base stations (macro base stations) are compatible with this
function.
–   DL TBS index optimization with index 33B introduced
For FDD, the following base stations are compatible with this function:
## ▪
3900 and 5900 series base stations (macro base stations)
## ▪
DBS3900 LampSite and DBS5900 LampSite
## ▪
## BTS3912E
## ▪
## BTS3911E
## Boards
For FDD, only the LBBPc is incompatible with this function.
RF Modules
For FDD, RF modules that meet the following condition support DL 256QAM:
The Description field of the DSP BRDMFRINFO command output, indicating the
RF module type, is V3, V6, KUNLUN, KL, WUYI, WY, or AAU. Before running the
DSP BRDMFRINFO command, operators must run the DSP CELLPHYTOPO
command to obtain the cabinet, subrack, and slot numbers of the RF modules.
## 5.3.3.4 Cells
●  Basic functions of DL 256QAM: no requirements
●  DL TBS index optimization: This function is supported only in cells with a 10
MHz, 15 MHz, or 20 MHz bandwidth.
## 5.3.3.5 Others
●  Basic functions of DL 256QAM
UEs must meet all of the following conditions:
–   The value of dl-256QAM-r12 in the UE capability message is supported.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.38

–   The UEs are of category 11 or higher.
●  DL TBS index optimization
–   DL TBS index optimization with index 33A introduced: UEs must comply
with 3GPP Release 12 or later. That is, the value of alternativeTBS-
Indices-r12 in the UE capability message must be supported.
–   DL TBS index optimization with index 33B introduced: UEs must comply
with 3GPP Release 14 or later. That is, the value of alternativeTBS-
Indices-r14 in the UE capability message must be supported.
5.3.4 Operation and Maintenance
## 5.3.4.1 Data Configuration
## 5.3.4.1.1 Data Preparation
Table 5-6 describes the parameters used for function activation.
Table 5-6 Parameters used for activation
## RA
## T
## Parameter
## Name
Parameter IDOptionSetting Notes
## FD
## D
## Downlink
## 256QAM
## Algorithm
## Switch
CellAlgoSwitc
h.Dl256QamAl
goSwitch
Dl256QamSwit
ch
It is recommended
that this option be
selected.
## FD
## D
## DL 256QAM
CQI Table
## Configure
## Strategy
CellDlschAlgo.
Dl256QamCqi
TblCfgStrateg
y
NoneSet this parameter to
its recommended
value.
## FD
## D
## DL 256QAM
CQI Table
## Adaptive
## Period
CellDlschAlgo.
Dl256QamCqi
TblAdpPeriod
NoneSet this parameter to
its recommended
value.
## FD
## D
DL Scheduling
## Extension
## Switch
CellAlgoSwitc
h.DlSchExtSwi
tch
## MIMO_TBSIZE_
## OPT_SWITCH
It is recommended
that this option be
selected when there
are TM9/TM10-
capable UEs.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.39

## RA
## T
## Parameter
## Name
Parameter IDOptionSetting Notes
## FD
## D
## Downlink
## 256QAM
## Algorithm
## Switch
CellAlgoSwitc
h.Dl256QamAl
goSwitch
Dl256QamTbsI
ndexExtSwitch
It is recommended
that this option be
selected. With this
option selected, it is
recommended that
the
CellDlschAlgo.
## Pdsch
MaxCodeRate
parameter be set to
## R14_0DOT932.

5.3.4.1.2 Using MML Commands
Before using MML commands, refer to 5.3.2.2 Impacts and complete the
parameter configurations for related functions based on the impact relationships
between the functions, as well as the actual network scenario.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
Activation Command Examples (FDD)
//Enabling basic functions of DL 256QAM
MOD CELLALGOSWITCH: LocalCellId=0, Dl256QamAlgoSwitch=Dl256QamSwitch-1;
//Enabling adaptive selection of the CQI table with DL 256QAM
MOD CELLDLSCHALGO: LocalCellId=0, Dl256QamCqiTblCfgStrategy=ADAPTIVE_CONFIG;
//Setting the interval for adaptive selection of the CQI table with DL 256QAM to 10s
MOD CELLDLSCHALGO: LocalCellId=0, Dl256QamCqiTblAdpPeriod=10;
//Enabling DL TBS index optimization with index 33A introduced when there are TM9/TM10-capable UEs
MOD CELLALGOSWITCH: LocalCellId=0, DlSchExtSwitch=MIMO_TBSIZE_OPT_SWITCH-1;
//Enabling DL TBS index optimization with index 33B introduced
MOD CELLALGOSWITCH: LocalCellId=0, Dl256QamAlgoSwitch=Dl256QamTbsIndexExtSwitch-1;
MOD CELLDLSCHALGO: LocalCellId=0, PdschMaxCodeRate=R14_0DOT932;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Disabling the DL TBS optimization with index 33A introduced
MOD CELLALGOSWITCH: LocalCellId=0, DlSchExtSwitch=MIMO_TBSIZE_OPT_SWITCH-0;
//Disabling the DL TBS optimization with index 33B introduced
MOD CELLALGOSWITCH: LocalCellId=0, Dl256QamAlgoSwitch=Dl256QamTbsIndexExtSwitch-0;
//Disabling basic functions of DL 256QAM
MOD CELLALGOSWITCH: LocalCellId=0, Dl256QamAlgoSwitch=Dl256QamSwitch-0;
5.3.4.1.3 MAE-Deployment (FDD)
●  Fast batch activation
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.40

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
## 5.3.4.2 Activation Verification
Basic Functions of DL 256QAM
If the value of at least one of the counters listed in Table 5-7 is greater than 0,
basic functions of DL 256QAM have taken effect.
Table 5-7 Counters related to DL 256QAM
Counter IDCounter Name
1526739656L.Traffic.DL.SCH.256QAM.TB
1526739657L.Traffic.DL.SCH.256QAM.TB.bits
1526739658L.Traffic.DL.SCH.256QAM.TB.Retrans
1526739659L.Traffic.DL.SCH.256QAM.TB.Retrans.
bits
1526739660L.Traffic.DL.SCH.256QAM.ErrTB.Ibler
1526739661L.Traffic.DL.SCH.256QAM.ErrTB.Rbler
1526739662 to 1526739677L.ChMeas.DL.256QAM.CQI.DL.0 to
L.ChMeas.DL.256QAM.CQI.DL.15
1526739682 to 1526739713L.ChMeas.PDSCH.DL.256QAM.MCS.0
to
L.ChMeas.PDSCH.DL.256QAM.MCS.3
## 1
1526739719L.Traffic.DL.SCH.256QAM.TB.NACK
1526741865L.CA.PCell.Traffic.DL.SCH.256QAM.TB
1526741866L.CA.SCell.Traffic.DL.SCH.256QAM.TB
1526741867L.CA.PCell.Traffic.DL.SCH.256QAM.Er
rTB.Ibler
1526741868L.CA.SCell.Traffic.DL.SCH.256QAM.Er
rTB.Ibler
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.41

Counter IDCounter Name
1526741869L.CA.PCell.Traffic.DL.SCH.256QAM.Er
rTB.Rbler
1526741870L.CA.SCell.Traffic.DL.SCH.256QAM.Er
rTB.Rbler
1526741862L.Traffic.DL.SCH.256QAM.TB.QCI.1
1526741863L.Traffic.DL.SCH.256QAM.TB.Retrans.
## QCI.1
1526741864L.Traffic.DL.SCH.256QAM.ErrTB.Ibler.
## QCI.1
1526741857L.Traffic.DL.SCH.256QAM.DRB.TB
1526741858L.Traffic.DL.SCH.256QAM.DRB.TB.Ret
rans
1526741859L.Traffic.DL.SCH.256QAM.DRB.ErrTB.I
bler
1526741860L.Traffic.DL.SCH.256QAM.DRB.ErrTB.
## Rbler
1526741861L.Traffic.DL.SCH.256QAM.ErrTB.bits.R
bler

To check how long the eNodeB uses the CQI table with 256QAM for a specific UE,
perform the following steps:
Step 1Check RRC connection reconfiguration messages sent by the eNodeB to the UE.
Find the first message in which the IE CQI-ReportConfig contains the field altCQI-
Table-r12. The presence of this field indicates that the eNodeB starts using the CQI
table with 256QAM for the UE. Record the time point as A.
Step 2Check RRC connection reconfiguration messages sent by the eNodeB to the UE
after the previous message. Find the first message in which the IE CQI-
ReportConfig no longer contains the field altCQI-Table-r12. The absence of this
field indicates that the eNodeB stops using the CQI table with 256QAM and starts
to use the CQI table without 256QAM for the UE. Record the time point as B.
Step 3Calculate the period within which the CQI table with 256QAM is used for the UE
by subtracting A from B.
Step 4Take the sum of such periods as the total duration.
----End
DL TBS Index Optimization
Perform the following steps to check whether DL TBS index optimization has
taken effect, by tracing air interface signaling on the MAE-Access.
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.42

Step 1On the MAE-Access, start a Uu interface tracing task by choosing Monitor >
Signaling Trace > Signaling Trace Management > LTE > Application Layer > Uu
## Interface Trace.
Step 2Check the Uu interface tracing result.
●  If the PDSCH-Config IE in the RRC_CONN_RECFG message contains the
PDSCH-ConfigDedicated-v1280 field whose value is a33, DL TBS index
optimization with index 33A introduced has taken effect.
●  If the PDSCH-Config IE in the RRC_CONN_RECFG message contains the
PDSCH-ConfigDedicatedSCell-v1430 field whose value is b33, DL TBS index
optimization with index 33B introduced has taken effect.
----End
## 5.3.4.3 Network Monitoring
Before activating DL 256QAM, operators can predict the proportion of times DL
256QAM will be selected by calculating the total proportion of times MCSs 27 and
28 indicating DL 64QAM have been selected. This is because, according to 3GPP
TS 36.213, these two proportions are expected to be similar. Note that the UEs for
which MCS 28 has been selected will benefit the most from DL 256QAM.
After DL 256QAM is activated in a cell, the probabilities of DL UE throughput in
high throughput ranges and Cell Downlink Average Throughput will increase
with the proportion of times DL 256QAM is selected for scheduling.
●  Proportion of times DL 256QAM is selected for scheduling
Proportion of times DL 256QAM is selected for scheduling =
L.Traffic.DL.SCH.256QAM.TB/(L.Traffic.DL.SCH.256QAM.TB +
L.Traffic.DL.SCH.64QAM.TB + L.Traffic.DL.SCH.16QAM.TB +
L.Traffic.DL.SCH.QPSK.TB)
●  Probability of DL UE throughput in each throughput range
Probability of DL UE throughput in throughput range
n =
L.Thrp.DL.BitRate.Samp.Index
n/sum(L.Thrp.DL.BitRate.Samp.Index0 to
L.Thrp.DL.BitRate.Samp.Index9), where
n is in the range of 0 to 9
eRAN
## Modulation Schemes Feature Parameter Description5 Enhanced Modulation Functions
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.43

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
## Modulation Schemes Feature Parameter Description6 Parameters
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.44

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
## Modulation Schemes Feature Parameter Description7 Counters
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.45

## 8 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
## Modulation Schemes Feature Parameter Description8 Glossary
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.46

## 9 Reference Documents
-  3GPP TS 36.211: "Evolved Universal Terrestrial Radio Access (E-UTRA);
Physical channels and modulation"
-  3GPP TS 36.213: "Physical layer procedures"
-  3GPP TS 36.321: "Evolved Universal Terrestrial Radio Access (E-UTRA);
Medium Access Control (MAC) protocol specification"
-  3GPP TS 36.331: "RRC Protocol Specification"
## 5.
## MIMO
6.eMTC
7.UMTS and LTE Spectrum Sharing
8.GSM and LTE Spectrum Concurrency
9.Short TTI (FDD)
10.DL CoMP (FDD)
11.High Speed Mobility
12.Low-Band Booster
13.NB-IoT Basics (FDD)
14.Smart 8T8R (FDD)
15.Energy Conservation and Emission Reduction
16.Terminal Awareness Differentiation
17.VoLTE
eRAN
## Modulation Schemes Feature Parameter Description9 Reference Documents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.47