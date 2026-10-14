

eRAN
## Channel State Management
## Feature Parameter Description
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
1.2 eRAN18.1 07 (2023-09-14)..................................................................................................................................................1
1.3 eRAN18.1 06 (2023-04-23)..................................................................................................................................................2
1.4 eRAN18.1 05 (2023-02-01)..................................................................................................................................................2
1.5 eRAN18.1 04 (2022-10-25)..................................................................................................................................................3
1.6 eRAN18.1 03 (2022-07-29)..................................................................................................................................................3
1.7 eRAN18.1 02 (2022-05-23)..................................................................................................................................................3
1.8 eRAN18.1 01 (2022-03-08)..................................................................................................................................................4
1.9 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 4
2 About This Document.............................................................................................................7
2.1 General Statements................................................................................................................................................................ 7
2.2 Applicable RAT......................................................................................................................................................................... 7
2.3 Features in This Document.................................................................................................................................................. 8
3 Overview....................................................................................................................................9
3.1 CSI Reporting Modes..............................................................................................................................................................9
3.2 Periodic and Aperiodic CQI Reporting........................................................................................................................... 11
4 CQI Reporting.........................................................................................................................13
4.1 Principles.................................................................................................................................................................................. 13
4.1.1 Periodic CQI Reporting.................................................................................................................................................... 13
4.1.2 Aperiodic CQI Reporting................................................................................................................................................. 14
4.1.3 Optimized CQI Detection................................................................................................................................................15
4.1.4 NPREO Constant Optimization (FDD)....................................................................................................................... 15
4.1.5 CRS-IC-based UE Steering (FDD).................................................................................................................................18
4.2 Network Analysis.................................................................................................................................................................. 19
4.2.1 Benefits................................................................................................................................................................................. 19
4.2.2 Impacts..................................................................................................................................................................................20
4.3 Requirements......................................................................................................................................................................... 28
4.3.1 Licenses................................................................................................................................................................................. 28
4.3.2 Software................................................................................................................................................................................28
4.3.3 Hardware..............................................................................................................................................................................29
4.3.4 Others....................................................................................................................................................................................30
eRAN
## Channel State Management Feature Parameter
DescriptionContents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iii

4.4 Operation and Maintenance.............................................................................................................................................30
4.4.1 Data Configuration (FDD)..............................................................................................................................................30
4.4.1.1 Data Preparation............................................................................................................................................................ 30
4.4.1.2 Using MML Commands............................................................................................................................................... 34
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 36
4.4.2 Activation Verification......................................................................................................................................................36
4.4.3 Network Monitoring.........................................................................................................................................................38
5 CQI Reporting Optimization...............................................................................................40
5.1 Principles.................................................................................................................................................................................. 40
5.1.1 Periodic CQI Reporting Optimization......................................................................................................................... 40
5.1.2 Aperiodic CQI Reporting Optimization...................................................................................................................... 41
5.1.2.1 UEs in the Initial Access...............................................................................................................................................41
5.1.2.2 UEs Involved in Handovers......................................................................................................................................... 41
5.1.2.3 UEs with Compatibility Issues....................................................................................................................................41
5.2 Network Analysis.................................................................................................................................................................. 42
5.2.1 Benefits................................................................................................................................................................................. 42
5.2.2 Impacts..................................................................................................................................................................................43
5.3 Requirements......................................................................................................................................................................... 43
5.3.1 Licenses................................................................................................................................................................................. 43
5.3.2 Software................................................................................................................................................................................43
5.3.3 Hardware..............................................................................................................................................................................43
5.3.4 Others....................................................................................................................................................................................44
5.4 Operation and Maintenance.............................................................................................................................................44
5.4.1 Data Configuration (FDD)..............................................................................................................................................44
5.4.1.1 Data Preparation............................................................................................................................................................ 44
5.4.1.2 Using MML Commands............................................................................................................................................... 45
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 45
5.4.2 Activation Verification......................................................................................................................................................46
5.4.3 Network Monitoring.........................................................................................................................................................48
6 CQI Adjustment..................................................................................................................... 49
6.1 Principles.................................................................................................................................................................................. 49
6.1.1 Downlink Target IBLER.................................................................................................................................................... 49
6.1.1.1 Fixed Configuration....................................................................................................................................................... 49
6.1.1.2 Adaptive Configuration................................................................................................................................................ 50
6.1.2 CQI Adjustment Period (FDD)...................................................................................................................................... 51
6.1.3 CQI Filtering Adjustment................................................................................................................................................ 52
6.1.3.1 Initial Filtered Value of Reported CQIs...................................................................................................................52
6.1.3.2 CQI Filtering Based on Spectral Efficiency Optimization................................................................................. 52
6.1.4 Optimized CQI Adjustment Value (FDD)..................................................................................................................52
6.1.4.1 Initial CQI Adjustment Value (FDD)........................................................................................................................52
6.1.4.2 CQI Adjustment Step (FDD).......................................................................................................................................53
6.2 Network Analysis.................................................................................................................................................................. 53
eRAN
## Channel State Management Feature Parameter
DescriptionContents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iv

6.2.1 Benefits................................................................................................................................................................................. 54
6.2.2 Impacts..................................................................................................................................................................................54
6.3 Requirements......................................................................................................................................................................... 57
6.3.1 Licenses................................................................................................................................................................................. 57
6.3.2 Software................................................................................................................................................................................58
6.3.3 Hardware..............................................................................................................................................................................58
6.3.4 Others....................................................................................................................................................................................59
6.4 Operation and Maintenance.............................................................................................................................................59
6.4.1 Data Configuration (FDD)..............................................................................................................................................59
6.4.1.1 Data Preparation............................................................................................................................................................ 59
6.4.1.2 Using MML Commands............................................................................................................................................... 60
6.4.1.3 Using the MAE-Deployment...................................................................................................................................... 61
6.4.2 Activation Verification......................................................................................................................................................61
6.4.3 Network Monitoring.........................................................................................................................................................62
7 Parameters..............................................................................................................................64
8 Counters.................................................................................................................................. 65
9 Glossary................................................................................................................................... 66
10 Reference Documents........................................................................................................ 67
eRAN
## Channel State Management Feature Parameter
DescriptionContents
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
Revised descriptions in this document.
1.2 eRAN18.1 07 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
Added the descriptions of the impact relationships between data-learning-based
downlink intelligent AMC and the following functions: downlink target IBLER
adaptation, enhanced downlink target IBLER adaptation, variable-step-based CQI
eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.1

adjustment, and adaptive variable-step-based CQI adjustment. For details, see
## 6.2.2 Impacts.
Added the descriptions of the impact relationships between downlink intelligent
JAMC and the following functions: variable-step-based CQI adjustment and
adaptive variable-step-based CQI adjustment. For details, see 6.2.2 Impacts.
Rectified the MML command examples for NPREO constant optimization. For
details, see 4.4.1.2 Using MML Commands.
Revised the MML command examples for CQI reporting. For details, see 4.4.1.2
Using MML Commands.
Revised the MML command examples for CQI reporting optimization. For details,
see 5.4.1.2 Using MML Commands.
Revised the MML command examples for CQI adjustment. For details, see 6.4.1.2
Using MML Commands.
1.3 eRAN18.1 06 (2023-04-23)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
Added the descriptions of the impact relationships between data-learning-based
downlink intelligent AMC and the following functions: downlink target IBLER
adaptation, enhanced downlink target IBLER adaptation, variable-step-based CQI
adjustment, and adaptive variable-step-based CQI adjustment. For details, see
## 6.2.2 Impacts.
Added the descriptions of the impact relationships between downlink intelligent
JAMC and the following functions: variable-step-based CQI adjustment and
adaptive variable-step-based CQI adjustment. For details, see 6.2.2 Impacts.
1.4 eRAN18.1 05 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
●  Revised descriptions in this document.
eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.2

●  Added the description of the dependency between CQI filtering based on
spectral efficiency optimization and the number of CRS ports. For details, see
## Prerequisite Functions.
●  Added the descriptions of the mutually exclusive relationships between CQI
filtering based on spectral efficiency optimization and the following functions:
high speed mobility and ultra high speed mobility. For details, see Mutually
## Exclusive Functions.
1.5 eRAN18.1 04 (2022-10-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.6 eRAN18.1 03 (2022-07-29)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.7 eRAN18.1 02 (2022-05-23)
This issue includes the following changes.
## Technical Changes
## Change Description
Parameter ChangeRATBase Station Model
Added an impact
relationship between
cell-level NPREO
constant optimization
and simulated load.
For details, see 4.1.4
NPREO Constant
Optimization (FDD).
NoneFDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite

eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.3

## Editorial Changes
Revised descriptions in this document.
1.8 eRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.9 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 05 (2021-11-27).
## Technical Changes
Change DescriptionParameter ChangeRATBase Station Model
Added periodic
triggering of aperiodic
CQI reporting for UEs
running downlink
common large-packet
services. For details,
see:
## ●4.1.2 Aperiodic
CQI Reporting
## ●4.3.3 Hardware
## ●4.4.1.1 Data
## Preparation
●4.4.1.2 Using MML
## Commands
Added the
CellDlSchExtPar-
am.AperiodicCqiTri-
gUeType parameter.
FDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
Enabled micro base
stations to support
CQI filtering based on
spectral efficiency
optimization. For
details, see 6 CQI
## Adjustment.
Added the
CqiFltSpectralEf-
fOptSwitch option to
the
CellAlgoSwitch.CqiA
djAlgoSwitch
parameter.
## FDDBTS3202E
Enabled micro base
stations to support
CQI reporting interval
optimization for CA
UEs. For details, see 5
CQI Reporting
## Optimization.
Added the
CellCqiAdaptiveCfg.C
ellCqiAlgoSwitch
parameter.
## FDD● BTS3912E
## ● BTS3911E
## ● BTS3203E
## ● BTS3202E
eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.4

Change DescriptionParameter ChangeRATBase Station Model
Enabled micro base
stations to support
CRS-IC-based UE
steering. For details,
see 4 CQI Reporting.
Modified parameters:
● Added the
CrsIcHoSwitch
option to the
CellHoParaCfg.Ho
ModeSwitch
parameter.
● Added the
CrsIcHoTargetInd
option to the
EutranInterNFreq.
MobilityTargetInd
parameter.
## FDD● BTS3203E
## ● BTS3202E
Optimized the CQI
reporting interval for
CA UEs. For details,
see 5.1.1 Periodic CQI
## Reporting
## Optimization.
Added the
CellCqiAdaptiveCfg.C
ellCqiAlgoSwitch
parameter.
FDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E
## ● BTS3203E
## ● BTS3202E
Added the CRS-IC-
based UE steering
function. For details,
see:
●4.1.5 CRS-IC-based
UE Steering (FDD)
## ●4.2.1 Benefits
## ●4.2.2 Impacts
## ●4.4.1.1 Data
## Preparation
●4.4.1.2 Using MML
## Commands
Modified parameters:
● Added the
CrsIcHoSwitch
option to the
CellHoParaCfg.Ho
ModeSwitch
parameter.
● Added the
CrsIcHoTargetInd
option to the
EutranInterNFreq.
MobilityTargetInd
parameter.
FDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
## ● BTS3203E
## ● BTS3202E
Added CQI
adjustment value
optimization in
NPREO constant
optimization. For
details, see 4.1.4
NPREO Constant
Optimization (FDD).
Added the
CellDlpcPdschPa.UeN
preoAdjOptSwitch
parameter.
FDD3900 and 5900 series
base stations (macro
base stations)
eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.5

Change DescriptionParameter ChangeRATBase Station Model
Added an impact
relationship between
periodic CQI reporting
and CRS dynamic
muting. For details,
see 4.2.2 Impacts.
NoneFDD● 3900 and 5900
series base stations
(macro base
stations)
● DBS3900 LampSite
and DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E
## ● BTS3203E
## ● BTS3202E
Added an impact
relationship between
enhanced aperiodic
CQI reporting and
downlink intelligent
joint adaptive
modulation and
coding (JAMC). For
details, see 4.2.2
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
## ● BTS3203E
## ● BTS3202E

## Editorial Changes
Revised descriptions in this document.
eRAN
## Channel State Management Feature Parameter
## Description1 Change History
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.6

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
## Channel State Management Feature Parameter
## Description2 About This Document
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.7

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-002031Aperiodic CQI
## Reporting
4 CQI Reporting
LCOFD-171301Precise Channel
## Measurement
4.1.4 NPREO Constant
Optimization (FDD)
4.1.5 CRS-IC-based UE
Steering (FDD)
LBFD-060101Optimization of CQI
## Reporting
5 CQI Reporting
## Optimization
LBFD-00101501CQI Adjustment6 CQI Adjustment
eRAN
## Channel State Management Feature Parameter
## Description2 About This Document
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.8

## 3 Overview
UEs report channel state information (CSI) to the eNodeB. This CSI includes a
channel quality indicator (CQI), a precoding matrix indication (PMI), and a rank
indication (RI). The information is used for downlink user plane scheduling and
downlink multiple-input multiple-output (MIMO).
## CQI
A CQI is a measure of channel quality. The eNodeB automatically selects a
modulation and coding scheme (MCS) for data transmission to the UE based on
this measure.
## PMI
A PMI indicates a precoding matrix. The eNodeB performs closed-loop MIMO
transmission to the UE based on this indicator.
## RI
An RI is a rank that the eNodeB uses to determine the number of spatial
multiplexing layers for the UE.
3.1 CSI Reporting Modes
CSI reporting modes depend on CQI, PMI, and RI reporting modes:
●  The specific CSI reporting modes are described in Table 3-1.
●  RIs and CQIs/PMIs are reported in different subframes in periodic CSI
reporting mode. RIs and CQIs/PMIs are reported in the same subframes in
aperiodic CSI reporting mode.
eRAN
## Channel State Management Feature Parameter
## Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.9

Table 3-1 CSI reporting modes
## CSI
## Reporting
## Mode
CQI Reporting
## Mode
## PMI
## Reporting
## Mode
Periodic or
## Aperiodic
## Supporting
UEs
1-0WidebandNonePeriodicAll UEs
1-1WidebandWidebandPeriodic
1-2WidebandSub-bandAperiodic
2-0Wideband CQI
reporting, or
optimum sub-
band CQI
reporting at a
larger granularity
NonePeriodicUEs with the
corresponding
capabilities
Wideband CQI
reporting, or UE-
selected sub-
band CQI
reporting at a
smaller
granularity
NoneAperiodic
2-1Wideband CQI
reporting, or
optimum sub-
band CQI
reporting at a
larger granularity
WidebandPeriodic
2-2Wideband CQI
reporting, or UE-
selected sub-
band CQI
reporting at a
smaller
granularity
Sub-bandAperiodic
3-0Wideband CQI
reporting, or all
sub-band CQI
reporting at a
larger granularity
NoneAperiodicAll UEs
3-1Wideband CQI
reporting, or all
sub-band CQI
reporting at a
larger granularity
WidebandAperiodic
eRAN
## Channel State Management Feature Parameter
## Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.10

## CSI
## Reporting
## Mode
CQI Reporting
## Mode
## PMI
## Reporting
## Mode
Periodic or
## Aperiodic
## Supporting
UEs
3-2Wideband CQI
reporting, or all
sub-band CQI
reporting at a
larger granularity
Sub-bandAperiodicUEs in
compliance
with 3GPP
Release 12 or
later

Table 3-2 lists the CSI reporting modes supported by Huawei eNodeBs in different
MIMO transmission modes.
Table 3-2 CSI reporting modes for different MIMO transmission modes
## Transmission
## Mode
Periodic CSI Reporting ModeAperiodic CSI Reporting
## Mode
## TM11-03-0
## TM21-13-0
## TM31-03-0
TM41-11-2 (FDD only)
## 3-1
3-2 (FDD only)
TM61-11-2 (FDD only)
## 3-1
3-2 (FDD only)
TM91-11-2 (FDD only)
## 3-1
3-2 (FDD only)

3.2 Periodic and Aperiodic CQI Reporting
CQIs can be reported periodically or aperiodically. CQI reporting is configured the
same way as CSI reporting.
Figure 3-1 illustrates how the eNodeB selects a CQI reporting mode for a
scheduled UE.
●  For a UE in frequency selective scheduling (FSS) mode, the eNodeB selects
aperiodic CQI reporting.
●  For a UE in frequency diversity scheduling (FDS) mode, the eNodeB selects
periodic or aperiodic CQI reporting.
eRAN
## Channel State Management Feature Parameter
## Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.11

## NO TE
If the periodic CQI reporting time conflicts with the aperiodic CQI reporting time, only
aperiodic CQI reporting is triggered.
For details about FSS and FDS, see Scheduling.
Figure 3-1 CQI reporting mode selection for UEs in FSS and FDS modes
eRAN
## Channel State Management Feature Parameter
## Description3 Overview
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.12

4 CQI Reporting
## 4.1 Principles
In periodic mode, the CQI reporting intervals, reporting modes, and time-
frequency resources are configured in the
CQI-ReportConfig RRC IE.
●  When there is no uplink data transmission, CQIs are reported over the PUCCH.
●  When there is uplink data transmission, CQIs are reported over the PUSCH.
In aperiodic mode, the CQI reporting modes are specified in the uplink scheduling
indications sent to UEs and CQIs can be reported over the PUSCH only.
●  When the UE has data to be scheduled for uplink initial transmission, CQIs are
aperiodically reported together with data.
●  When the UE has no data to be scheduled for uplink initial transmission, CQIs
are reported in CQI-only mode.
The CQI-only mode increases both uplink overhead and uplink interference. To
minimize these adverse impacts, set the CellUlschAlgo.
AperiodicCsiUlTxMode
parameter to specify the transmission mode of aperiodic CQIs on the PUSCH.
●  If this parameter is set to CsiOnly and there is aperiodic CQI reporting, the UE
can immediately report CQIs in CQI-only mode or report CQIs aperiodically
together with data.
●  If this parameter is set to CsiWiUlService, there is aperiodic CQI reporting,
and the UE has no data to be scheduled for uplink initial transmission, the UE
cannot immediately report CQIs in CQI-only mode. This can reduce the
number of times of aperiodic CQI reporting in CQI-only mode and decreases
uplink interference. However, this transmission mode is not as prompt as
aperiodic CQI reporting in CQI-only mode. In this case, the downlink initial
block error rate (IBLER) slightly increases when uplink data services of the UE
are sparse.
4.1.1 Periodic CQI Reporting
The periodic CQI reporting interval is controlled by the
CellCqiAdaptiveCfg.CqiPeriodAdaptive parameter.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.13

●  If the parameter is set to ON, the reporting interval is adjusted based on the
PUCCH load. When the load is light, a short interval is used; when the load is
heavy, a longer interval is used.
In an FDD cell, the periodic CQI reporting interval varies across the range of
[CellCqiAdaptiveCfg.MinCqiPeriod, 160 ms].
●  If this parameter is set to OFF, the reporting interval is a fixed value specified
by the CellCqiAdaptiveCfg.UserCqiPeriod parameter.
4.1.2 Aperiodic CQI Reporting
Aperiodic CQI reporting allows the eNodeB to obtain more current downlink
channel quality and increase downlink transmission rates. However, aperiodic CQI
reporting consumes additional PDCCH resources. It is recommended that the
CellPdcchAlgo.
PdcchSymNumSwitch parameter be set to ECFIADAPTIONON to
reduce the number of symbols used by the PDCCH and increase downlink
transmission rates.
Configurations for aperiodic CQI reporting are different for UEs in FSS and FDS
modes.
UEs in FSS Mode
Aperiodic CQI reporting is triggered at intervals configured for UEs in FSS mode.
The interval is configured using the CellDlschAlgo.
FSUEAperCQITrigPeriod
parameter.
The CQIs that are aperiodically reported are only valid for a period of time
specified by the CellDlschAlgo.
FSUESbCQIValidityPeriod parameter. If a UE in
FSS mode does not use the aperiodically reported CQIs within this period of time,
these CQIs are considered invalid.
If this parameter, which specifies the validity period, is set to a value at least equal
to the value used for the triggering period
(CellDlschAlgo.
FSUEAperCQITrigPeriod), then FSS is more likely to be selected
for the UEs.
When smart frequency selective scheduling takes effect, the triggering interval
and validity period for UEs in FSS mode are adaptively adjusted but not specified
by CellDlschAlgo.
FSUEAperCQITrigPeriod or
CellDlschAlgo.FSUESbCQIValidityPeriod.
UEs in FDS Mode
Aperiodic CQI reporting is not triggered for UEs in FDS mode if there are valid
CQIs that are periodically reported. Aperiodic CQI reporting is triggered in the
following situations:
●  When there are no valid CQIs that are periodically reported in a period that is
eight times the periodic CQI reporting interval, aperiodic CQI reporting is
triggered once.
●  When there are no resources for periodic CQI reporting, aperiodic CQI
reporting is triggered every 160 ms.
In FDD, the eNodeB can trigger aperiodic CQI reporting at intervals for all UEs in
FDS mode. This function is controlled by the EnAperiodicCqiRptSwitch option of
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.14

the CellAlgoSwitch.DlSchSwitch parameter. The interval is specified by the
CellDlschAlgo.FDUEEnhAperCQITrigPeriod parameter.
In FDD, the eNodeB can also trigger aperiodic CQI reporting at intervals for UEs in
FDS mode that are running downlink common large-packet services. This function
is controlled by the CellDlSchExtParam.AperiodicCqiTrigUeType parameter. If the
Cell.CrsPortNum parameter is set to CRS_PORT_2 and the
CellDlSchExtParam.AperiodicCqiTrigUeType parameter is set to
COMMON_LARGE_PKT, aperiodic CQI reporting is triggered at intervals for UEs
running downlink common large-packet services. The downlink data volume
threshold for such UEs is specified by the CellDlschAlgo.
DlUserDataThld
parameter, and the interval is specified by the
CellDlschAlgo.FDUEEnhAperCQITrigPeriod parameter.
4.1.3 Optimized CQI Detection
False CQI detection is when the eNodeB detects a CQI but the UEs have not
reported any.
The eNodeB supports optimized CQI detection on the PUSCH and PUCCH, which
reduces the amount of false CQI detection on the network. This function is
controlled by the CellCqiAdjAlgo.
CqiOptSwitch parameter.
●  When the PUSCH_CQI_FALSE_DETECTION_SW option of this parameter is
selected, the amount of false CQI detection is reduced on the PUSCH.
●  When the PUCCH_CQI_FALSE_DETECTION_SW option of this parameter is
selected, the amount of false CQI detection is reduced on the PUCCH.
4.1.4 NPREO Constant Optimization (FDD)
As defined in 3GPP Release 8, nomPDSCH-RS-EPRE-Offset (NPREO) is a field
introduced in the CQI-ReportConfig information element (IE). The NPREO
constant is used to compensate for PDSCH SINR estimation for non-TM9/TM10
UEs. The NPREO constant can be specified by the
CellDlpcPdschPa.
NomPdschRsEpreOffset parameter.
●  A larger NPREO constant results in a larger proportion of high ranks reported
by UEs and larger CQIs reported in the same rank.
●  A smaller NPREO constant results in a smaller proportion of high ranks
reported by UEs and smaller CQIs reported in the same rank.
Properly set the NPREO constant to ensure that the CQIs and ranks reported by
UEs match PDSCH quality, thereby increasing downlink user-perceived rates.
The eNodeB supports the following two levels of NPREO constant optimization:
●  Cell-level NPREO constant optimization: This function is enabled when the
CellDlpcPdschPa.
CellNpreoAdjThreshold parameter is set to a value ranging
from 0 to 50 and disabled when the parameter is set to 255.
●  UE-level NPREO constant optimization: This function is enabled when the
CellDlpcPdschPa.
UeNpreoAdjThreshold parameter is set to a value ranging
from -2 to 20 and disabled when the parameter is set to 127.
The cell-level and UE-level NPREO constant optimization functions can be
simultaneously enabled. In this case, the two functions run independently.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.15

Cell-Level NPREO Constant Optimization
After the cell-level NPREO constant optimization function is enabled, the eNodeB
automatically searches for the optimal cell-level NPREO constant. The eNodeB
tries different cell-level NPREO constant values. If the estimated UE throughput of
value A divided by that of value B minus 1 is greater than the
CellDlpcPdschPa.
CellNpreoAdjThreshold parameter value, the eNodeB considers
that A is better than B. Once the optimal cell-level NPREO constant is determined,
it is used to replace the CellDlpcPdschPa.NomPdschRsEpreOffset parameter
value.
## NO TE
Due to real-time changes in network interference and load, the cell-level NPREO constant
optimization function searches again for the optimal NPREO constant in the latest network
environment one month after the last optimization.
If the deactivation of a cell is not caused by running the DEA CELL command, the data for
NPREO constant optimization before the deactivation can be retained for a maximum of 24
hours.
●   If the cell is restarted within 24 hours, the cell-level NPREO constant optimization
function will keep searching for a better constant based on the retained optimization
data.
●   If the cell is not restarted within 24 hours, the retained optimization data will be
deleted.
When the PRBs occupied by simulated load are measured using counters, the measurement
accuracy is affected. As such, it is recommended that they are not measured when cell-level
NPREO constant optimization is enabled.
UE-Level NPREO Constant Optimization
After the UE-level NPREO constant optimization function is enabled in a cell, the
eNodeB configures A3 measurement information for UEs that treat the cell as
their primary cell (PCell) and A6 measurement information for UEs that treat the
cell as their secondary cell (SCell). The eNodeB adjusts the NPREO constant of a
UE based on information such as A3 or A6 reports, neighboring cell RSRP values,
neighboring cell PCIs, and neighboring cell interference values. When the
CellDlpcPdschPa.
UeNpreoAdjThreshold parameter is not set to 127, the
parameter value indicates the compensation value of UE-level NPREO constant
optimization.
Figure 4-1 shows the UE-level NPREO constant optimization process.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.16

Figure 4-1 NPREO constant optimization process
The neighboring cell interference values are obtained by using a corresponding
algorithm of precise AMC. For details, see eMIMO (FDD).
If precise AMC and UE-level NPREO constant optimization are both enabled,
adjusting the CellDlschAlgo.
IntrfFilterCoeff parameter value will affect the
neighboring cell interference values obtained in precise AMC and UE-level NPREO
constant optimization.
The upper limit of UE-level NPREO constant adjustment is specified by the
CellDlpcPdschPa.
UeNpreoAdjUpperLimit parameter. The value 1 is
recommended when the PCI mod 3 values of adjacent cells on the network are
different, while the value 2 is recommended when the PCI mod 3 values of
adjacent cells on the network are the same.
To reduce the interference from LTE CRS to NR PDSCH when LTE and NR spectrum
sharing is enabled, you are advised to plan the same PCI mod 3 value for LTE cells
and configure the upper limit of UE-level NPREO constant adjustment for LTE
cells. This can increase the downlink user-perceived rates of UEs running downlink
large-packet (full buffer) services in LTE cells.
After UE-level NPREO constant optimization is enabled, you are advised to enable
CQI adjustment value optimization in NPREO constant optimization (by selecting
the CQI_ADJ_OPT_SW option of the CellDlpcPdschPa.
UeNpreoAdjOptSwitch
parameter) to avoid a sharp increase or decrease in the MCS indexes for UEs.
## NO TE
The A3 and A6 offsets are specified by the
NCellDlRsrpMeasPara.
NCellDlRsrpMeasA3Offset and
NCellDlRsrpMeasPara.DlRsrpNCellMeasA6Offset parameters, respectively. The smaller
the parameter values, the larger the range of non-cell-center areas and the greater the
number of UEs for which the UE-level NPREO constant optimization function takes effect.
For the exchange of interference information between inter-eNodeB neighboring cells, X2 or
eX2 interfaces are required. If X2 interfaces are used, service coordination must be
supported in non-ideal backhaul mode.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.17

4.1.5 CRS-IC-based UE Steering (FDD)
Cell-specific reference signal-interference cancellation (CRS-IC) capability refers to
crs-InterfHandl-r11, which is a field introduced in the UE capability IE, as defined
in 3GPP Release 11. It indicates whether a UE supports cancellation of interference
from neighboring cells to CRSs of the serving cell in time synchronization
scenarios.
When the planned PCI mod 3 values of adjacent cells are the same, UEs that do
not support CRS-IC in a cell will cause the channel quality of the cell to deteriorate
as they cannot cancel interference from neighboring cells. To address this issue,
CRS-IC-based UE steering is introduced, which is controlled by the CrsIcHoSwitch
option of the CellHoParaCfg.
HoModeSwitch parameter. After this function is
enabled, the eNodeB identifies crs-InterfHandl-r11 reported by UEs and performs
the following optimization to improve the CRS demodulation capability of UEs
that support CRS-IC in a cell working on a specific frequency and the cell's channel
quality.
●  For a cell working on a specific frequency
After the CrsIcHoSwitch option is selected for the cell:
–   UEs that support CRS-IC will be retained in the cell.
–   UEs that do not support CRS-IC will be handed over to a cell not working
on that specific frequency.
●  For a cell not working on that specific frequency
After the CrsIcHoSwitch option is selected for the cell, UEs that support CRS-
IC will be handed over to a cell working on that specific frequency.
The target frequency for CRS-IC-based handover is determined based on the
CrsIcHoTargetInd option of the EutranInterNFreq.
MobilityTargetInd parameter.
●  When a UE that supports CRS-IC is handed over to a cell working on a specific
frequency, the target frequency is a frequency with this option selected.
●  When a UE that does not support CRS-IC is handed over to a cell not working
on that specific frequency, the target frequency is not a frequency with this
option selected.
As shown in Figure 4-2, after CRS-IC-based UE steering is enabled, UE 1 stays in a
cell working on a specific frequency, UE 2 is handed over from a cell not working
on that specific frequency to the cell working on that specific frequency, and UE 3
is handed over from a cell working on a specific frequency to a cell not working
on that specific frequency.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.18

Figure 4-2 CRS-IC-based UE steering
## 4.2 Network Analysis
## 4.2.1 Benefits
eNodeBs increase downlink cell throughput based on periodic and aperiodic CQI
reporting.
Aperiodic CQI reporting, a supplement to periodic CQI reporting, provides real-
time UE channel states and increases downlink transmission rates.
For FDD, the gains of NPREO constant optimization are indicated by the User
## Downlink Average Throughput.
The factors that affect the gains of NPREO constant optimization are as follows:
●  PCI conflict: The larger the number of UEs in cells with PCI conflicts, the
higher the gains.
●  Inter-site distance (ISD): The smaller the ISD, the denser the network, the
greater the inter-UE interference in the cell, and the higher the gains of
NPREO constant optimization.
●  2T/4T network: On a 4T network, NPREO constant optimization can
significantly increase the proportion of high ranks and provide higher gains.
●  eX2 interface: If it is configured, inter-eNodeB interference information can be
obtained. As a result, the function can take effect for more UEs, providing
higher gains.
●  Proportion of TM9/TM10 UEs: NPREO constant optimization is mainly used to
adjust the estimated SINRs for non-TM9/TM10 UEs such as TM3/TM4 UEs.
The smaller the proportion of TM9/TM10 UEs, the higher the gains of NPREO
constant optimization.
As UE-level NPREO constant optimization requires neighboring cell information
exchange, it is recommended that UE-level NPREO constant optimization be
enabled in continuously covered areas.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.19

It is recommended that both cell-level and UE-level NPREO constant optimization
functions be enabled to maximize the overall gains when all the following
conditions are met. Under these conditions, when the optimal cell-level NPREO
constant is different from the CellDlpcPdschPa.NomPdschRsEpreOffset
parameter value, the User Downlink Average Throughput will increase by 1% to
## 5%.
●  The ISD does not exceed 700 m in densely populated urban areas.
●  The average downlink PRB usage in a day is greater than 20%.
●  4-port TM4 is supported on the network side.
For FDD, CRS-IC-based UE steering can reduce the Call Drop Rate (VoIP) and
increase the Intra-Frequency Handover Out Success Rate. You are advised to
enable this function when all the following conditions are met.
●  Time synchronization is used.
●  The ISD does not exceed 700 m in densely populated urban areas.
The gains of CRS-IC-based UE steering are affected by the following factors:
●  PCI conflict
The larger the number of UEs in cells with PCI conflicts, the higher the gains.
## ●  ISD
The smaller the ISD, the denser the network, the greater the inter-UE
interference in the cell, and the higher the gains.
## 4.2.2 Impacts
## Network Impacts
Aperiodic CQI reporting scheduled on the uplink in CQI-only mode occupies
PUSCH and PDCCH resources.
When the optimized CQI detection function is enabled, the average CQI value
increases slightly.
Average CQI value = (L.ChMeas.CQI.DL.0 x 0 + L.ChMeas.CQI.DL.1 x 1 +
L.ChMeas.CQI.DL.2 x 2 + L.ChMeas.CQI.DL.3 x 3 + L.ChMeas.CQI.DL.4 x 4 +
L.ChMeas.CQI.DL.5 x 5 + L.ChMeas.CQI.DL.6 x 6 + L.ChMeas.CQI.DL.7 x 7 +
L.ChMeas.CQI.DL.8 x 8 + L.ChMeas.CQI.DL.9 x 9 + L.ChMeas.CQI.DL.10 x 10 +
L.ChMeas.CQI.DL.11 x 11 + L.ChMeas.CQI.DL.12 x 12 + L.ChMeas.CQI.DL.13 x 13
+ L.ChMeas.CQI.DL.14 x 14 + L.ChMeas.CQI.DL.15 x 15)/∑(L.ChMeas.CQI.DL.0 to
L.ChMeas.CQI.DL.15)
For FDD, cell-level NPREO constant optimization proactively tries different NPREO
constant values. The downlink UE throughput may decrease by no more than 5%.
It takes at least one week for cell-level NPREO constant optimization to determine
the optimal NPREO constant. Therefore, the performance fluctuation lasts for
about one week.
UE-level NPREO constant optimization periodically measures the interference from
neighboring cells. If the interference changes greatly in the measurement period,
the accuracy of calculated interference will be affected. Consequently, the
performance of UE-level NPREO constant optimization will be affected and the
downlink user-perceived throughput may decrease. In addition, UE-level NPREO
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.20

constant optimization requires the UE to measure neighboring cell RSRP values
and report event A3 or A6 to the eNodeB. This consumes PDCCH CCE and PUSCH
RB resources and therefore affects uplink performance. The impact increases with
the growing number of UEs and the increased traffic volume of uplink services.
The number of used PDCCH CCEs can be observed using the
L.ChMeas.CCE.ULUsed.SRB and L.ChMeas.CCE.DLUsed.SRB counters.
NPREO constant optimization also causes other downlink cell KPIs to change,
including the proportion of high ranks, average CQI, average MCS index, PDSCH
IBLER, and PDSCH RBLER. For example, if the optimal cell-level NPREO constant is
greater than the CellDlpcPdschPa.
NomPdschRsEpreOffset parameter value, the
proportion of high ranks reported by UEs will increase.
CRS-IC-based UE steering causes other cell KPIs to change, including the average
CQI and average MCS index.
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDEnergy saving
based on
proactive
scheduling
SymbolPwrS
aving.TrigBn
dlSchDlAvgPr
bThld
## Energy
## Conservation
and Emission
## Reduction
Energy saving based
on proactive
scheduling may cause
fluctuations in the
number of CQI and
rank reporting times.
If the
CellCqiAdaptiveCfg.
## C
qiPeriodAdaptive
parameter is set to
ON, the number of
UEs that report CQIs
and ranks at short
intervals decreases
and the number of
UEs that report CQIs
and ranks at long
intervals increases.
FDDDedicated
carrier for
## TM9
Tm9Dedicate
dCarrier.Wor
kMode
## Dedicated
Carrier for
## TM9
When this function is
enabled, almost all
UEs in the cell work in
TM9. NPREO constant
adjustment has no
impact on TM9 UEs.
As NPREO constant
optimization has no
gains, enabling it is
not recommended.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.21

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDCRS dynamic
muting
## CRS_DYNAMI
## C_MUTING_S
W option of
the
SymbolPwrS
aving.
## Symbol
ShutdownEn
hancedSw
parameter
## Energy
## Conservation
and Emission
## Reduction
DRX On Duration
alignment performed
during CRS muting
may cause
fluctuations in the
number of CQI and
rank reporting times.
If the switch
controlled by
CellCqiAdaptiveCfg.
## C
qiPeriodAdaptive
is
on, the number of UEs
that report CQIs and
ranks at short
intervals decreases
and the number of
UEs that report CQIs
and ranks at long
intervals increases.
FDDCompact
bandwidth
Cell.Customiz
edBandWidt
hCfgInd
## Compact
## Bandwidth
## (FDD)
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the
punctured RBs to the
RBs in the configured
LTE bandwidth, the
lower the gains of
NPREO constant
optimization.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.22

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDLTE in-band
deployment
Prb.DeployM
ode
NB-IoT Basics
## (FDD)
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the NB-
IoT RBs to the RBs in
the configured LTE
bandwidth, the lower
the gains of NPREO
constant optimization.
FDDCDMA and
LTE Zero
## Bufferzone
AvoidCDMAI
nterfSwitch
option of the
CellAlgoSwit
ch.AvoidInter
fSwitch
parameter
CDMA and
LTE Zero
## Bufferzone
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the
downlink RBs shared
by LTE and CDMA to
the RBs in the
configured LTE
bandwidth, the lower
the gains of NPREO
constant optimization.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.23

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDGSM and LTE
## Buffer Zone
## Optimization
AvoidGeranIn
terfSwitch
option of the
CellAlgoSwit
ch.AvoidInter
fSwitch
parameter
GSM and LTE
## Buffer Zone
## Optimization
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the
downlink LTE RBs that
experience
interference from
GSM to the RBs in the
configured LTE
bandwidth, the lower
the gains of NPREO
constant optimization.
FDDUL Refarming
## Zero
## Bufferzone
AvoidUtranIn
terfSwitch
option of the
CellAlgoSwit
ch.AvoidInter
fSwitch
parameter
UL Refarming
## Zero
## Bufferzone
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the
downlink LTE RBs that
experience
interference from
UMTS to the RBs in
the configured LTE
bandwidth, the lower
the gains of NPREO
constant optimization.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.24

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDGSM and LTE
## Spectrum
## Concurrency
SpectrumClo
ud.Spectrum
CloudSwitch
GSM and LTE
## Spectrum
## Concurrency
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the RBs
shared by LTE and
GSM to the RBs in the
configured LTE
bandwidth, the lower
the gains of NPREO
constant optimization.
FDDFlexible
bandwidth
based on
overlapping
carriers
DdCellGroup.
DdBandwidt
h
## Flexible
## Bandwidth
based on
## Overlap
## Carriers
## (FDD)
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
The larger the
proportion of the
punctured RBs to the
RBs in the configured
LTE bandwidth, the
lower the gains of
NPREO constant
optimization.
FDDAdaptive SFN/
## SDMA
CellAlgoSwit
ch.SfnDlSchS
witch
SFNWhen this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
Therefore, you are
advised not to enable
UE-level NPREO
constant optimization.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.25

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDL CoMP cellFDDHomNet
DlCompSwitc
h and
FDDHetNetD
lCompSwitch
options of the
CellAlgoSwit
ch.
DlCompS
witch
parameter
DL CoMP
## (FDD)
When this function is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
UE-level NPREO
constant optimization.
Therefore, you are
advised not to enable
UE-level NPREO
constant optimization.
FDDPrecise AMCPreciseAmcS
witch option
of the
CellAlgoSwit
ch.EmimoSwi
tch
parameter
eMIMO
## (FDD)
When this function is
enabled, UE-level
NPREO constant
optimization uses the
same neighboring cell
interference values as
this function. If this
function has been
enabled and then UE-
level NPREO constant
optimization is
enabled, the gains of
NPREO constant
optimization may
decrease.
FDDDownlink
basic
frequency
selective
scheduling
FreqSelSwitc
h option of
the
CellAlgoSwit
ch.DlSchSwit
ch
parameter
SchedulingWhen downlink basic
frequency selective
scheduling is enabled,
modifying the UE-
level NPREO constant
may affect CQI and
rank reporting by UEs
in FSS mode, which in
turn affects FSS gains.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.26

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDownlink
smart
frequency
selective
scheduling
## SMART_FSS_
## SWITCH
option of the
CellAlgoSwit
ch.DlSchExtS
witch
parameter
SchedulingWhen downlink smart
frequency selective
scheduling is enabled
and CQI adjustment
value optimization in
NPREO constant
optimization is
disabled, the UE-level
NPREO constant is
always 0 to ensure
FSS gains.
FDDCSPCCspcAlgoPara
.CspcAlgoSwi
tch
CSPCWhen CSPC is
enabled, the accuracy
of neighboring cell
interference
calculation is affected,
which in turn affects
the performance of
CQI adjustment value
optimization in
NPREO constant
optimization. In this
case, you are advised
not to enable CQI
adjustment value
optimization in
NPREO constant
optimization.
FDDRank
detection
CellDlschAlg
o.DlRankDet
ectSwitch
NoneWhen rank detection
and CQI adjustment
value optimization in
NPREO constant
optimization are both
enabled, the accuracy
of MCS index
selection is affected,
which in turn affects
the performance of
CQI adjustment value
optimization.
Therefore, you are
advised not to enable
rank detection.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.27

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDownlink
intelligent
## JAMC
## CELL_DL_JOI
## NT_INTEL_A
## MC_SW
option of the
CellIntelAmc
## Config.
## Intelli
gentAmcSwit
ch parameter
Smart 8T8R
## (FDD)
If enhanced aperiodic
CQI reporting is
enabled and the
CellDlschAlgo.FDUEE
nhAperCQITrigPeriod
parameter is set to a
small value (for
example, 5 ms), the
baseline AMC
performance is good
due to frequent and
fast CQI reporting. In
this case, enabling
downlink intelligent
JAMC may not bring
significant gains.

## 4.3 Requirements
## 4.3.1 Licenses
The following are FDD license requirements:
Feature ID
Feature NameModelSales Unit
LCOFD-171301Precise Channel
## Measurement
LT1S00PCMFDDper cell

## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## RAT
## Function
## Name
## Function
## Switch
ReferenceDescription
## FDDNPREO
constant
optimization
CellDlpcPdsc
hPa.NomPdsc
hRsEpreOffse
t
## Channel State
## Management
CRS-IC-based UE
steering requires
NPREO constant
optimization.

eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.28

## Mutually Exclusive Functions
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDWTTx MU-
## MIMO
Tm9FourLaye
rPairSwitch
option of the
CellAlgoExtS
witch.WttxM
uMimoSwitc
h
parameter
WTTx MU-
## MIMO (FDD)
WTTx MU-MIMO
cannot work with the
CQI reporting interval
adaptation.

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
## FDD:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  BTS3912E
## ●  BTS3911E
## ●  BTS3203E
## ●  BTS3202E
## NO TE
Only 3900 and 5900 series base stations (macro base stations) support CQI adjustment
value optimization in NPREO constant optimization.
The following base stations do not support NPREO constant optimization:
## ●  BTS3203E
## ●  BTS3202E
The following base stations do not support configuration of the upper limit of UE-level
NPREO constant adjustment and periodic triggering of aperiodic CQI reporting for UEs
running downlink common large-packet services:
## ●  BTS3912E
## ●  BTS3911E
## ●  BTS3203E
## ●  BTS3202E
The following base stations do not support CRS-IC-based UE steering:
## ●  BTS3912E
## ●  BTS3911E
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.29

## Boards
For FDD:
●  NPREO constant optimization requires the LBBPd or UBBP boards. CQI
adjustment value optimization in this function requires the UBBP boards.
●  CRS-IC-based UE steering requires the LBBPd or UBBP boards.
●  Periodic triggering of aperiodic CQI reporting for UEs running downlink
common large-packet services is not supported by the LBBPc boards.
●  Other functions: no requirements
RF Modules
No requirements
## 4.3.4 Others
For FDD, cell-level NPREO constant optimization requires that counters related to
different NPREO constant values be collected. Therefore, it requires subscription to
hour-level or 30-minute network performance counters, such as L.thrp.bits.DL,
L.thrp.bits.DL.LastTTI, L.Thrp.Time.DL.RmvLastTTI, and
L.ChMeas.PRB.DL.Used.Avg.
4.4 Operation and Maintenance
4.4.1 Data Configuration (FDD)
## 4.4.1.1 Data Preparation
The periodic CQI reporting interval can be fixedly configured or adaptively
changed.
## Subfunction
Parameter NameParameter IDSetting Notes
## Adaptive
change
CQI Period
## Adaptive Switch
CellCqiAdaptiveC
fg.CqiPeriodAdap
tive
Set this parameter to
## ON.
Minimal CQI
## Period
CellCqiAdaptiveC
fg.MinCqiPeriod
The default value of
this parameter is
recommended.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.30

SubfunctionParameter NameParameter IDSetting Notes
## Fixed
configuration
User CQI periodCellCqiAdaptiveC
fg.UserCqiPeriod
This parameter is valid
only when the
CellCqiAdaptiveCfg.C
qiPeriodAdaptive
parameter is set to
## OFF.
The default value of
this parameter is
recommended.

The conditions for triggering aperiodic CQI reporting are different for UEs in
different states.
SubfunctionParameter
## Name
## Parameter
## ID
OptionSetting Notes
## Basic
configuration
## Aperiodic
CSI Uplink
## Transmit
## Mode
CellUlschA
lgo.Aperio
dicCsiUlTx
## Mode
NoneSet this parameter to
its recommended
value.
## PDCCH
## Symbol
## Number
## Adjust
## Switch
CellPdcchA
lgo.PdcchS
ymNumSw
itch
NoneRetain the default
value.
For UEs in FSS
mode
## FS UE
## Aperiodic
## CQI
## Triggering
## Period
CellDlschA
lgo.FSUEA
perCQITrig
## Period
NoneRetain the default
value.
## FS UE
## Aperiodic
## Subband
## CQI
## Validity
## Period
CellDlschA
lgo.FSUESb
CQIValidit
yPeriod
NoneRetain the default
value.
For UEs in
FDS mode
## DL
schedule
switch
CellAlgoS
witch.DlSc
hSwitch
EnAperiodi
cCqiRptSwi
tch
Select this option.
## FD UE
## Enhanced
## Aperiodic
CQI Trigger
## Period
CellDlschA
lgo.FDUEE
nhAperCQI
TrigPeriod
NoneRetain the default
value.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.31

SubfunctionParameter
## Name
## Parameter
## ID
OptionSetting Notes
## Downlink
## User Data
## Threshold
CellDlschA
lgo.DlUser
DataThld
NoneRetain the default
value.
## Aperiodic
CQI Trigger
UE Type
CellDlSchE
xtParam.A
periodicCqi
TrigUeType
NoneTo enable periodic
triggering of aperiodic
CQI reporting for UEs
running downlink
common large-packet
services, set this
parameter to
## COMMON_LARGE_PK
## T.

The following table describes the parameter related to optimized CQI detection.
## Parameter
## Name
Parameter IDOptionSetting Notes
## CQI
## Optimization
## Algorithm
## Switch
CellCqiAdjAlgo.C
qiOptSwitch
## PUSCH_CQI_FALS
## E_DETECTION_SW
## PUCCH_CQI_FALS
## E_DETECTION_SW
Set this parameter
based on live network
conditions.

The following table describes the parameters used for activating NPREO constant
optimization.
## Parameter
## Name
Parameter IDOptionSetting Notes
Cell-Level
## NPREO
## Adjustment
## Threshold
CellDlpcPdschPa.
CellNpreoAdjThr
eshold
NoneSet this parameter to
a value other than
- The value 5 is
recommended.
UE-Level
## NPREO
## Adjustment
## Threshold
CellDlpcPdschPa.
UeNpreoAdjThre
shold
NoneSet this parameter to
a value other than
- If the PCI mod 3
values are the same,
the value 10 is
recommended. If the
PCI mod 3 values are
different, the value 1
is recommended.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.32

## Parameter
## Name
Parameter IDOptionSetting Notes
UE-Level
## NPREO
## Adjustment
## Upper Limit
CellDlpcPdschPa.
UeNpreoAdjUppe
rLimit
NoneThe value 1 is
recommended when
the PCI mod 3 values
of adjacent cells are
different, while the
value 2 is
recommended when
the PCI mod 3 values
of adjacent cells are
the same.
UE-Level
## NPREO
## Adjustment
## Opt Switch
CellDlpcPdschPa.
UeNpreoAdjOptS
witch
CQI_ADJ_OPT_SWYou are advised to
select this option after
UE-level NPREO
constant optimization
is enabled.

The following table describes the parameters used for optimizing NPREO constant
optimization.
## Parameter
## Name
Parameter IDSetting Notes
## Interference
## Filter
## Coefficient
CellDlschAlgo.Int
rfFilterCoeff
The value 50 is recommended.
## DL RSRP
NCell
## Measurement
## A3 Offset
NCellDlRsrpMeas
Para.NCellDlRsrp
MeasA3Offset
The value -20 is recommended when
NPREO constant optimization is enabled.
## DL RSRP
NCell
## Measurement
## A6 Offset
NCellDlRsrpMeas
Para.DlRsrpNCell
MeasA6Offset
The value -20 is recommended when
NPREO constant optimization is enabled.

The following table describes the parameters used for activating CRS-IC-based UE
steering.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.33

## Parameter
## Name
Parameter IDOptionSetting Notes
## Handover
Mode switch
CellHoParaCfg.Ho
ModeSwitch
CrsIcHoSwitc
h
You are advised to select
this option when the
planned PCI mod 3
values of adjacent cells
are identical.
## Mobility
## Target
## Indicator
EutranInterNFreq.
MobilityTargetInd
CrsIcHoTarget
## Ind
Set this parameter based
on live network
conditions.

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
●Periodic CQI reporting
Adaptive change of periodic CQI reporting
//Configuring periodic CQI reporting
MOD CELLCQIADAPTIVECFG: LocalCellId=0, CqiPeriodAdaptive=ON, MinCqiPeriod=ms5;
Fixed configuration of periodic CQI reporting
//Configuring periodic CQI reporting
MOD CELLCQIADAPTIVECFG: LocalCellId=0, CqiPeriodAdaptive=OFF, UserCqiPeriod=ms40;
●Aperiodic CQI reporting
//Configuring the transmission mode of aperiodic CSI in the uplink
MOD CELLULSCHALGO: LocalCellId=0, AperiodicCsiUlTxMode=CsiOnly;
//Configuring the number of OFDM symbols occupied by the PDCCH
MOD CELLPDCCHALGO: LocalCellId=0, PdcchSymNumSwitch=ECFIADAPTIONON;
//Setting the triggering interval and validity period for UEs in FSS mode
MOD CELLDLSCHALGO: LocalCellId=0, FSUEAperCQITrigPeriod=2, FSUESbCQIValidityPeriod=10,
FDUEEnhAperCQITrigPeriod=5ms;
//Configuring aperiodic CQI reporting for UEs in FDS mode
MOD CELLALGOSWITCH: LocalCellId=0, DlSchSwitch=EnAperiodicCqiRptSwitch-1;
//Configuring periodic triggering of aperiodic CQI reporting for UEs running downlink common large-
packet services
MOD CELLDLSCHALGO: LocalCellId=0, DlUserDataThld=500;
MOD CELLDLSCHEXTPARAM: LocalCellId=0, AperiodicCqiTrigUeType=COMMON_LARGE_PKT;
●Optimized CQI detection
//Enabling optimized CQI detection
MOD CELLCQIADJALGO: LocalCellId=0,
CqiOptSwitch=PUSCH_CQI_FALSE_DETECTION_SW-1&PUCCH_CQI_FALSE_DETECTION_SW-1;
●NPREO constant optimization
//Enabling cell-level NPREO constant optimization
MOD CELLDLPCPDSCHPA: LocalCellId=101, CellNpreoAdjThreshold=5;
//Enabling the UE-level NPREO constant optimization function
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.34

MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjThreshold=1;
//Configuring the upper limit of UE-level NPREO constant adjustment
MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjUpperLimit=1;
//Enabling CQI adjustment value optimization in NPREO constant optimization
MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjOptSwitch=CQI_ADJ_OPT_SW-1;
●CRS-IC-based UE steering
//Enabling UEs that do not support CRS-IC in a cell working on a specific frequency to be handed over
to a cell not working on the specific frequency
MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjUpperLimit=2;
MOD CELLHOPARACFG: LocalCellId=101, HoModeSwitch=CrsIcHoSwitch-1;
//Enabling UEs that support CRS-IC to be retained in or handed over to a cell working on a specific
frequency
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=CrsIcHoSwitch-1;
MOD EUTRANINTERNFREQ: LocalCellId=0, DlEarfcn=1500, UlEarfcnCfgInd=CFG, UlEarfcn=19500,
MobilityTargetInd=CrsIcHoTargetInd-1;
## Optimization Command Examples
NPREO constant optimization
-  Set parameters.
//Setting the interference filtering coefficient
MOD CELLDLSCHALGO: LocalCellId=101, IntrfFilterCoeff=50;
//Adjusting the DL RSRP NCell Measurement A3 Offset parameter to increase the proportion of UEs
for which UE-level NPREO constant optimization takes effect
MOD NCELLDLRSRPMEASPARA: LocalCellId=101, NCellDlRsrpMeasA3Offset=-20;
//Adjusting the DL RSRP NCell Measurement A6 Offset parameter to increase the proportion of UEs
for which UE-level NPREO constant optimization takes effect
MOD NCELLDLRSRPMEASPARA: LocalCellId=101, DlRsrpNCellMeasA6Offset=-20;
-  Set up an eX2 interface between base stations. For detailed operations, see
eX2 Self-Management. Configure an X2 interface (service coordination must
be supported in non-ideal backhaul mode). For detailed operations, see
## S1
and X2 Self-Management.
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
●Aperiodic CQI reporting
//Disabling periodic triggering of aperiodic CQI reporting for UEs running downlink common large-
packet services
MOD CELLDLSCHEXTPARAM: LocalCellId=0, AperiodicCqiTrigUeType=NULL;
●Optimized CQI detection
//Disabling optimized CQI detection
MOD CELLCQIADJALGO: LocalCellId=0,
CqiOptSwitch=PUSCH_CQI_FALSE_DETECTION_SW-0&PUCCH_CQI_FALSE_DETECTION_SW-0;
●NPREO constant optimization
//Disabling CQI adjustment value optimization in NPREO constant optimization
MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjOptSwitch=CQI_ADJ_OPT_SW-0;
//Disabling UE-level NPREO constant optimization
MOD CELLDLPCPDSCHPA: LocalCellId=101, UeNpreoAdjThreshold=127;
//Disabling cell-level NPREO constant optimization and restoring the NPREO constant to the expected
value
MOD CELLDLPCPDSCHPA: LocalCellId=101, CellNpreoAdjThreshold=255;
MOD CELLDLPCPDSCHPA: LocalCellId=101, NomPdschRsEpreOffset=0;
●CRS-IC-based UE steering
//Disabling CRS-IC-based UE steering
MOD CELLHOPARACFG: LocalCellId=101, HoModeSwitch=CrsIcHoSwitch-0;
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=CrsIcHoSwitch-0;
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.35

4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
CSI Reporting Mode
If the CQI-ReportModeAperiodic IE contains rmXY in the RRC_CONN_SETUP
message traced on the Uu interface, CSI reporting mode X-Y has taken effect.
Periodic CQI Reporting
Verify whether optimized periodic CQI reporting on the PUCCH has taken effect by
performing the following steps:
Step 1Enable 10 UEs to access the cell and perform ping services.
Step 2Disable optimized periodic CQI reporting on the PUCCH. Then, enable a UE to
access the cell. Query the cqi-pmi-ConfigIndex value in the RRC_CONN_RECFG
message traced over the Uu interface, as shown in Figure 4-3. The value indicates
that the CQI reporting interval is 5 ms.
Figure 4-3 CQI reporting interval of 5 ms
Step 3Release the UE that accessed the cell in Step 2. Enable optimized periodic CQI
reporting on the PUCCH. Then, enable a UE to access the cell again. Query the
cqi-pmi-ConfigIndex value in the RRC_CONN_RECFG message traced over the Uu
interface, as shown in Figure 4-4. The value indicates that the CQI reporting
interval is 40 ms.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.36

Figure 4-4 CQI reporting interval of 40 ms
----End
Aperiodic CQI Reporting
Aperiodic CQI reporting has taken effect if the value of any of the counters listed
in Table 4-1 increases significantly after aperiodic CQI reporting is triggered.
Table 4-1 Counters related to aperiodic CQI reporting
Counter ID
## Counter Name
1526729367 through
## 1526729382
L.ChMeas.CQI.DL.DualCW.Code0.Aperiodic.0
through
L.ChMeas.CQI.DL.DualCW.Code0.Aperiodic.15
1526729399 through
## 1526729414
L.ChMeas.CQI.DL.DualCW.Code1.Aperiodic.0
through
L.ChMeas.CQI.DL.DualCW.Code1.Aperiodic.15
1526729335 through
## 1526729350
L.ChMeas.CQI.DL.SingleCW.Aperiodic.0 through
L.ChMeas.CQI.DL.SingleCW.Aperiodic.15

NPREO Constant Optimization (FDD)
●  Using MML commands
Run the DSP CELLNPREOOPTIMIZESTATUS command to query the running
status of the cell-level NPREO constant optimization function. If the query
result shows that the function is running, the function has taken effect.
●  Using signaling tracing
After UE-level NPREO constant optimization is enabled, it will adjust the
NPREO constants of UEs. Check the value of nomPDSCH-RS-EPRE-Offset in
the CQI-ReportConfig IE of the RRC Connection Reconfiguration message. If
the value is not equal to that configured in the MML command window, the
function has taken effect. In addition, after UE-level NPREO constant
optimization is enabled, you can check cell indicators such as the proportion
of high ranks, average CQI, and average MCS index. If the values significantly
fluctuate or change, the function has taken effect.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.37

CRS-IC-based UE Steering (FDD)
After CRS-IC-based UE steering is enabled, if the eNodeB triggers a handover of a
UE in a cell working on a specific frequency to a cell not working on the specific
frequency and any of the following conditions is met, this function has taken
effect.
●  In the reported UE-EUTRA-Capability IE, the value of crs-InterfHandl-r11 in
UE-EUTRA-Capability-v920-IEs is not supported.
●  The UE complies with 3GPP Release 11 or later.
## 4.4.3 Network Monitoring
After periodic CQI reporting, aperiodic CQI reporting, and optimized CQI detection
are enabled, the User Downlink Average Throughput increases but the User
Uplink Average Throughput decreases.
For FDD, after NPREO constant optimization is enabled, the User Downlink
Average Throughput increases.
User Uplink Average Throughput = (L.Thrp.bits.UL –
L.Thrp.bits.UE.UL.LastTTI)/L.Thrp.Time.UE.UL.RmvLastTTI
User Downlink Average Throughput = (L.Thrp.bits.DL – L.Thrp.bits.DL.LastTTI)/
L.Thrp.Time.DL.RmvLastTTI
For FDD, after CRS-IC-based UE steering is enabled, the Intra-Frequency
Handover Out Success Rate increases and the Call Drop Rate (VoIP) decreases.
For FDD, check the cell-level downlink rank distribution, CQI distribution, MCS
index distribution, average CQI, average MCS index, PDSCH IBLER, and PDSCH
RBLER to see their changes.
Average periodic CQI = (L.ChMeas.CQI.DL.1 + 2 x L.ChMeas.CQI.DL.2 + 3 x
L.ChMeas.CQI.DL.3 + ... + 15 x L.ChMeas.CQI.DL.15)/(L.ChMeas.CQI.DL.0 +
L.ChMeas.CQI.DL.1 + L.ChMeas.CQI.DL.2 +...+ L.ChMeas.CQI.DL.15)
Average MCS = (L.ChMeas.PDSCH.MCS.1 + 2 x L.ChMeas.PDSCH.MCS.2 + 3 x
L.ChMeas.PDSCH.MCS.3 + ... + 28 x L.ChMeas.PDSCH.MCS.28)/
(L.ChMeas.PDSCH.MCS.0 + L.ChMeas.PDSCH.MCS.1 + L.ChMeas.PDSCH.MCS.2
+...+ L.ChMeas.PDSCH.MCS.28)
PDSCH IBLER = (L.Traffic.DL.SCH.QPSK.ErrTB.Ibler +
L.Traffic.DL.SCH.16QAM.ErrTB.Ibler + L.Traffic.DL.SCH.64QAM.ErrTB.Ibler +
L.Traffic.DL.SCH.256QAM.ErrTB.Ibler)/(L.Traffic.DL.SCH.QPSK.TB +
L.Traffic.DL.SCH.16QAM.TB + L.Traffic.DL.SCH.64QAM.TB +
L.Traffic.DL.SCH.256QAM.TB) x 100%
PDSCH RBLER = (L.Traffic.DL.SCH.QPSK.ErrTB.Rbler +
L.Traffic.DL.SCH.16QAM.ErrTB.Rbler + L.Traffic.DL.SCH.64QAM.ErrTB.Rbler +
L.Traffic.DL.SCH.256QAM.ErrTB.Rbler)/(L.Traffic.DL.SCH.QPSK.TB +
L.Traffic.DL.SCH.16QAM.TB + L.Traffic.DL.SCH.64QAM.TB+
L.Traffic.DL.SCH.256QAM.TB) x 100%
Table 4-2 lists the related counters.
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.38

Table 4-2 Counters related to network monitoring
Counter IDCounter Name
1526728261L.Thrp.bits.DL
1526729005L.Thrp.bits.DL.LastTTI
1526729015L.Thrp.Time.DL.RmvLastTTI
1526728180L.Traffic.DL.SCH.QPSK.ErrTB.Ibler
1526728182L.Traffic.DL.SCH.16QAM.ErrTB.Ibler
1526728184L.Traffic.DL.SCH.64QAM.ErrTB.Ibler
1526739660L.Traffic.DL.SCH.256QAM.ErrTB.Ibler
1526727354L.Traffic.DL.SCH.QPSK.TB
1526727355L.Traffic.DL.SCH.16QAM.TB
1526727356L.Traffic.DL.SCH.64QAM.TB
1526739656L.Traffic.DL.SCH.256QAM.TB
1526728181L.Traffic.DL.SCH.QPSK.ErrTB.Rbler
1526728183L.Traffic.DL.SCH.16QAM.ErrTB.Rbler
1526728185L.Traffic.DL.SCH.64QAM.ErrTB.Rbler
1526739661L.Traffic.DL.SCH.256QAM.ErrTB.Rbler
1526730141L.ChMeas.RI.Rank1
1526730142L.ChMeas.RI.Rank2
1526732737L.ChMeas.RI.Rank3
1526732738L.ChMeas.RI.Rank4
1526746770L.ChMeas.RI.Rank5
1526746771L.ChMeas.RI.Rank6
1526746772L.ChMeas.RI.Rank7
1526746773L.ChMeas.RI.Rank8
1526727396 through
## 1526727411
L.ChMeas.CQI.DL.0 through L.ChMeas.CQI.DL.15
1526727444 through
## 1526727472
L.ChMeas.PDSCH.MCS.0 through
L.ChMeas.PDSCH.MCS.28
eRAN
## Channel State Management Feature Parameter
Description4 CQI Reporting
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.39

5 CQI Reporting Optimization
## 5.1 Principles
Huawei eNodeBs optimize CQI reporting for flexible control.
5.1.1 Periodic CQI Reporting Optimization
When the CellCqiAdaptiveCfg.CqiPeriodAdaptive parameter is set to ON to
adjust the periodic CQI reporting interval based on the PUCCH load, further
optimizations can be made using the following parameters.
In FDD, the base station can optimize the CQI reporting interval using the
CqiAdaptiveCfg.
PucchPeriodicCqiOptSwitch parameter to increase the number
of UEs that report CQIs at long intervals.
●  If this parameter is set to ON, more UEs report CQIs at long intervals, fewer
RBs are allocated to the PUCCH, and more RBs can be allocated to the PUSCH
to increase uplink throughput. However, the UEs do not promptly report
channel quality and downlink performance may deteriorate.
●  If this parameter is set to OFF, more UEs report CQIs at short intervals, the
UEs promptly report channel quality, and downlink performance may improve.
However, the uplink peak rate may be lower than that obtained when this
parameter is set to ON.
The base station can optimize the CQI reporting interval for CA UEs using the
CA_CQI_PERIOD_OPT_SW option of the CellCqiAdaptiveCfg.
CellCqiAlgoSwitch
parameter to reduce the probability of periodic CQI reporting conflicts for CA UEs.
●  If this option is selected, the base station considers both the number of uplink
carriers configured with SRS resources and the number of downlink carriers
when configuring the CQI reporting interval for CA UEs. This ensures that the
periodic CQI reporting time for all carriers does not conflict with each other.
●  If this option is deselected, the base station considers only the number of
downlink carriers but not the number of uplink carriers configured with SRS
resources when configuring the CQI reporting interval for CA UEs. In this case,
the CQI reporting interval may be excessively short and the CQI reporting
time for some carriers will conflict. As a result, the corresponding CQI reports
cannot be sent.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.40

5.1.2 Aperiodic CQI Reporting Optimization
The triggering of aperiodic CQI reporting is optimized for UEs in the initial access,
UEs involved in handovers, and UEs with compatibility issues.
5.1.2.1 UEs in the Initial Access
During the initial access, if periodic CQI reporting fails repeatedly, aperiodic CQI
reporting is triggered. If the aperiodic CQI reporting fails a cyclic redundancy code
(CRC) check, the aperiodic CQI reporting is triggered again eight transmission time
intervals (TTIs) later.
Aperiodic CQI reporting scheduled in CQI-only mode occupies PUSCH and PDCCH
resources. To reduce the chance that aperiodic CQI reporting is triggered during
initial access, Huawei eNodeBs support optimized aperiodic CQI reporting
triggering. For details about CQI-only mode, see
## Scheduling.
Optimized aperiodic CQI reporting triggering is controlled by the
AperiodicCqiTrigOptSwitch option of the CellAlgoSwitch.
DlSchSwitch
parameter. When this option is selected and an aperiodically reported CQI fails a
CRC check, the eNodeB determines whether to trigger aperiodic CQI reporting
again based on the DRX switch setting (specified by the
CellDrxPara.
DrxAlgSwitch parameter):
●  If the DRX switch is turned on, aperiodic CQI reporting is not triggered again.
●  If the DRX switch is turned off, aperiodic CQI reporting is triggered after eight
TTIs.
5.1.2.2 UEs Involved in Handovers
Aperiodic CQI reporting can be configured in handover commands for UEs
involved in handovers. If there are downlink services for a UE after the handover,
aperiodic CQI reporting is triggered once. This function is controlled by
CellCqiAdaptiveCfg.
HoAperiodicCqiCfgSwitch:
●  If this switch is turned on, aperiodic CQI reporting is configured in handover
commands. When there are downlink services for UEs after handovers,
aperiodic CQI reporting is triggered if no periodic CQI resources are
configured for the UEs, thereby increasing downlink throughput. However, the
high handover signaling overhead may decrease the handover success rate
and increase handover delay.
●  If this switch is turned off, aperiodic CQI reporting is not configured in
handover commands. Instead, it is configured only after handovers.
5.1.2.3 UEs with Compatibility Issues
ACK/NACK Issues
Some UEs have compatibility issues with CQI reporting. When aperiodic CQI
reports are sent in CQI-only mode at the same time as ACK/NACK responses,
some UEs do not calculate the number of required subcarriers in line with 3GPP
specifications. As a result, the eNodeB ACK/NACK demodulation fails, which may
lead to a loss in downlink throughput.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.41

This issue can be addressed by selecting the ApCqiAndAckAbnCtrlSwitch option
of the ENodeBAlgoSwitch.CompatibilityCtrlSwitch parameter.
●  If this option is selected, the aperiodically reported CQIs are only scheduled in
preallocation mode.
●  If this option is deselected, the aperiodically reported CQIs are only scheduled
in CQI-only mode.
No Aperiodic CQI Reporting in SCells
In carrier aggregation (CA) scenarios, if a reconfiguration message does not
contain aperiodic CQI reporting data, some CA UEs will not send aperiodic CQI
reports in the secondary cells (SCells). This will lead to mis-demodulation by
eNodeBs, affecting downlink performance and even deactivating SCells.
This issue can be addressed by selecting the ApCqiRptAbnormalCtrlSwitch
option of the ENodeBAlgoSwitch.
CompatibilityCtrlSwitch parameter.
●  If this option is selected, each reconfiguration message sent to the UE will
carry aperiodic CQI reporting data.
●  If this option is deselected, the reconfiguration message carries aperiodic CQI
reporting data when configurations for aperiodic CQI reporting are changed.
In non-CA scenarios, it is recommended that this option be deselected. If this
option is selected, the RRC signaling overhead increases and the cell capacity
decreases.
## 5.2 Network Analysis
## 5.2.1 Benefits
Periodic CQI reporting optimization offers the following benefits:
In FDD, setting the CqiAdaptiveCfg.
PucchPeriodicCqiOptSwitch parameter to
ON increases the number of UEs that report CQIs at long intervals, reduces
PUCCH resource consumption, and increases uplink throughput.
Selecting the CA_CQI_PERIOD_OPT_SW option of the
CellCqiAdaptiveCfg.
CellCqiAlgoSwitch parameter ensures that the periodic CQI
reporting time for all carriers of a CA UE does not conflict.
Aperiodic CQI reporting optimization offers the following benefits:
●  Reduces PUSCH and PDCCH resource consumption by decreasing the number
of times aperiodic CQI reporting is triggered during the initial access.
●  Increases downlink throughput by configuring aperiodic CQI reporting in a
handover command and triggering aperiodic CQI reporting for a single time
once the handover is completed and there is a downlink service. However, the
high handover signaling overhead may decrease the handover success rate
and increase handover delay.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.42

## 5.2.2 Impacts
## Network Impacts
In FDD, setting the CqiAdaptiveCfg.PucchPeriodicCqiOptSwitch parameter to
ON increases the number of UEs that report CQIs at long intervals and therefore
increases uplink throughput. However, UEs do not promptly report channel quality
and therefore downlink performance may deteriorate.
## Function Impacts
## None
## 5.3 Requirements
## 5.3.1 Licenses
## None
## 5.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## None
## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
## FDD:
●  3900 and 5900 series base stations (macro base stations)
## ●  BTS3912E
## ●  BTS3911E
## ●  BTS3203E
## ●  BTS3202E
## Boards
No requirements
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.43

RF Modules
No requirements
## 5.3.4 Others
## None
5.4 Operation and Maintenance
5.4.1 Data Configuration (FDD)
## 5.4.1.1 Data Preparation
The following table describes the parameter related to periodic CQI reporting
optimization.
SubfunctionParameter
## Name
Parameter IDSetting Notes
## Adaptive
change
## PUCCH
Periodic CQI
## Optimize
## Switch
CqiAdaptiveCfg.Pucc
hPeriodicCqiOptS-
witch
The default value of
this parameter is
recommended.
Cell CQI
## Algorithm
## Switch
## CA_CQI_PERIOD_OP
T_SW option of the
CellCqiAdaptiveCfg.
CellCqiAlgoSwitch
parameter
Select this option.

The conditions for triggering aperiodic CQI reporting are different for UEs in
different states.
## Subfunction
## Parameter
## Name
## Parameter
## ID
OptionSetting Notes
For UEs in the
initial access
## DL
schedule
switch
CellAlgoS
witch.DlSc
hSwitch
AperiodicC
qiTrigOptS
witch
Select this option.
For UEs
involved in
handovers
## Handover
## Aperiodic
CQI Config
## Switch
CellCqiAda
ptiveCfg.H
oAperiodic
CqiCfgSwit
ch
NoneThe default value of
this parameter is
recommended.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.44

SubfunctionParameter
## Name
## Parameter
## ID
OptionSetting Notes
For UEs with
compatibility
issues
## Compatibili
ty Control
## Switch
ENodeBAlg
oSwitch.Co
mpatibility
CtrlSwitch
ApCqiAnd
AckAbnCtr
lSwitch
ApCqiRptA
bnormalCt
rlSwitch
Set this parameter
based on live network
conditions.

5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
●Periodic CQI reporting optimization
//Configuring periodic CQI reporting optimization
MOD CQIADAPTIVECFG: PucchPeriodicCqiOptSwitch=ON;
//Configuring periodic CQI reporting optimization for CA UEs
MOD CELLCQIADAPTIVECFG: LocalCellId=0, CellCqiAlgoSwitch=CA_CQI_PERIOD_OPT_SW-1;
●Aperiodic CQI reporting optimization
//Configuring aperiodic CQI reporting for UEs in the initial access
MOD CELLALGOSWITCH: LocalCellId=0, DlSchSwitch=AperiodicCqiTrigOptSwitch-1;
//Configuring aperiodic CQI reporting for UEs involved in handovers
MOD CELLCQIADAPTIVECFG: LocalCellId=0, HoAperiodicCqiCfgSwitch=ON;
//Configuring aperiodic CQI reporting for UEs with compatibility issues
MOD ENODEBALGOSWITCH: CompatibilityCtrlSwitch=ApCqiAndAckAbnCtrlSwitch-1;
//Configuring aperiodic CQI reporting for CA UEs with compatibility issues
MOD ENODEBALGOSWITCH: CompatibilityCtrlSwitch=ApCqiRptAbnormalCtrlSwitch-1;
## Deactivation Command Examples
●Periodic CQI reporting optimization
//Disabling periodic CQI reporting optimization
MOD CQIADAPTIVECFG: PucchPeriodicCqiOptSwitch=OFF;
//Disabling periodic CQI reporting optimization for CA UEs
MOD CELLCQIADAPTIVECFG: LocalCellId=0, CellCqiAlgoSwitch=CA_CQI_PERIOD_OPT_SW-0;
●Aperiodic CQI reporting optimization
//Disabling aperiodic CQI reporting for UEs in the initial access
MOD CELLALGOSWITCH: LocalCellId=0, DlSchSwitch=AperiodicCqiTrigOptSwitch-0;
//Disabling aperiodic CQI reporting for UEs involved in handovers
MOD CELLCQIADAPTIVECFG: LocalCellId=0, HoAperiodicCqiCfgSwitch=OFF;
//Disabling aperiodic CQI reporting for UEs with compatibility issues
MOD ENODEBALGOSWITCH: CompatibilityCtrlSwitch=ApCqiAndAckAbnCtrlSwitch-0;
//Disabling aperiodic CQI reporting for CA UEs with compatibility issues
MOD ENODEBALGOSWITCH: CompatibilityCtrlSwitch=ApCqiRptAbnormalCtrlSwitch-0;
5.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.45

## 5.4.2 Activation Verification
CSI Reporting Mode
If the CQI-ReportModeAperiodic IE contains rmXY in the RRC_CONN_SETUP
message traced on the Uu interface, CSI reporting mode X-Y has taken effect.
Periodic CQI Reporting Optimization
Verify whether optimized periodic CQI reporting on the PUCCH has taken effect by
performing the following steps:
Step 1Enable 10 UEs to access the cell and perform ping services.
Step 2Disable optimized periodic CQI reporting on the PUCCH. Then, enable a UE to
access the cell. Query the cqi-pmi-ConfigIndex value in the RRC_CONN_RECFG
message traced over the Uu interface, as shown in Figure 5-1. The value indicates
that the CQI reporting interval is 5 ms.
Figure 5-1 CQI reporting interval of 5 ms
Step 3Release the UE that accessed the cell in Step 2. Enable optimized periodic CQI
reporting on the PUCCH. Then, enable a UE to access the cell again. Query the
cqi-pmi-ConfigIndex value in the RRC_CONN_RECFG message traced over the Uu
interface, as shown in Figure 5-2. The value indicates that the CQI reporting
interval is 40 ms.
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.46

Figure 5-2 CQI reporting interval of 40 ms
----End
Periodic CQI Reporting Optimization for CA UEs
Verify whether periodic CQI reporting optimization for CA UEs has taken effect by
performing the following steps:
Step 1In intra-BBU FDD+TDD DL 5CC+UL 2CC CA scenarios, configure an FDD carrier as
the PCC and enable SRS transmission on the two uplink SCCs.
Step 2Deselect the CA_CQI_PERIOD_OPT_SW option of the
CellCqiAdaptiveCfg.
CellCqiAlgoSwitch parameter. Then, enable a 5CC-capable
UE to access the network and perform downlink large-packet services. Query the
cqi-pmi-ConfigIndex value in the RRC_CONN_RECFG message traced over the Uu
interface. The value indicates that the CQI reporting interval is 5 ms.
Step 3Release the UE that accessed the cell in Step 2. Select the
CA_CQI_PERIOD_OPT_SW option of the CellCqiAdaptiveCfg.
CellCqiAlgoSwitch
parameter. Then, enable a 5CC-capable UE to access the network again and
perform downlink large-packet services. Query the cqi-pmi-ConfigIndex value in
the RRC_CONN_RECFG message traced over the Uu interface. The value indicates
that the CQI reporting interval is 10 ms.
----End
Aperiodic CQI Reporting
Optimized aperiodic CQI reporting triggering has taken effect if the value of the
counter listed in Table 5-1 decreases after both optimized aperiodic CQI reporting
triggering and DRX are enabled.
Table 5-1 Counter related to optimized aperiodic CQI reporting triggering
Counter ID
## Counter Name
1526727441L.ChMeas.PUSCH.MCS.29

eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.47

## 5.4.3 Network Monitoring
After CQI reporting optimization is enabled, the User Downlink Average
Throughput increases but the User Uplink Average Throughput decreases.
User Uplink Average Throughput = (L.Thrp.bits.UL –
L.Thrp.bits.UE.UL.LastTTI)/L.Thrp.Time.UE.UL.RmvLastTTI
User Downlink Average Throughput = (L.Thrp.bits.DL – L.Thrp.bits.DL.LastTTI)/
L.Thrp.Time.DL.RmvLastTTI
eRAN
## Channel State Management Feature Parameter
Description5 CQI Reporting Optimization
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.48

6 CQI Adjustment
## 6.1 Principles
The CQI reporting may be delayed, and the CQI reporting interval significantly
exceeds the scheduling period. As a result, the reported CQI may not reflect the
channel quality and IBLER will be unable to approach the target optimum value.
In such a case, the eNodeB must calculate the difference between the reported
channel quality and the actual channel quality, based on HARQ feedback, and
adjust the CQI accordingly.
CQI adjustment is controlled by the CqiAdjAlgoSwitch option of the
CellAlgoSwitch.
CqiAdjAlgoSwitch parameter. If this option is selected, the
eNodeB selects an MCS based on the adjusted CQI.
●  If the selected MCS requires better channel quality than is available, the block
error rate (BLER) for data packets increases. The eNodeB then decreases the
CQI based on the feedback from the UE.
●  If the current channel quality is better than that required by the selected MCS,
the BLER for data packets decreases. The eNodeB reacts by increasing the CQI
based on the feedback from the UE.
CQI adjustment enables the downlink IBLER to close in on a predefined target
value. The target IBLER determines the CQI adjustment value.
6.1.1 Downlink Target IBLER
## 6.1.1.1 Fixed Configuration
The downlink target IBLER for a UE depends on the downlink target IBLERs
corresponding to the bearers of the QCIs set up for the UE, as shown in Table 6-1.
The target IBLER corresponding to a bearer of a QCI set up for the UE is
determined by the CellQciPara.
InitDlTargetIbler parameter. If this parameter
value is changed, the specified target IBLER takes effect only when a bearer of a
QCI is created, modified, or released for the admitted UE.
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.49

Table 6-1 Target IBLERs for a UE
Target IBLERs Corresponding to
Bearers of the QCIs Set Up for the
## UE
Target IBLER for the UE
All the target IBLER values are zero.The target IBLER is determined by the
CellCqiAdjAlgo.InitDlIblerTarget
parameter.
Only one of the target IBLER values is
non-zero.
The target IBLER is the non-zero target
IBLER value.
More than one of the target IBLER
values are non-zero.
A non-zero parameter value with the
QCI that takes precedence over the
other QCIs is used as the target IBLER
for the UE. The QCIs in descending
order of precedence are as follows: QCI
2, QCI 1, QCIs for non-IMS signaling,
and QCIs for IMS signaling.
There are multiple QCIs for non-IMS
signaling.
The target IBLER depends on the QCI
that takes precedence over the other
QCIs. The QCIs are sorted in
descending order of QCI priority.
Multiple QCIs have the same priority
but correspond to different target
IBLER values.
The smallest target IBLER value is
used.

## 6.1.1.2 Adaptive Configuration
The downlink target IBLER can be configured both fixedly and adaptively. Adaptive
configuration of the target IBLER does not apply to UEs running services with QCI
## 1.
## Adaptation
For FDD, downlink target IBLER adaptation is controlled by the
DlVarIBLERtargetSwitch option of the CellAlgoSwitch.CqiAdjAlgoSwitch
parameter. If this option is selected, the eNodeB adjusts the target IBLER to:
●  10% for UEs running non-small-packet services at non-edge locations.
●  30% for UEs running small-packet services at non-edge locations and UEs at
cell edges.
## Enhanced Adaptation
Enhanced downlink target IBLER adaptation is controlled by the
DlEnVarIblerTargetSwitch option of the CellAlgoSwitch.CqiAdjAlgoSwitch
parameter. If this option is selected, the eNodeB adjusts the target IBLER based on
the TBS index threshold for low target IBLER specified by the
CellDlschAlgo.
LowIblerTargetTbsIdxThld parameter.
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.50

When the TBS index threshold for low target IBLER is 255, the eNodeB does not
adjust the target IBLER based on the TBS index.
●  For UEs performing services with slightly fluctuated CQI values, the target
IBLER is changed to 5%.
●  For UEs performing services with moderately fluctuated CQI values, the target
IBLER is determined as if the DlVarIBLERtargetSwitch option of the
CellAlgoSwitch.CqiAdjAlgoSwitch parameter is selected.
●  For UEs performing services with heavily fluctuated CQI values, the target
IBLER is changed to 30%.
When the TBS index threshold for low target IBLER is not 255, the eNodeB adjusts
the target IBLER based on the TBS index.
●  For UEs performing services with slightly fluctuated CQI values,
–   If the TBS index is not less than the value of the
CellDlschAlgo.
LowIblerTargetTbsIdxThld parameter, the target IBLER is
changed to 5%.
–   If the TBS index is less than the value of the
CellDlschAlgo.LowIblerTargetTbsIdxThld parameter, the target IBLER is
changed to 10%.
●  For UEs performing services with heavily fluctuated CQI values,
–   If the TBS index does not exceed the value of the
CellDlschAlgo.
HighIblerTargetTbsIdxThld parameter, the target IBLER is
changed to 30%.
–   If the TBS index exceeds the value of the
CellDlschAlgo.
HighIblerTargetTbsIdxThld parameter, the target IBLER is
changed to 10%.
●  For UEs performing services with moderately fluctuated CQI values,
The target IBLER is determined as if the DlVarIBLERtargetSwitch option of
the CellAlgoSwitch.CqiAdjAlgoSwitch parameter is selected.
## NO TE
If both the DlVarIBLERtargetSwitch and DlEnVarIblerTargetSwitch options of the
CellAlgoSwitch.CqiAdjAlgoSwitch parameter are selected, the target IBLER is determined
by the DlEnVarIblerTargetSwitch option of the CellAlgoSwitch.CqiAdjAlgoSwitch
parameter.
6.1.2 CQI Adjustment Period (FDD)
In FDD, if a cell serves a large number of online users, the CQI adjustment period
is prolonged and the CQI adjustment algorithm may receive multiple HARQ
feedback messages in a CQI adjustment period.
The DlCqiAdjDeltaOptSwitch option of the CellAlgoSwitch.
CqiAdjAlgoSwitch
parameter specifies how to calculate the CQI adjustment value.
●  When this option is deselected, the CQI adjustment algorithm treats all the
received HARQ feedback messages in a CQI adjustment period as a single
feedback message, based on which the CQI adjustment value is calculated.
This calculation method causes slow CQI adjustment.
●  When this option is selected, the CQI adjustment algorithm calculates the CQI
adjustment value based on each individual HARQ feedback message received
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.51

in a CQI adjustment period. This calculation method causes fast CQI
adjustment.
6.1.3 CQI Filtering Adjustment
6.1.3.1 Initial Filtered Value of Reported CQIs
The eNodeB applies filtering to the reported CQIs. The initial filtered value of the
CQIs reported by a newly admitted UE is determined by the RptCqiFltInitSwitch
option of the CellAlgoSwitch.
CqiAdjAlgoSwitch parameter. This function does
not take effect for UEs running services with QCI 1.
●  If this option is deselected, the initial filtered value is always 4.
●  If this option is selected, the initial filtered value is adaptively configured
based on the reported CQIs, which can increase the User Downlink Average
## Throughput.
6.1.3.2 CQI Filtering Based on Spectral Efficiency Optimization
This function is controlled by the CqiFltSpectralEffOptSwitch option of the
CellAlgoSwitch.
CqiAdjAlgoSwitch parameter. In FDD, it takes effect for TM4 UEs.
●  If this option is deselected, each time the eNodeB receives a CQI value from a
UE, it directly applies filtering to the reported CQI and the previous filtered
## CQI.
●  If this option is selected, each time the eNodeB receives a CQI value from a
UE, it determines the difference between the reported CQI and the previous
filtered CQI. If the difference is large, the eNodeB adjusts the reported CQI
based on spectral efficiency optimization, and then applies filtering to the
adjusted CQI and the previous filtered CQI. If the difference is small, the
eNodeB directly applies filtering to the reported CQI and the previous filtered
## CQI.
6.1.4 Optimized CQI Adjustment Value (FDD)
An eNodeB calculates a CQI adjustment value for a UE based on HARQ feedback.
It sets an initial value for the UE during initial access, RRC connection
reestablishment, or incoming handovers. The larger the CQI adjustment value, the
more aggressive the MCS for the UE. The smaller the CQI adjustment value, the
more conservative the MCS for the UE.
6.1.4.1 Initial CQI Adjustment Value (FDD)
In FDD, the initial CQI adjustment value for UEs during initial access, RRC
connection reestablishment, or incoming handovers is specified by the
CellCqiAdjAlgo.
InitDeltaCqi parameter.
The PreciseMcsAdaptSwitch option of the CellAlgoSwitch.CqiAdjAlgoSwitch
parameter determines whether the eNodeB modifies the reported CQI value for
the UEs. If this option is selected, the eNodeB:
●Modifies the reported CQI value if the CellCqiAdjAlgo.
InitDeltaCqi
parameter is set to a value smaller than –1 and the UE reports consecutive
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.52

ACKs as feedback on downlink HARQ. This function does not take effect for
UEs running services with QCI 1.
●  Increases the TBS index used for the first downlink HARQ retransmission. The
increased amount is specified by the CellDlschAlgo.DlFirstHarqTxTbsIncNum
parameter.
6.1.4.2 CQI Adjustment Step (FDD)
The CQI adjustment step can be fixed, variable, or adaptively variable. The eNodeB
can fix the CQI adjustment step to the CellCqiAdjAlgo.CqiAdjStep parameter
value.
The CQI adjustment step for UEs during initial access or incoming handovers can
be fixed to the CellDlschAlgo.
CqiAdjInitialStep parameter value.
Variable-Step-based CQI Adjustment
This function is controlled by the StepVarySwitch option of the
CellAlgoSwitch.
CqiAdjAlgoSwitch parameter.
If this option is selected, the eNodeB determines the CQI adjustment step based
on how likely the UE is to be scheduled in the downlink within the next 100 ms.
●  UE is less than 10% likely to be scheduled.
This means that the UE is not accessing many downlink services. The CQI
adjustment step is adjusted based on how far the IBLER is from its configured
target. The farther the IBLER is from the target IBLER, the larger the
adjustment step is, which helps the IBLER more rapidly approach the target
## IBLER.
●  UE is at least 10% likely to be scheduled.
This means that the UE is accessing many downlink services. The CQI
adjustment step is fixed to the value of the CellCqiAdjAlgo.
CqiAdjStep
parameter.
Adaptive Variable-Step-based CQI Adjustment
This function takes effect when the AdaptiveStepVarySwitch option of the
CellAlgoSwitch.CqiAdjAlgoSwitch parameter is selected and the
CellCqiAdjAlgo.
CqiAdjStep parameter value is used as the CQI adjustment step.
If this option is selected, the eNodeB adjusts the CQI adjustment step based on
the HARQ feedback for downlink transmissions. This function does not take effect
for UEs running services with QCI 1.
●  If the eNodeB consistently receives HARQ ACKs for downlink transmissions, it
increases the CQI by a large step.
●  If the eNodeB consistently receives HARQ NACKs for downlink transmissions,
it decreases the CQI by a large step.
## 6.2 Network Analysis
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.53

## 6.2.1 Benefits
Downlink CQI adjustment, using a closed-loop mechanism to dynamically
compensate for inaccurate CQIs reported by UEs, optimizes MCS selection and
increases cell throughput.
If the network has moderate or heavy loads in the downlink (for example, the
downlink PRB usage is greater than 20%) and the proportion of rank 2 and above
exceeds 40%, the downlink user-perceived rate will increase by 1% to 3% after
CQI filtering based on spectral efficiency optimization takes effect.
## 6.2.2 Impacts
## Network Impacts
In massive MIMO scenarios, enhanced downlink target IBLER adaptation decreases
the average MCS index, spectral efficiency, and average cell throughput in the
downlink when most UEs in the cell are near the cell center and when wireless to
the x (WTTx) is used or there is little interference. Therefore, enhanced downlink
target IBLER adaptation is not recommended in the preceding massive MIMO
scenarios.
## Function Impacts
## RAT
## Function
## Name
## Function
## Switch
ReferenceDescription
FDDShort TTISHORT_TTI_S
W option of
the
CellShortTtiA
lgo.SttiAlgoS
witch
parameter
Short TTI
## (FDD)
Different from UEs
that are scheduled
using normal
transmission time
intervals (TTIs), UEs
that are scheduled
using short TTIs
cannot use the
optimized CQI
adjustment value, but
use an individual set
of CQI adjustment
values.
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.54

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDData-
learning-
based
downlink
intelligent
## AMC
## DL_INTEL_A
## MC_SELECTI
## ON_SW
option of the
CellIntelAmc
## Config.
## Intelli
gentAmcSwit
ch parameter
eMIMO
## (FDD)
● If downlink target
IBLER adaptation is
enabled, the
eNodeB adaptively
adjusts the target
IBLER of UEs to
improve spectral
efficiency. In this
case, the spectral
efficiency is high. If
downlink
intelligent AMC is
then enabled, the
gains of downlink
intelligent AMC are
smaller than
expected.
● If enhanced
downlink target
IBLER adaptation is
enabled, the
eNodeB adaptively
adjusts the target
IBLER of UEs to
improve spectral
efficiency. In this
case, the spectral
efficiency is high. If
downlink
intelligent AMC is
then enabled, the
gains of downlink
intelligent AMC are
smaller than
expected.
● If variable-step-
based CQI
adjustment is
enabled, the
eNodeB adjusts the
IBLER convergence
rate based on the
scheduling
opportunities of
downlink services
for UEs. In this
case, the IBLER
convergence rate is
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.55

RATFunction
## Name
## Function
## Switch
ReferenceDescription
high. If downlink
intelligent AMC is
then enabled, the
gains of downlink
intelligent AMC are
smaller than
expected.
● If adaptive
variable-step-based
CQI adjustment is
enabled, the
eNodeB adjusts the
CQI adjustment
step based on the
UEs' HARQ
feedback for
downlink
transmissions. In
this case, the CQI
adjustment value
changes greatly. If
downlink
intelligent AMC is
then enabled, it
may not produce
significant gains.
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.56

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDownlink
intelligent
## JAMC
## CELL_DL_JOI
## NT_INTEL_A
## MC_SW
option of the
CellIntelAmc
## Config.
## Intelli
gentAmcSwit
ch parameter
Smart 8T8R
## (FDD)
● If variable-step-
based CQI
adjustment is
enabled, the
eNodeB adjusts the
IBLER convergence
rate based on the
scheduling
opportunities of
downlink services
for UEs. In this
case, the IBLER
convergence rate is
high. If downlink
intelligent JAMC is
then enabled, the
gains of downlink
intelligent JAMC
are smaller than
expected.
● If adaptive
variable-step-based
CQI adjustment is
enabled, the
eNodeB adjusts the
CQI adjustment
step based on the
UEs' HARQ
feedback for
downlink
transmissions. In
this case, the CQI
adjustment value
changes greatly. If
downlink
intelligent JAMC is
then enabled, it
may not produce
significant gains.

## 6.3 Requirements
## 6.3.1 Licenses
## None
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.57

## 6.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDCRS Port
## Number
Cell.CrsPortN
um
NoneCQI filtering based on
spectral efficiency
optimization can be
enabled only when
the Cell.CrsPortNum
parameter is set to
## CRS_PORT_4.

## Mutually Exclusive Functions
## RAT
## Function
## Name
## Function
## Switch
ReferenceDescription
FDDHigh speed
mobility
Cell.HighSpe
edFlag set to
## HIGH_SPEED
## High Speed
## Mobility
## None
FDDUltra high
speed
mobility
Cell.HighSpe
edFlag set to
## ULTRA_HIGH
## _SPEED
## High Speed
## Mobility
## None

## 6.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
●  Only the 3900 and 5900 series base stations (macro base stations) as well as
BTS3202E support CQI filtering based on spectral efficiency optimization.
●  Other functions: no requirements
## Boards
No requirements
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.58

RF Modules
No requirements
## 6.3.4 Others
## None
6.4 Operation and Maintenance
6.4.1 Data Configuration (FDD)
## 6.4.1.1 Data Preparation
Table 6-2 and Table 6-3 describe the parameters used for function activation and
optimization, respectively.
Table 6-2 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
CQI Adjust
## Algorithm
## Switch
CellAlgoSwitch.C
qiAdjAlgoSwitch
CqiAdjAlgoSwitchSelect this option.
DlVarIBLERtargetS
witch
Select this option.
DlEnVarIblerTar-
getSwitch
Select this option.
DlCqiAdjDeltaOpt
## Switch
Select this option.
RptCqiFltInitSwitc
h
Select this option.
StepVarySwitchSelect this option.
AdaptiveStepVar-
ySwitch
Select this option.
CqiFltSpectralEf-
fOptSwitch
Select this option.
PreciseMcsAdaptS
witch
Select this option.

eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.59

Table 6-3 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
## Initial
## Downlink
IBLER Target
CellCqiAdjAlgo.In
itDlIblerTarget
Set this parameter to its recommended
value.
## Initial Delta
## Cqi
CellCqiAdjAlgo.In
itDeltaCqi
Set this parameter to its recommended
value.
DL First
HARQ Tx TBS
## Index Increase
## Num
CellDlschAlgo.Dl
FirstHarqTxTbsIn
cNum
Set this parameter to its recommended
value.
CQI Adjust
## Step
CellCqiAdjAlgo.C
qiAdjStep
Set this parameter to its recommended
value.
TBS Index
Threshold for
## Low Target
## IBLER
CellDlschAlgo.Lo
wIblerTargetTbsI
dxThld
Set this parameter to its recommended
value.
TBS Index
Threshold for
## High Target
## IBLER
CellDlschAlgo.Hi
ghIblerTargetTb-
sIdxThld
Set this parameter to its recommended
value.
## CQI
## Adjustment
## Initial Step
CellDlschAlgo.Cqi
AdjInitialStep
Set this parameter to its recommended
value.

6.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
Before using MML commands, refer to 6.2.2 Impacts and 6.3.2 Software and
complete the parameter configurations for related functions based on the impact
and dependency relationships between the functions, as well as the actual
network scenario.
//Setting the switches of the CQI adjustment algorithm
MOD CELLALGOSWITCH: LocalCellId=0,
CqiAdjAlgoSwitch=DlVarIBLERtargetSwitch-1&DlEnVarIblerTargetSwitch-1&DlCqiAdjDeltaOptSwitch-1&RptC
qiFltInitSwitch-1&StepVarySwitch-1&AdaptiveStepVarySwitch-1&CqiFltSpectralEffOptSwitch-1&PreciseMcsAd
aptSwitch-1;
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.60

## Optimization Command Examples
//Modifying cell-specific CQI adjustment parameters
MOD CELLCQIADJALGO: LocalCellId=0, InitDlIblerTarget=10, InitDeltaCqi=-4, CqiAdjStep=10;
//Modifying cell-specific downlink scheduling parameters
MOD CELLDLSCHALGO: LocalCellId=0, CqiAdjInitialStep=10, DlFirstHarqTxTbsIncNum=0,
HighIblerTargetTbsIdxThld=5, LowIblerTargetTbsIdxThld=21;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Turning off the switches of the CQI adjustment algorithm
MOD CELLALGOSWITCH: LocalCellId=0,
CqiAdjAlgoSwitch=DlVarIBLERtargetSwitch-0&DlEnVarIblerTargetSwitch-0&DlCqiAdjDeltaOptSwitch-0&RptC
qiFltInitSwitch-0&StepVarySwitch-0&AdaptiveStepVarySwitch-0&CqiFltSpectralEffOptSwitch-0&PreciseMcsAd
aptSwitch-0;
6.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 6.4.2 Activation Verification
This section describes the procedures for verifying the activation of CQI
adjustment. The following examples show test results for commercial UEs in cells
with a bandwidth of 20 MHz.
Verifying CQI Adjustment
Step 1Enable a UE to access a cell in the cell center.
Step 2On the MAE-Access, start channel quality monitoring and BLER monitoring on the
## UE.
●  To start channel quality monitoring, choose Monitor > Signaling Trace >
Signaling Trace Management. Then in the navigation tree on the left,
choose Trace Type > LTE > User Performance Monitoring > Quality of
## Channel Monitoring.
●  To start BLER monitoring, choose Monitor > Signaling Trace > Signaling
Trace Management. Then in the navigation tree on the left, choose Trace
Type > LTE > User Performance Monitoring > BLER Monitoring.
Step 3Perform downlink full packet injection on the UE (about 1000 scheduling
instances). During the packet injection, gradually move the UE towards the cell
edge.
Step 4Check the downlink channel quality and the downlink IBLER. The CQI should be
approximately 11, and the value of Downlink IBLER(Permillage) is fluctuating
around 100. These values indicated that the downlink IBLER is approaching the
default value 10%. The results indicate that CQI adjustment has taken effect.
----End
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.61

Verifying Target IBLER Adaptation (FDD)
Step 1Enable a UE to access the cell.
Step 2On the MAE-Access, start BLER monitoring on the UE.
To start BLER monitoring, choose Monitor > Signaling Trace > Signaling Trace
Management. Then in the navigation tree on the left, choose Trace Type > LTE >
User Performance Monitoring > BLER Monitoring.
Step 3Perform downlink full packet injection on the UE. During the packet injection,
gradually move the UE towards the cell edge. Check the downlink BLER. The
downlink IBLER is approaching 30%. The result indicates that target IBLER
adaption has taken effect. If the configured initial downlink target IBLER is 15%,
check whether the downlink IBLER approaches 15%. If the downlink IBLER
approaches 15%, the related parameter setting has taken effect.
----End
Verifying Enhanced Target IBLER Adaptation
Step 1Enable a UE to access the cell.
Step 2On the MAE-Access, start BLER monitoring on the UE.
To start BLER monitoring, choose Monitor > Signaling Trace > Signaling Trace
Management. Then in the navigation tree on the left, choose Trace Type > LTE >
User Performance Monitoring > BLER Monitoring.
Step 3Ensure that the DlEnVarIblerTargetSwitch option has been selected.
Step 4Perform downlink full packet injection on the UE. During the packet injection,
gradually move the UE towards the cell edge. Check the downlink BLER. The
downlink IBLER is approaching 30%. The result indicates that enhanced target
IBLER adaption has taken effect.
----End
## 6.4.3 Network Monitoring
Monitor the counters listed in Table 6-4, and use the following formula to
calculate the downlink IBLER. Check that the downlink IBLER approaches the
default value 10%.
Table 6-4 Counters related to CQI adjustment
## Counter Name
## Counter Description
L.Traffic.DL.SCH.QPSK.E
rrTB.Ibler
Number of downlink error TBs after initial
transmission in QPSK modulation mode
L.Traffic.DL.SCH.16QA
M.ErrTB.Ibler
Number of downlink error TBs after initial
transmission in 16QAM modulation mode
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.62

Counter NameCounter Description
L.Traffic.DL.SCH.64QA
M.ErrTB.Ibler
Number of downlink error TBs after initial
transmission in 64QAM modulation mode
L.Traffic.DL.SCH.QPSK.T
## B
Number of TBs initially transmitted on the downlink
SCH in QPSK modulation mode
L.Traffic.DL.SCH.16QA
## M.TB
Number of TBs initially transmitted on the downlink
SCH in the 16QAM modulation mode
L.Traffic.DL.SCH.64QA
## M.TB
Number of TBs initially transmitted on the downlink
SCH in the 64QAM modulation mode
eRAN
## Channel State Management Feature Parameter
Description6 CQI Adjustment
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.63

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
eRAN
## Channel State Management Feature Parameter
## Description7 Parameters
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.64

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
eRAN
## Channel State Management Feature Parameter
## Description8 Counters
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.65

## 9 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
## Channel State Management Feature Parameter
## Description9 Glossary
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.66

## 10 Reference Documents
1.Scheduling
2.eMIMO (FDD)
3.Compact Bandwidth (FDD)
4.NB-IoT Basics (FDD)
5.CDMA and LTE Zero Bufferzone
6.GSM and LTE Buffer Zone Optimization
7.UL Refarming Zero Bufferzone
8.GSM and LTE Spectrum Concurrency
9.Flexible Bandwidth based on Overlap Carriers (FDD)
## 10.SFN
11.DL CoMP (FDD)
12.Dedicated Carrier for TM9
13.WTTx MU-MIMO (FDD)
14.S1 and X2 Self-Management
15.Physical Channel Resource Management
16.Short TTI (FDD)
## 17.CSPC
18.eX2 Self-Management
19.Energy Conservation and Emission Reduction
20.Smart 8T8R (FDD)
21.High Speed Mobility
eRAN
## Channel State Management Feature Parameter
## Description10 Reference Documents
Issue 08 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.67