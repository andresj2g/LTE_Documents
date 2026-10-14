

eRAN
DL CoMP (FDD) Feature Parameter
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
2 About This Document.............................................................................................................4
2.1 General Statements................................................................................................................................................................ 4
2.2 Applicable RAT......................................................................................................................................................................... 5
2.3 Features in This Document.................................................................................................................................................. 5
3 Overview....................................................................................................................................6
3.1 Introduction...............................................................................................................................................................................6
3.2 Related Concepts.....................................................................................................................................................................8
3.3 Architecture............................................................................................................................................................................... 8
4 DL CoMP with TM10.............................................................................................................10
4.1 Principles.................................................................................................................................................................................. 10
4.1.1 Selection of a Coordinating Cell Set........................................................................................................................... 10
4.1.2 Selection of CoMP UEs and Coordinating Cells...................................................................................................... 11
4.1.2.1 Entering the DPS Mode............................................................................................................................................... 11
4.1.2.2 Entering the JT Mode................................................................................................................................................... 12
4.1.2.3 Exiting the DPS or JT Mode........................................................................................................................................13
4.1.3 Multi-Cell Coordinated Transmission..........................................................................................................................13
4.2 Network Analysis.................................................................................................................................................................. 14
4.2.1 Benefits................................................................................................................................................................................. 14
4.2.2 Impacts..................................................................................................................................................................................14
4.3 Requirements......................................................................................................................................................................... 21
4.3.1 Licenses................................................................................................................................................................................. 21
4.3.2 Software................................................................................................................................................................................21
4.3.3 Hardware..............................................................................................................................................................................24
4.3.4 Networking.......................................................................................................................................................................... 25
4.3.5 Others....................................................................................................................................................................................25
4.4 Operation and Maintenance.............................................................................................................................................27
eRAN
DL CoMP (FDD) Feature Parameter DescriptionContents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iii

4.4.1 Data Configuration........................................................................................................................................................... 27
4.4.1.1 Data Preparation............................................................................................................................................................ 27
4.4.1.2 Using MML Commands............................................................................................................................................... 32
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 33
4.4.2 Activation Verification......................................................................................................................................................33
4.4.3 Network Monitoring.........................................................................................................................................................34
4.4.4 Possible Issues.................................................................................................................................................................... 35
5 DL CoMP with TM9...............................................................................................................37
5.1 Principles.................................................................................................................................................................................. 37
5.1.1 Selection of a TM9 JT Coordinating Cell Set............................................................................................................37
5.1.2 Selection of TM9 JT UEs and Coordinating Cells....................................................................................................38
5.1.2.1 Entering the JT Mode................................................................................................................................................... 38
5.1.2.2 Exiting the JT Mode.......................................................................................................................................................39
5.1.3 Multi-Cell Coordinated Transmission..........................................................................................................................39
5.2 Network Analysis.................................................................................................................................................................. 40
5.2.1 Benefits................................................................................................................................................................................. 40
5.2.2 Impacts..................................................................................................................................................................................40
5.3 Requirements......................................................................................................................................................................... 49
5.3.1 Licenses................................................................................................................................................................................. 49
5.3.2 Software................................................................................................................................................................................49
5.3.3 Hardware..............................................................................................................................................................................50
5.3.4 Networking.......................................................................................................................................................................... 51
5.3.5 Others....................................................................................................................................................................................51
5.4 Operation and Maintenance.............................................................................................................................................53
5.4.1 Data Configuration........................................................................................................................................................... 53
5.4.1.1 Data Preparation............................................................................................................................................................ 53
5.4.1.2 Using MML Commands............................................................................................................................................... 58
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 58
5.4.2 Activation Verification......................................................................................................................................................58
5.4.3 Network Monitoring.........................................................................................................................................................59
5.4.4 Possible Issues.................................................................................................................................................................... 60
6 Parameters..............................................................................................................................62
7 Counters.................................................................................................................................. 63
8 Glossary................................................................................................................................... 64
9 Reference Documents...........................................................................................................65
eRAN
DL CoMP (FDD) Feature Parameter DescriptionContents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 04 (2023-09-14)
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.2 eRAN18.1 03 (2023-04-23)
## Technical Changes
## Change Description
## Parameter
## Change
RATBase Station
## Model
Added the impact
relationship between DL
CoMP with TM10 and
the RuralLink solution
(LTE). For details, see
## Function Impacts.
NoneFDD5900 series base
stations (macro
base stations)

eRAN
DL CoMP (FDD) Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.1

## Editorial Changes
Revised descriptions in this document.
1.3 eRAN18.1 02 (2023-02-01)
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 01 (2022-03-08)
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 03 (2021-06-26).
## Technical Changes
## Change Description
Parameter ChangeBase Station Model
Added the impact
relationship between DL
CoMP with TM10 and
energy saving based on
flexible frequency-domain
scheduling. For details, see
## 4.2.2 Impacts.
None● 3900 and 5900
series base
stations
## ● DBS3900
LampSite and
## DBS5900
LampSite
Added the impact
relationship between DL
CoMP with TM9 and energy
saving based on flexible
frequency-domain
scheduling. For details, see
## 5.2.2 Impacts.
None● 3900 and 5900
series base
stations
## ● DBS3900
LampSite and
## DBS5900
LampSite
eRAN
DL CoMP (FDD) Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.2

Change DescriptionParameter ChangeBase Station Model
Added the impact
relationship between DL
CoMP with TM9 and Next
Generation eCall over LTE.
For details, see 5.2.2
## Impacts.
None● 3900 and 5900
series base
stations
## ● DBS3900
LampSite and
## DBS5900
LampSite
Added the mutually
exclusive relationship
between DL CoMP with TM9
and TM4 and TM6
Adaptation. For details, see
## 5.3.2 Software.
None● 3900 and 5900
series base
stations
## ● DBS3900
LampSite and
## DBS5900
LampSite

## Editorial Changes
Revised descriptions in this document.
eRAN
DL CoMP (FDD) Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.3

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
DL CoMP (FDD) Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.4

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
Feature ID
Feature NameChapter/Section
LAOFD-120201DL CoMP (Trial)4 DL CoMP with TM10
LBFD-150302Joint Transmission
with TM9
5 DL CoMP with TM9
eRAN
DL CoMP (FDD) Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.5

## 3 Overview
## 3.1 Introduction
Downlink coordinated multipoint transmission (DL CoMP) is implemented based
on TM9 introduced in 3GPP Release 10 or TM10 introduced in 3GPP Release 11.
This feature enables multiple cells to work collaboratively based on ideal backhaul
transmission (intra-BBU or USU-based multi-BBU interconnection) to process and
transmit physical downlink shared channel (PDSCH) data of a UE using antennas
of neighboring cells.
●  DL CoMP with TM10 corresponds to LAOFD-120201 DL CoMP (Trial). It uses
dynamic point selection (DPS) and joint transmission (JT) to improve the
capacity of hotspot cells or uses JT to improve the performance of cell edge
users (CEUs). eNodeBs can adaptively select an appropriate transmission
mode based on the cell load and channel quality.
●  DL CoMP with TM9 corresponds to LBFD-150302 Joint Transmission with
TM9. JT is used to improve CEU performance.
## DPS
In DPS mode, the coordinating cell sends PDSCH data to the UE to increase the
hotspot cell capacity, CEU throughput, and average UE throughput.
Figure 3-1 illustrates the DPS mode. In this mode, the PDCCH data of a UE is sent
by cell 1 (serving cell), and its PDSCH data is sent to cell 2 (coordinating cell)
through cell 1 and then sent by cell 2.
eRAN
DL CoMP (FDD) Feature Parameter Description3 Overview
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.6

Figure 3-1 DPS
## JT
In JT mode, both the serving cell and coordinating cell transmit PDSCH data to
improve the throughput of CEUs with a low signal to interference plus noise ratio
## (SINR).
Figure 3-2 illustrates the JT mode, in which
●  PDCCH data of the UE is sent by cell 1 (the serving cell), and PDSCH data is
sent by cell 1 to cell 2 (the coordinating cell). Cell 1 and cell 2 allocate the
same RBs to send PDSCH data to the UE.
●  The UE receives the same PDSCH data from cell 1 and cell 2 simultaneously.
Figure 3-2 JT
eRAN
DL CoMP (FDD) Feature Parameter Description3 Overview
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.7

## 3.2 Related Concepts
Table 3-1 lists the concepts related to DL CoMP.
Table 3-1 Related concepts
ConceptDefinition
Coordinating cell
set of the
serving cell
A set of 10 neighboring cells that cause the strongest
interference to the serving cell as measured by the eNodeB
Serving cellA serving cell is the cell that UEs access.
DPS UEThe eNodeB uses algorithms to determine whether a UE
meets the DPS threshold conditions. The UE that meets the
DPS threshold conditions is a DPS UE.
JT UEThe eNodeB uses algorithms to determine whether a UE
meets the JT threshold conditions. The UE that meets the JT
threshold conditions is a JT UE.
Coordinating cell
of a DPS or JT
## UE
The eNodeB identifies the coordinating cells for a DPS or JT
UE based on the event A3 measurement report sent by the
DPS or JT UE. The coordinating cells of a UE belong to the
coordinating cell set of the serving cell of the UE.
eX2 interfaceWhen USU-based multi-BBU interconnection is used, the eX2
interface is responsible for service coordination between
eNodeBs.

## 3.3 Architecture
DL CoMP is implemented through the coordination of the MAE-Access, USU,
eNodeB, and UE. Figure 3-3 to Figure 3-5 show the networking diagrams. If DL
CoMP is performed among BBUs, time synchronization is required across the
entire network.
Figure 3-3 Networking diagram for intra-BBU DL CoMP (HomNet/HetNet
networking)
eRAN
DL CoMP (FDD) Feature Parameter Description3 Overview
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.8

Figure 3-4 Networking diagram for inter-BBU DL CoMP (HomNet networking)
Figure 3-5 Networking diagram for inter-BBU DL CoMP (HetNet networking)
Table 3-2 describes the functions of the network elements (NEs).
Table 3-2 NE functions
## NE
## Function
## MAE-
## Access
Used for parameter configuration and performance monitoring.
eNodeB●Configures channel state information-reference signal (CSI-RS)
resources of a cell.
● Maintains and manages the coordinating cell set of a cell.
● Determines whether a UE is a DPS or JT UE and configures TM9
or TM10 for the UE.
● Performs coordinated transmission based on DPS or JT UE
attributes.
UE● Reports air interface measurement information, including the
reference signal received power (RSRP) and CSI.
● Receives PDSCH data according to the DCI format 2D or DCI
format 2C indication.
eRAN
DL CoMP (FDD) Feature Parameter Description3 Overview
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.9

4 DL CoMP with TM10
## 4.1 Principles
Figure 4-1 shows the DL CoMP process, including selection of a coordinating cell
set, selection of CoMP UEs and coordinating cells, and multi-cell coordinated
transmission.
Figure 4-1 DL CoMP process
4.1.1 Selection of a Coordinating Cell Set
The eNodeB selects a coordinating cell set as follows:
-  The NCellDlRsrpMeasPara.DlRsrpAutoNCellMeasSwitch parameter is set to
ON and the NCellDlRsrpMeasPara.
NCellDlRsrpMeasA3Offset parameter is
set to a desired value.
-  After DL CoMP with TM10 is enabled, the eNodeB selects a coordinating cell
set for the serving cell based on the neighboring cell information reported by
UEs.
The DL CoMP algorithm switch settings vary with networking scenarios.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.10

## Network
ing
## Scenario
## Parameter Setting
HomNetFDDHomNetDlCompSwitch option of the
CellAlgoSwitch.DlCompSwitch parameter
HetNetFDDHetNetDlCompSwitch option of the
CellAlgoSwitch.DlCompSwitch parameter
HomNet
and
HetNet
Both of the preceding options are selected.

-  By collecting information on neighboring cells that meet event A3 reporting
conditions once every hour, the eNodeB selects 10 neighboring cells that
cause the highest interference to the serving cell as the coordinating cell set
for DL CoMP. If micro cells exist, the eNodeB preferentially selects micro cells
(6 at most), and then selects macro cells to form a coordinating cell set.
4.1.2 Selection of CoMP UEs and Coordinating Cells
After selecting the DPS or JT serving cell, the eNodeB selects coordinating cells
and CoMP UEs based on the preset load thresholds.
4.1.2.1 Entering the DPS Mode
The process for a UE to enter the DPS mode is as follows:
-  DPS serving cell selection is triggered.
Figure 4-2 Triggering of DPS/JT serving cell selection
As shown in Figure 4-2, when the PRB usage of the serving cell is greater
than the threshold specified by the
CellDlCompAlgo.
DpsServingCellDlPrbThd parameter and the serving cell is
a macro cell, the eNodeB selects the serving cell as the DPS serving cell.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.11

-  The eNodeB selects the cells with the strongest RSRP in the coordinating cell
set as coordinating cells.
If the RSRP of a neighboring cell of the UE minus that of the serving cell of
the UE is greater than or equal to the coordinating cell RSRP threshold plus
the coordinating cell RSRP offset, the UE reports event A3. If the neighboring
cell that meets the event A3 reporting conditions belongs to the coordinating
cell set, it is selected as a coordinating cell.
–   In HomNet networking scenarios, the coordinating cell RSRP threshold is
specified by the CellDlCompAlgo.HomnetDpsCoCellRsrpThd parameter,
and only the macro cells with the strongest RSRP in the coordinating cell
set can be selected as coordinating cells.
–   In HetNet scenarios, the coordinating cell RSRP threshold is specified by
the CellDlCompAlgo.
HetnetDpsCoCellRsrpThd parameter, and only the
micro cells with the strongest RSRP in the coordinating cell set can be
selected as coordinating cells.
–   In HomNet and HetNet hybrid networking scenarios, the micro cells with
the strongest RSRP in the coordinating cell set are preferentially selected
as coordinating cells.
## NO TE
The system automatically configures the coordinating cell RSRP offset to prevent ping-
pong configuration of TM10 for UEs.
-  The eNodeB selects DPS UEs.
If the coordinating cells selected in 2 meet all of the following conditions, the
eNodeB selects the UEs as DPS UEs and configures the TM10 mode for them.
–   The PRB usage of the serving cell minus the PRB usage of a coordinating
cell is greater than the value of the CellDlCompAlgo.
DpsLoadDiffThd
parameter.
–   The number of UEs in RRC_CONNECTED mode in a coordinating cell
divided by the number of UEs in RRC_CONNECTED mode in the serving
cell is less than or equal to the value of the
CellDlCompAlgo.
DpsCoCellUserRatioThd parameter. The selected DPS
UE is regarded as a UE in the coordinating cell.
–   No PCI mod 3 conflict exists between coordinating cells and the serving
cell.
4.1.2.2 Entering the JT Mode
The process for a UE to enter the JT mode is as follows:
-  JT serving cell selection is triggered.
As shown in Figure 4-2, when the PRB usage of the serving cell is less than or
equal to the threshold specified by the
CellDlCompAlgo.
JtServingCellDlPrbThd parameter, the eNodeB selects the
serving cell as the JT serving cell.
-  The eNodeB selects the cells with the strongest RSRP in the coordinating cell
set as coordinating cells.
If the RSRP of a neighboring cell of the UE minus that of the serving cell of
the UE is greater than or equal to the value of the
CellDlCompAlgo.
JtCoCellRsrpThd parameter plus the coordinating cell RSRP
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.12

offset, and the neighboring cell belongs to the coordinating cell set, it is
selected as a coordinating cell.
–   In HomNet networking scenarios, only the cells of the same site type as
the serving cell and with the strongest RSRP in the coordinating cell set
can be selected as coordinating cells.
–   In HetNet networking scenarios, when the serving cell is a macro cell,
only the micro cells with the strongest RSRP in the coordinating cell set
can be selected as coordinating cells.
–   In HomNet and HetNet hybrid networking scenarios, the cells with the
strongest RSRP in the coordinating cell set are preferentially selected as
coordinating cells.
## NO TE
The system automatically configures the coordinating cell RSRP offset to prevent ping-
pong configuration of TM10 for UEs.
-  The eNodeB selects JT UEs.
If the coordinating cells selected in 2 meet all of the following conditions, the
eNodeB selects the UEs as JT UEs and configures the TM10 mode for them.
–   The PRB usage of a coordinating cell is less than the value of the
CellDlCompAlgo.
JtCoCellDlPrbThd parameter.
–   When the UE is a 256QAM UE, the spectral efficiency corresponding to
the CQI for each codeword reported by the UE is lower than that
corresponding to CQI 4. For details about CQI 4, see "Table 7.2.3-2 4-bit
CQI Table 2" in section 7.2.3 "Channel Quality Indicator (CQI) definition"
in 3GPP TS 36.213 V12.9.1.
–   When the UE is a non-256QAM UE, the spectral efficiency corresponding
to the CQI for each codeword reported by the UE is lower than that
corresponding to CQI 7. For details about CQI 7, see "Table 7.2.3-1 4-bit
CQI Table" in section 7.2.3 "Channel Quality Indicator (CQI) definition" in
## 3GPP TS 36.213 V12.9.1.
4.1.2.3 Exiting the DPS or JT Mode
If a DPS or JT UE reports exit event A3, the eNodeB disables TM10 configuration
for the UE and configures the UE as a common user.
4.1.3 Multi-Cell Coordinated Transmission
After the eNodeB determines the DPS or JT serving cell based on the downlink
PRB usage threshold, the transmission mode used by the serving cell is also
determined.
As shown in Figure 4-3, the eNodeB delivers two sets of CSI measurement
configurations to a CoMP UE for measuring channel state information (CSI),
including precoding matrix indication (PMI), rank indication (RI), and CQI, of the
serving and coordinating cells, respectively. The eNodeB transmits data in DPS or
JT mode based on the CSI measurement results reported by the UE and the
scheduling information of the serving and coordinating cells.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.13

Figure 4-3 CSI measurement configuration
## 4.2 Network Analysis
## 4.2.1 Benefits
## Gains
This feature improves the downlink throughput and user experience of CEUs.
●  DPS increases the capacity of hotspot cells and improves the CEU throughput
and average UE throughput when the network load is heavy and imbalanced.
●  JT improves the throughput of CEUs with a low SINR when the network load
is light.
## Most Beneficial Scenarios
This feature is recommended when all of the following conditions are met:
●  The inter-site distance is less than 500 m in densely populated urban areas.
●  The average downlink PRB usage of hotspot cells is greater than 40% in
heavy-load scenarios. This condition is more easily met in macro-micro
networking scenarios.
●  The average downlink PRB usage of cells is less than 20% in light-load
scenarios.
●  Most UEs move at a speed lower than 10 km/h.
●  The penetration rate of TM10-capable UEs exceeds 70%.
## 4.2.2 Impacts
## Network Impacts
●  When DPS takes effect, PDSCH data of CEUs in the heavily loaded serving cell
are offloaded to coordinating cells. In this way, more resources are available
for UEs in the serving cell, and the user-perceived downlink throughput in the
serving cell increases. If the increase of resources for DPS UEs in the lightly
loaded coordinating cells cannot compensate for the loss of channel quality
deterioration, the user-perceived downlink throughput of the DPS UEs
decreases.
●  HomNet networking: When the PRB usage of the heavily loaded cell is 60%,
DL CoMP increases the CEU throughput by 5% to 10% and the average UE
throughput by up to 5%.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.14

●  HetNet networking: When a macro cell includes four micro cells and the PRB
usage of the macro cell is 60%, DL CoMP increases the CEU throughput by
about 20% and the average UE throughput by about 10%.
●  When the PRB usage of a cell is 10%, DL CoMP increases the throughput of JT
UEs by about 10%. The CEU throughput increase depends on the proportion
of JT UEs among CEUs.
## Function Impacts
## Function
## Name
Function SwitchReferenceDescription
VoIP
semi-
persistent
schedulin
g
Uplink: SpsSchSwitch
option of the
CellAlgoSwitch.UlSch
Switch parameter
## Downlink:
SpsSchSwitch option
of the
CellAlgoSwitch.
DlSch
## Switch
parameter
VoLTEResource conflicts may occur
between coordinating cell
scheduling of DL CoMP with
TM10 and semi-persistent
scheduling. Therefore,
coordinating cell scheduling
of DL CoMP is not performed
within the TTI in which semi-
persistent scheduling is in
effect.
MROCellAlgoSwitch.MroS
witch
MROMRO may affect the optimal
RSRP threshold setting of
coordinating cells in DL CoMP
with TM10. As a result, the
cell-edge throughput across
the entire network cannot
reach the optimal level that
DL CoMP with TM10 can
achieve.
## Enhanced
downlink
frequency
selective
schedulin
g
FreqSelSwitch option
of the
CellAlgoSwitch.DlSch
Switch parameter
SchedulingFrequency-selective
scheduling can be performed
for UEs using DL CoMP with
TM10 only in the serving cell.
## Symbol
power
saving
SymbolShutdownS-
witch option of the
ENodeBAlgoSwitch.P
owerSaveSwitch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
When both DL CoMP with
TM10 and symbol power
saving are enabled, symbol
power saving is not triggered
in the coordinating cells for
DL CoMP with TM10 during
scheduling in these cells.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.15

## Function
## Name
Function SwitchReferenceDescription
ePDCCH
## (trial)
CellPdcchAlgo.Epdcc
hAlgoSwitch
## Physical
## Channel
## Resource
## Managem
ent
When both DL CoMP with
TM10 and ePDCCH are
enabled, a UE configured
with the ePDCCH cannot be
selected as a CoMP UE. As a
result, DL CoMP with TM10
cannot achieve optimal
performance.
## Emergenc
y call
NoneEmergency
## Call
UEs making emergency calls
cannot be selected as CoMP
UEs. As a result, DL CoMP
with TM10 cannot achieve
optimal performance.
## Coordinat
ed
schedulin
g-based
power
control
## Coordinated
scheduling-based
power control (CSPC):
CellCspcPara.CellCsp
cSwitch
eCSPC:
CellCspcPara.CelleCs
pcSwitch
Intra-eNodeB CSPC:
CellCspcPara.
IntraEn
bCspcSw
CSPC● DL CoMP with TM10 and
CSPC (controlled by
CellCspcPara.CellCspcSwi
tch) can be enabled
simultaneously, but CSPC
takes effect preferentially.
If CSPC has taken effect in
a cell, DL CoMP UEs are
not scheduled in
coordinating cells.
● DL CoMP with TM10 and
eCSPC (controlled by
CellCspcPara.
CelleCspcSw
itch
) cannot be enabled
simultaneously.
SFNUplink:
CellAlgoSwitch.SfnUl
SchSwitch
## Downlink:
CellAlgoSwitch.SfnDl
SchSwitch
SFNIf the antenna modes of the
physical cells forming an SFN
cell are different, the SFN cell
cannot be selected as a
coordinating cell for DL
CoMP. That is, DL CoMP with
TM10 cannot be used in the
SFN cell.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.16

## Function
## Name
Function SwitchReferenceDescription
## Adaptive
## SFN/
## SDMA
## Uplink:
CellAlgoSwitch.SfnUl
SchSwitch
## Downlink:
CellAlgoSwitch.SfnDl
SchSwitch
SFNDL CoMP with TM10 and
adaptive SFN/SDMA can be
enabled simultaneously.
However, the joint scheduling
mode is always used for UEs
in coordinating cells because
the serving cell does not have
RSRP information about the
RRUs serving neighboring
cells and cannot determine
UE attributes.
eMTC
introducti
on
## EMTC_SWITCH
option of the
CellEmtcAlgo.EmtcAl
goSwitch parameter
eMTCeMTC UEs do not support DL
CoMP with TM10.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.17

## Function
## Name
Function SwitchReferenceDescription
## DL
## 256QAM
Dl256QamSwitch
option of the
CellAlgoSwitch.Dl256
QamAlgoSwitch
parameter
## Modulatio
n Schemes
## ● If
CellDlschAlgo.Dl256Qam
CqiTblCfgStrategy is set
to ADAPTIVE_CONFIG or
## CQI_BASED_ADAPTIVE_C
ONFIG for the serving cell,
JT UEs can be selected as
256QAM UEs, and non-JT
UEs with 256QAM cannot
be selected as JT UEs. This
is because non-JT UEs can
be selected as 256QAM
UEs only when the SINR is
high in adaptive
configuration mode.
## ● If
CellDlschAlgo.
Dl256Qam
CqiTblCfgStrategy is set
to FIX_CONFIG for the
serving cell, JT UEs can be
selected as 256QAM UEs,
and non-JT UEs with
256QAM can be selected
as JT UEs.
For details about 256QAM
UEs, see "Table 7.2.3-2 4-bit
CQI Table 2" in section
"Channel quality indicator
(CQI) definition" in 3GPP TS
36.213. The 256QAM UEs
mentioned earlier are UEs for
which this CQI table is
selected.
DL CoMP with TM10 can be
performed only when the DL
256QAM switch settings of
the serving and coordinating
cells are the same.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.18

## Function
## Name
Function SwitchReferenceDescription
## Dynamic
## Power
## Sharing
## Between
## LTE
## Carriers
## LTE_DYN_POWER_SH
ARING_SW option of
the
CellDynPowerShar-
ing.DynamicPowerSh
aringSwitch
parameter
## Dynamic
## Power
## Sharing
## Between
## LTE
## Carriers
● Jointly scheduled JT UEs
do not share power.
Independently scheduled
JT UEs can share power.
● DPS UEs can share power
when scheduled in the
serving cell, but cannot
share power when
scheduled in coordinating
cells.
## Downlink
## 2CC
aggregati
on
NoneCarrier
## Aggregatio
n
DL CoMP with TM10 can be
configured in both the PCells
and SCells of UEs in the intra-
BBU CA state.
## Downlink
## FDD+TDD
## CA
InterFddTddCaSwitch
option of the
CaMgtCfg.CellCaAlgo
Switch parameter
## Carrier
## Aggregatio
n
DL CoMP with TM10 can be
configured in both the PCells
and SCells of UEs in the intra-
BBU CA state.
DL CoMP
with TM9
Tm9JtSwitch option
of the
CellAlgoSwitch.DlCo
mpSwitch parameter
DL CoMP
## (FDD)
If both DL CoMP with TM10
and DL CoMP with TM9 are
enabled and the conditions
for them to take effect are
both met, DL CoMP with TM9
is preferentially used.
## Static
## Multiple
## Beam
None3D
## Beamform
ing (FDD)
When inner and outer cells
generated using vertical
multiple sectors (VMS) are
working for CoMP, the cell
power setting must be
reduced by half. This affects
network performance.
## Precise
## AMC
PreciseAmcSwitch
option of the
CellAlgoSwitch.Emim
oSwitch parameter
eMIMO
## (FDD)
Enabling DL CoMP affects the
accuracy of calculated
interference from neighboring
cells and further affects the
performance of precise AMC.
Therefore, you are advised to
disable precise AMC when DL
CoMP is enabled.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.19

## Function
## Name
Function SwitchReferenceDescription
## NPREO
constant
optimizati
on
CellDlpcPdschPa.UeN
preoAdjThreshold
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
the accuracy of neighboring
cell interference calculation is
affected and the performance
of UE-level NPREO constant
optimization is affected.
Therefore, you are advised
not to enable UE-level
NPREO constant
optimization.
## Downlink
target
## IBLER
adaptatio
n
DlVarIBLERtargetS-
witch option of the
CellAlgoSwitch.CqiA
djAlgoSwitch
parameter
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
aperiodic CQI reporting is
used, which affects the
accuracy of downlink target
IBLER adaptation. Therefore,
when both DL CoMP and
downlink target IBLER
adaptation are enabled,
downlink target IBLER
adaptation does not take
effect for JT UEs.
## Enhanced
downlink
target
## IBLER
adaptatio
n
DlEnVarIblerTargetS-
witch option of the
CellAlgoSwitch.CqiA
djAlgoSwitch
parameter
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
aperiodic CQI reporting is
used, which affects the
accuracy of enhanced
downlink target IBLER
adaptation. Therefore, when
both DL CoMP and enhanced
downlink target IBLER
adaptation are enabled,
enhanced downlink target
IBLER adaptation does not
take effect for JT UEs.
## Energy
saving
based on
flexible
frequency
## -domain
schedulin
g
## FLEX_FREQ_SCH_ENE
## RGY_SAVING_SW
option of the
CellPwrSavingAl-
go.PwrSavingAlgoSw
itch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
Energy saving based on
flexible frequency-domain
scheduling is not performed
for TM10 JT UEs.
RuralLink
solution
CellTypeExt.Wireless
FhCellFlag
RuralLink
## Solution
RuralLink cells do not support
DL CoMP with TM10.

eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.20

## 4.3 Requirements
## 4.3.1 Licenses
There are currently no license requirements for trial features. For details, see 2.1
## General Statements.
## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## Function
## Name
Function SwitchReferenceDescription
## Synchronizati
on with GPS
NoneSynchroniz
ation
If DL CoMP is performed
among BBUs, time
synchronization is required
across the entire network. In
this case, DL CoMP requires
either of the two functions.
## IEEE1588 V2
clock
synchronizati
on
NoneSynchroniz
ation

## Mutually Exclusive Functions
## Function
## Name
Function SwitchReferenceDescription
## Adaptive
power
allocation for
cell-edge UEs
AdptCellEdgePwr
AllocSw option of
the
CellAlgoSwitch.Ce
llDlCoverEnhance
## Switch
parameter
SchedulingAdaptive power allocation for
cell-edge UEs does not take
effect for DL CoMP UEs.
High speed
mobility
Cell.HighSpeedFla
g
## High
## Speed
## Mobility
In high-speed mobility
scenarios, channel conditions
and cell load change so
rapidly that DL CoMP cannot
be promptly performed.
Ultra high
speed
mobility
Cell.HighSpeedFla
g
## High
## Speed
## Mobility
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.21

## Function
## Name
Function SwitchReferenceDescription
## Extended
## Cell Access
## Radius
Cell.CellRadiusExtended
## Cell Range
In DL CoMP, UEs need to
receive data from different
cells simultaneously.
Therefore, DL CoMP does not
apply to extended cell range
scenarios.
Extended CPCell.DlCyclicPrefixExtended
## CP
## Dynamic
TDM eICIC
CellAlgoSwitch.Ei
cicSwitch
TDM eICIC
## (FDD)
Both DL CoMP and enhanced
inter-cell interference
coordination (eICIC) can offer
macro-micro offloading gains
by using cell range expansion
(CRE). Because CEUs have
been handed over to the
micro cell, enabling both DL
CoMP and eICIC will generate
negative impacts.
FeICICCellAlgoSwitch.Fe
icicSwitch
TDM eICIC
## (FDD)
## Adaptive
inter-cell
interference
coordination
NoneAdaptive
## ICIC
Adaptive inter-cell
interference coordination
(ICIC) is based on the
eCoordinator architecture.
After DL CoMP is enabled,
the frequency bands of
neighboring cells where
adaptive ICIC takes effect
cannot be obtained. In this
case, UEs cannot be
coordinated to neighboring
cells for scheduling.
Virtual 4T4RVirtual4T4RSwitc
h option of the
CellAlgoSwitch.E
mimoSwitch
parameter
## Virtual
## 4T4R
## (FDD)
DL CoMP is temporarily not
supported in virtual 4T4R
scenarios.
## Massive
MIMO cell
NoneMassive
## MIMO
## (FDD)
## None
## Intelligent
beam
shaping
## MM_INTELLIGENT
## _BEAM_SHAPING_
SW option of the
SectorSplitGroup.
SectorSplitSwitch
parameter
## Massive
## MIMO
## (FDD)
## None
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.22

## Function
## Name
Function SwitchReferenceDescription
## Downlink
MU-MIMO in
## TM9
4TxTM9MuMimoS
witch option of
the
CellAlgoSwitch.E
mimoSwitch
parameter
eMIMO
## (FDD)
Downlink MU-MIMO in TM9
is generally used in heavy-
load scenarios, while JT is
used in light-load scenarios.
Therefore, downlink MU-
MIMO in TM9 and TM10 JT
cannot be enabled at the
same time.
eCSPCCellCspcPara.Celle
CspcSwitch
CSPCeCSPC adjusts power among
cells to reduce interference
and applies to heavy-load
scenarios. The gain source
and application scenarios of
eCSPC are different from
those of JT.
4x4 MIMO in
the
overlapping
areas
between the
physical cells
of an SFN
cell
SfnJtSwitch
option of the
CellAlgoSwitch.Sf
nAlgoSwitch
parameter
SFN4x4 MIMO in the overlapping
areas between the physical
cells of an SFN cell and DL
CoMP with TM10 cannot be
enabled at the same time
due to issues related to CSI-
RS cooperation between
features.
Inter-eNodeB
SFN based
on eNodeB
coordination
Cell.EuCellStandb
yMode
SFNIn inter-BBU SFN scenarios,
SFN cells do not support DL
CoMP with TM10.
## Adaptive
## SFN/SDMA
with TM9/
## TM10
TM9Switch option
of the
CellAlgoSwitch.En
hMIMOSwitch
parameter
SFNDL CoMP with TM10 and
adaptive SFN/SDMA with
TM9 cannot be enabled at
the same time.
## Dynamic
## Massive
## Beam
None3D
## Beamform
ing (FDD)
## None
WTTx MU-
## MIMO
Tm9FourLayerPair
Switch option of
the
CellAlgoExtSwitch
.WttxMuMimoSwi
tch
parameter
WTTx MU-
## MIMO
## (FDD)
## None
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.23

## Function
## Name
Function SwitchReferenceDescription
RF channel
dynamic
muting
## RF_CHN_DYN_MU
TING_SW option
of the
CellRfChnDynMut
ing.RfChnDynMut
ingAlgoSwitch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
## None
## Static
## Multiple
## Beam
SectorSplitGroup.
BeamTemplateId
set to 0,
SectorSplitGroup.
BeamDeployment
## Mode
set to
MODE_3, and
SectorSplitCell.Cel
lBeamIndex
set to
0 or 1
## Smart
## 8T8R
## (FDD)
## None

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
The following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  USU3910
## Boards
●  BBU: The BBU5900A/BBU5900/BBU3900/BBU3910/BBU3910A/BBU3910C
supports this function. When the BBU3910A is used, only intra-BBU DL CoMP
is supported, and inter-BBU DL CoMP is not supported.
●  BBP: The LBBP does not support this function.
●  Main control board: A UMPT must be configured to support this function.
RF Modules
Micro cells in DL CoMP are those served by low-power RRUs, such as the
RRU3220E and RRU3230E.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.24

## Cells
●  JT: Both of the following requirements must be met:
–   The Cell.CrsPortNum settings of the cells where this function is enabled
are the same.
–   Both the serving cell and coordinating cell must support 2T or 4T.
●  DPS: Both the serving cell and coordinating cell must support 2T or 4T.
## 4.3.4 Networking
●  If inter-BBU DL CoMP is used, the Cloud BB network using USU-based multi-
BBU interconnection must be deployed.
–   For details about Cloud BB networking, see Cloud BB Overview.
–   For details about the networking, cable connections, and clock
synchronization for the USU3910-based Cloud BB architecture, see
USU3910-based Multi-BBU Interconnection.
●  eNodeBs provide contiguous coverage with the same frequency and
bandwidth. The cell bandwidth must be greater than or equal to 5 MHz. It is
recommended that the bandwidth be greater than 5 MHz even if the function
supports the 5 MHz bandwidth.
●  The PDSCHCfg.Pb settings of the cells where this feature is enabled are the
same.
●  If inter-BBU DL CoMP is used, time synchronization is required across the
entire network. The time synchronization accuracy between all cells with DL
CoMP to be enabled must be less than 3 μs, and GPS or IEEE1588 V2
synchronization can be used. For details, see
## Synchronization.
## 4.3.5 Others
## NO TICE
The performance counters of CEUs can be obtained only when the
BasedA3EdgeUserSwitch option of the
CellCounterParaGroup.CellCounterAlgoSwitch parameter is selected. The
eNodeB determines CEUs based on the setting of the
CellCounterParaGroup.EdgeUserA3Offset parameter, and determines CEUs with
weak coverage based on the setting of the
CellCounterParaGroup.EdgeUserServRSRPThd parameter.
Before activating DL CoMP, run the following command:
MOD CELLCOUNTERPARAGROUP:LocalCellId=0, CellCounterAlgoSwitch=BasedA3EdgeUserSwitch-1,
EdgeUserA3Offset=-12;
This feature requires support from UEs. UEs must be compliant with 3GPP Release
11 or later and capable of TM10 multi-CSI measurement.
To accurately evaluate whether the conditions for enabling DL CoMP are met,
collect the following information before feature deployment:
●  Penetration rate of TM10-capable UEs
Check whether UEs on the network support TM10 based on the
supportedCSIProcr11 field in the external CHR event
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.25

PRIVATE_UE_CAPABILITY_INFORMATION and evaluate the penetration rate of
TM10-capable UEs. For details about this field, see "supportedCSI-Proc-r11" in
"UE-EUTRA-Capability" in section 6.3.6 in 3GPP TS 36.331.
●  Engineering parameters of cells
–   Frequency and bandwidth configurations of cells
–   Inter-site distance and longitude and latitude of each site
–   Hardware information
●  Values of counters related to LTE network load status
## Measurement
## Item
Counter IDCounter Name
Number of UEs
in a cell
1526727378L.Traffic.User.Avg
1526727379L.Traffic.User.Max
1526728969L.Traffic.ActiveUser.DL.Avg
1526728970L.Traffic.ActiveUser.DL.Max
1526728975L.Traffic.ActiveUser.Avg
1526728976L.Traffic.ActiveUser.Max
## Average
number of
PRBs used in
the downlink
1526726740L.ChMeas.PRB.DL.Used.Avg
1526741767L.ChMeas.PRB.PDSCH.Avg.BorderUE

●  Values of counters related to LTE network interference and coverage
performance
## Measurement
## Item
Counter IDCounter Name
Number of cell
edge UEs in a
cell
1526741888L.Traffic.User.BorderUE.Avg
1526741889L.Traffic.User.BorderUE.Max
Number of
times MCS
index n (n = 0
to 31) is
selected for
## PDSCH
scheduling in a
cell
1526727444 to
## 1526727475
L.ChMeas.PDSCH.MCS.0 to
L.ChMeas.PDSCH.MCS.31
Number of
times the
reported
wideband CQI is
n (n = 0 to 15)
in a cell
1526727396 to
## 1526727411
L.ChMeas.CQI.DL.0 to
L.ChMeas.CQI.DL.15
1526737710L.ChMeas.CQI.DL.BorderUE.Total
1526737711L.ChMeas.CQI.DL.BorderUE.Num
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.26

## Measurement
## Item
Counter IDCounter Name
## Counters
related to the
number of
times ranks 1 to
4 are reported
by UEs in a cell
1526730141L.ChMeas.RI.Rank1
1526730142L.ChMeas.RI.Rank2
1526732737L.ChMeas.RI.Rank3
1526732738L.ChMeas.RI.Rank4
## Average
downlink user
data rate in a
cell
1526728261L.Thrp.bits.DL
1526728997L.Thrp.Time.Cell.DL.HighPrecision
1526728262L.Thrp.Time.DL
1526729005L.Thrp.bits.DL.LastTTI
1526729015L.Thrp.Time.DL.RmvLastTTI
Downlink data
rates of cell
edge UEs in a
cell
1526737755L.Thrp.bits.DL.BorderUE
1526741760L.Thrp.Time.DL.BorderUE
1526737758L.Thrp.bits.DL.LastTTI.BorderUE
1526737759L.Thrp.Time.DL.RmvLastTTI.BorderUE

4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Parameters Used for Activation and Parameters Used for Optimization
describe the parameters used for function activation and optimization,
respectively.
Parameters Used for Activation
DL CoMP based on USU3910-based multi-BBU interconnection requires that eX2
links be configured. For details about the parameters required for eX2 link setup,
see
eX2 Self-Management.
The following table describes the parameter that must be set in the
CellAlgoSwitch MO to configure the switches related to DL CoMP.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.27

Table 4-1 Parameter in the CellAlgoSwitch MO
## Parameter
## Name
Parameter IDOptionSetting Notes
## Downlink
CoMP
algorithms
switch
CellAlgoSwit
ch.DlCompS
witch
FDDHomNet
DlCompSwitc
h and
FDDHetNetD
lCompSwitch
Select one or both of them
based on the network
conditions.

The following table describes the parameters that must be set in the
NCellDlRsrpMeasPara MO for coordinating cell set measurement.
Table 4-2 Parameters in the NCellDlRsrpMeasPara MO
## Parameter
## Name
Parameter IDSetting Notes
DL RSRP Auto
NCell
## Measurement
## Switch
NCellDlRsrp
MeasPara.Dl
RsrpAutoNCe
llMeasSwitch
Set this parameter to ON.
## DL RSRP
NCell
## Measurement
## A3 Offset
NCellDlRsrp
MeasPara.NC
ellDlRsrpMea
sA3Offset
Set this parameter to its recommended value.
## DL RSRP
NCell
## Measurement
## A6 Offset
NCellDlRsrp
MeasPara.Dl
RsrpNCellMe
asA6Offset
This parameter is required only in intra-BBU CA
scenarios.
Set this parameter to its recommended value.

The following table describes the parameters that must be set in the
CellCsiRsParaCfg MO for the CSI-RS.
Table 4-3 Parameters in the CellCsiRsParaCfg MO
## Parameter
## Name
Parameter IDSetting Notes
CSI-RS SwitchCellCsiRsPara
Cfg.CsiRsSwit
ch
Before DL CoMP is enabled, set this parameter
to FIXED_CFG or ADAPTIVE_CFG.
If the TM10-capable UE penetration rate is
specified, set this parameter to FIXED_CFG.
Otherwise, it is recommended that this
parameter be set to ADAPTIVE_CFG.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.28

## Parameter
## Name
Parameter IDSetting Notes
CSI-RS PeriodCellCsiRsPara
Cfg.CsiRsPeri
od
Set this parameter to its recommended value.
CSI-RS Config
## User Ratio
## Threshold
CellCsiRsPara
Cfg.CsiRsConf
igUserRatioT
h
Value 70 is recommended.
CSI-RS Config
## User Number
## Threshold
CellCsiRsPara
Cfg.CsiRsConf
igUserNumT
h
Set this parameter to its recommended value.
## CSI-RS
## Unconfig User
## Ratio
## Threshold
CellCsiRsPara
Cfg.CsiRsUnc
onfigUserRat
ioTh
Value 50 is recommended.
## CSI-RS
## Unconfig User
## Number
## Threshold
CellCsiRsPara
Cfg.CsiRsUnc
onfigUserNu
mTh
Set this parameter to its recommended value.
CSI-RS Set
## Judge
## Hysteresis
## Timer
CellCsiRsPara
Cfg.CsiRsSetJ
udgeHysTim
er
Set this parameter to its recommended value.
CSI-RS Set
## Judge Timer
CellCsiRsPara
Cfg.CsiRsSetJ
udgeTimer
Set this parameter to its recommended value.

The following table describes the parameters that must be set in the
CellDlschAlgo MO for downlink scheduling.
Table 4-4 Parameters that must be set in the CellDlschAlgo MO
## Parameter
## Name
Parameter IDOptionSetting Notes
## CSI-RS
## Subframe
## Scheduling
## Strategy
## Switch
CellDlschAlg
o.CsiRsSfSchS
trSwitch
UnconfigCsiRs
UeEnDeOrder
SchSw
You are advised to select this
option.
When this option is selected,
the UnCfgCsiRsUEDeOr-
derSchSwitch option of the
CellDlschAlgo.
CsiRsSfSchStrS
witch parameter must be
deselected.

eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.29

The following table describes the parameter that must be set in the CellUlschAlgo
MO for uplink scheduling.
Table 4-5 Parameter that must be set in the CellUlschAlgo MO
## Parameter
## Name
Parameter IDSetting Notes
## Doppler
## Measurement
## Level
CellUlschAlg
o.DopMeasLe
vel
It is recommended that this parameter be set
to CLASS_1 to obtain more measurement
information.

Parameters Used for Optimization
Table 4-6 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
HetNet DPS
## Coordinating
Cell RSRP
## Threshold
CellDlCompA
lgo.HetnetDp
sCoCellRsrpT
hd
Calculate the ratio of the average number of
downlink DPS UEs (L.Traffic.User.DLDps.Avg)
or average number of JT UEs
(L.Traffic.User.DLJT.Avg) to the average
number of UEs in a cell (L.Traffic.User.Avg).
● If the ratio is higher than 30%, you are
advised to increase the coordinating cell
RSRP threshold (for example, from -6 dB to
-3 dB) to maintain the ratio within 15% to
## 30%.
● If the ratio is lower than 15%, you are
advised to decrease the coordinating cell
RSRP threshold (for example, from -3 dB to
-6 dB) to maintain the ratio within 15% to
## 30%.
For DPS UEs in HetNet scenarios, the
coordinating cell RSRP threshold cannot be
smaller than -6 dB. For DPS and JT UEs in
HomNet scenarios, the coordinating cell RSRP
threshold cannot be smaller than -3 dB.
Otherwise, the correctness of data transmission
is affected.
HomNet DPS
## Coordinating
Cell RSRP
## Threshold
CellDlCompA
lgo.HomnetD
psCoCellRsrp
## Thd
## JT
## Coordinating
Cell RSRP
## Threshold
CellDlCompA
lgo.JtCoCellR
srpThd
## DPS
## Coordinating
## Cell User
## Ratio
## Threshold
CellDlCompA
lgo.DpsCoCel
lUserRatioTh
d
Set this parameter to its recommended value.
A larger value of this parameter leads to more
UEs in coordinating cells and smaller offload
gains to the serving cell. A smaller value of this
parameter leads to fewer UEs in coordinating
cells and larger offload gains to the serving
cell.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.30

## Parameter
## Name
Parameter IDSetting Notes
DPS Serving
cell download
## PRB
## Threshold
CellDlCompA
lgo.DpsServin
gCellDlPrbTh
d
Set this parameter to its recommended value.
A smaller value of this parameter leads to a
lower threshold for a cell to be selected as a
DPS serving cell, increasing the probability of
negative DPS gains. A larger value of this
parameter leads to a higher threshold for a cell
to be selected as a DPS serving cell. In this
case, DPS gains cannot be maximized.
If negative impacts occur after DL CoMP is
enabled and DPS takes effect on the live
network, set this parameter to a larger value.
DPS Load
## Difference
## Threshold
CellDlCompA
lgo.DpsLoad
DiffThd
Set this parameter to its recommended value.
A larger value of this parameter indicates that
more UEs can be transferred to a coordinating
cell in an update interval, significantly
improving the system throughput. However, it
is possible that the eNodeB cannot select a
proper neighboring cell if the value is too
large. A smaller value of this parameter
indicates that fewer UEs can be transferred to
a coordinating cell in an update interval. In this
case, the system throughput does not improve
significantly.
If negative impacts occur after DL CoMP is
enabled and DPS takes effect on the live
network, set this parameter to a larger value.
## JT
## Coordinating
Cell DL PRB
## Threshold
CellDlCompA
lgo.JtCoCellD
lPrbThd
A smaller value of this parameter indicates a
lower threshold for a cell to be selected as a
coordinating cell for JT. In this case, JT gains
cannot be maximized. A larger value of this
parameter indicates a higher threshold for a
cell to be selected as a coordinating cell for JT,
increasing the probability of negative JT gains.
Set this parameter to its recommended value.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.31

## Parameter
## Name
Parameter IDSetting Notes
JT Serving
Cell DL PRB
## Threshold
CellDlCompA
lgo.JtServing
CellDlPrbThd
A smaller value of this parameter indicates a
lower threshold for a cell to be selected as a JT
serving cell, reducing the number of cells that
perform JT. In this case, JT gains decrease. A
larger value of this parameter indicates a
higher threshold for selecting a JT serving cell,
increasing interference caused by JT and
interference to neighboring cells. In this case,
the system throughput is affected.
Set this parameter to the recommended value
on the live network.
Set this parameter to 100 during fixed point
tests.
DL CoMP
## Report
## Interval
CellDlCompA
lgo.DlCompR
eportInterval
Set this parameter to its recommended value.
When UL CoMP takes effect, the reporting
interval of DL CoMP measurement reports is
subject to the reporting interval of UL CoMP
measurement reports.
DL CoMP
## Scheduling
## Priority Factor
CellDlCompA
lgo.DlCompS
chPriFactor
Set this parameter to its recommended value.
## MBSFN
## Subframe
## Configuration
CellDlschAlg
o.MbsfnSfCfg
In scenarios where the TM10-capable UE
penetration rate approaches 100% or in
demonstration scenarios, it is recommended
that this parameter be set to the maximum
number of MBSFN subframes (including
subframes 1, 2, 3, 6, 7, and 8) for cells with DL
CoMP enabled to offset TM10 demodulation
reference signal (DMRS) overheads and reduce
cell-specific reference signal (CRS) interference.
DL CoMP requires that the MBSFN subframe
configurations for all cells be consistent.

4.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.32

## Activation Command Examples
## NO TICE
● All cells with this feature enabled must have the same DL CoMP configurations.
● This feature is implemented on the basis of TM10. CSI-RSs must be configured
(using the CellCsiRsParaCfg MO) in all the cells with this feature enabled.
When USU3910-based multi-BBU interconnection is adopted, configure eX2
interfaces. For details, see
eX2 Self-Management.
//Enabling cell-level automatic measurement of neighboring cell downlink RSRP
MOD NCELLDLRSRPMEASPARA: LocalCellId=0, DlRsrpAutoNCellMeasSwitch=ON,
DlRsrpNCellMeasA6Offset=-12;
//Turning on the DL CoMP algorithm switch
MOD CELLALGOSWITCH: LocalCellId=0,
DlCompSwitch=FDDHetNetDlCompSwitch-1&FDDHomNetDlCompSwitch-1;
//Setting CSI-RS-related parameters
MOD CELLCSIRSPARACFG: LocalCellId=0, CsiRsSwitch=ADAPTIVE_CFG, CsiRsPeriod=ms20,
CsiRsConfigUserNumTh=10, CsiRsUnconfigUserNumTh=200, CsiRsConfigUserRatioTh=70,
CsiRsUnconfigUserRatioTh=50, CsiRsSetJudgeHysTimer=600, CsiRsSetJudgeTimer=600;
//Setting downlink scheduling-related parameters
MOD CELLDLSCHALGO: LocalCellId=0,
CsiRsSfSchStrSwitch=UnCfgCsiRsUEDeOrderSchSwitch-0&UnconfigCsiRsUeEnDeOrderSchSw-1;
//Modifying cell-level DL CoMP parameters
MOD CELLDLCOMPALGO:LocalCellId=0,HetnetDpsCoCellRsrpThd=-12, DpsCoCellUserRatioThd=50,
DpsLoadDiffThd=20, DpsServingCellDlPrbThd=40, HomnetDpsCoCellRsrpThd=-6, JtCoCellRsrpThd=-6,
JtCoCellDlPrbThd=20, JtServingCellDlPrbThd=100, DlCompSchPriFactor=1;
//Setting uplink scheduling-related parameters
MOD CELLULSCHALGO: LocalCellId=0, DopMeasLevel=CLASS_1;
//Setting the reporting interval of event A3 or A6 for DL CoMP
MOD CELLDLCOMPALGO: LocalCellId=0, DlCompReportInterval=1024MS;
## Deactivation Command Examples
//(Optional) Turning off the CSI-RS configuration switch when deactivating DL CoMP with TM10 if only this
feature is enabled on the network (other features based on TM9 and TM10 transmission modes are
disabled)
MOD CELLCSIRSPARACFG: LocalCellId=0, CsiRsSwitch=NOT_CFG;
//Turning off the DL CoMP switch
MOD CELLALGOSWITCH: LocalCellId=0,
DlCompSwitch=FDDHetNetDlCompSwitch-0&FDDHomNetDlCompSwitch-0;
//(Optional) Disabling cell-level automatic measurement of neighboring cell downlink RSRP if eCSPC and
adaptive ICIC are not enabled
MOD NCELLDLRSRPMEASPARA: LocalCellId=0, DlRsrpAutoNCellMeasSwitch=OFF;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
Perform the following steps:
Step 1On the eNodeB side, run the DSP CELLDLCOMPCOCELLS command to query the
value of Cell DL CoMP Property.
Expected result: The value of Cell DL CoMP Property is
CELL_STATUS_TYPE_TM10_DPS_IN, CELL_STATUS_TYPE_TM10_JT_IN, or
CELL_STATUS_TYPE_TM9TM10_JT_IN, and there are coordinating cells.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.33

Step 2Log in to the MAE-Access and choose Monitoring > Signaling Trace > Signaling
Trace Management. In the displayed window, choose Cell Performance
Monitoring > DL CoMP Monitoring in the navigation tree. In the displayed dialog
box, select the target eNodeB and create a DL CoMP monitoring task that
monitors the number of UEs that benefit from DPS or JT. Observe the number of
times JT UEs in the local cell are scheduled in coordinating cells.
Expected result: The value of DPS Benefit User Number or JT Benefit User
Number is not zero. This result shows that this feature has taken effect.
----End
## 4.4.3 Network Monitoring
The gains offered by this feature can be observed using the following methods.
## Using Counters
Observe the counters listed in the following table before and after activating this
feature. The changes in the counter values reflect feature performance.
Counter IDCounter Name
1526743727L.Traffic.User.DLDps.Avg
1526743728L.Traffic.User.DLJT.Avg
1526749462L.Traffic.User.SCell.Active.DLJT.Avg
1526743725L.ChMeas.PRB.DL.DPS.Used.Avg.Othe
rCell
1526743726L.ChMeas.PRB.DL.JT.Used.Avg.OtherC
ell
1526727444 to 1526727475L.ChMeas.PDSCH.MCS.0 to
L.ChMeas.PDSCH.MCS.31

Observe the following indicators before and after activating this feature. The
changes in the values reflect feature gains.
## NO TICE
Before observing the downlink average user-perceived rate and the user-perceived
rate at the cell edge, run the MOD CELLCOUNTERPARAGROUP command to turn
on switches related to cell-level performance measurement.
MML command example:
MOD CELLCOUNTERPARAGROUP: LocalCellId=0, CellCounterAlgoSwitch=BasedA3EdgeUserSwitch-1,
EdgeUserA3Offset=-12;
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.34

IndicatorFormulaExpected Result
Downlink average
perceived rate
(L.Thrp.bits.DL –
L.Thrp.bits.DL.LastTTI)/
L.Thrp.Time.DL.RmvLast
## TTI
The average downlink
user-perceived data rate
increases or remains
unchanged after feature
activation.
Average downlink CEU
throughput
(L.Thrp.bits.DL.BorderU
## E –
L.Thrp.bits.DL.LastTTI.B
orderUE)/
L.Thrp.Time.DL.RmvLast
TTI.BorderUE
The average downlink
CEU throughput
increases after feature
activation.

## Using Signaling Tracing
●  Cell-level performance monitoring
a.  On the MAE-Access, choose Monitor > Signaling Trace > Signaling
## Trace Management.
b.  In the displayed window, choose Cell Performance Monitoring > DL
CoMP (Cell) Monitoring in the navigation tree and select the target
eNodeB to create a monitoring task.
c.  Observe the number of beneficiary UEs and the number of RBs used in
the serving cell and coordinating cell.
●  UE-level performance monitoring
a.  On the MAE-Access, choose Monitor > Signaling Trace > Signaling
## Trace Management.
b.  In the displayed window, choose User Performance Monitoring > DL
CoMP (User) Monitoring in the navigation tree and select a target user
to create a monitoring task.
c.  Observe the following items in the tracing result:
## ▪
Coordinating Cell's Local Cell ID
## ▪
UE Code Count of Coordinating Cell
▪CoCell CQI
▪CoCell DLSCH Code0 Num/CoCell DLSCH Code1 Num
▪CoCell DLSCH Code0 RBs/CoCell DLSCH Code1 RBs
## 4.4.4 Possible Issues
If the number of UEs that benefit from DPS and JT is zero, or the CEU throughput
of the entire network does not increase after this feature is activated, perform the
following steps:
Step 1Run the LST CELLALGOSWITCH command to check whether the DL CoMP
algorithm switch is turned on.
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.35

●  If yes, go to Step 2.
●  If no, configure parameters by referring to 4.4.1.1 Data Preparation.
Step 2Run the DSP CELLDLCOMPCOCELLS command to check whether DL CoMP has
taken effect.
●  If yes, check whether there is a coordinating cell list.
–   If yes, go to Step 3.
–   If no, check whether intra-frequency neighbor relationships have been
established between the local cell and neighboring cells. Check whether
there are CEUs in the cell by observing the L.Traffic.User.BorderUE.Avg
counter. Check whether the DL CoMP switch has been turned on for more
than one hour.
●  If no, check whether the local cell meets the thresholds for entering DL CoMP,
including:
–CellCsiRsParaCfg.
CsiRsConfigUserRatioTh
–CellCsiRsParaCfg.CsiRsUnconfigUserRatioTh
–CellDlCompAlgo.JtCoCellDlPrbThd and
CellDlCompAlgo.
JtServingCellDlPrbThd
Step 3Check the following performance counters to see whether the DPS or JT UE
proportion is too low, for example, lower than 15%.
Counter ID
Counter NameDescription
1526743727L.Traffic.User.DLD
PS.Avg
Average number of downlink DPS UEs
in a cell
1526743728L.Traffic.User.DLJT.
## Avg
Average number of downlink JT UEs in
a cell

●  If no, go to Step 4.
●  If yes, the number of DPS or JT UEs is too small. In this case, DL CoMP cannot
offer noticeable gains to increase the UE quantity and data rate.
Step 4If the preceding steps fail to resolve the problem, contact Huawei technical
support.
----End
eRAN
DL CoMP (FDD) Feature Parameter Description4 DL CoMP with TM10
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.36

5 DL CoMP with TM9
## 5.1 Principles
Figure 5-1 shows the process of DL CoMP with TM9, including selection of a TM9
JT coordinating cell set, selection of TM9 JT UEs and coordinating cells, and multi-
cell coordinated transmission.
Figure 5-1 Process of DL CoMP with TM9
This function is controlled by the Tm9JtSwitch option of the
CellAlgoSwitch.
DlCompSwitch parameter. This option is selected by default.
5.1.1 Selection of a TM9 JT Coordinating Cell Set
The eNodeB selects a TM9 JT coordinating cell set using either of the following
methods:
●  Automatic selection of intra-eNodeB intra-frequency neighboring cells:
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.37

If the NCellDlRsrpMeasPara.DlRsrpAutoNCellMeasSwitch parameter is set
to OFF, the eNodeB automatically selects intra-eNodeB intra-frequency
neighboring cells to form a TM9 JT coordinating cell set. TM9 JT can be
performed on intra-eNodeB CEUs that meet the event A3 and A6 reporting
conditions.
●  Selection of neighboring cells based on neighboring cell measurement:
If the NCellDlRsrpMeasPara.DlRsrpAutoNCellMeasSwitch parameter is set
to ON, the eNodeB periodically collects neighboring cell information of UEs
that meet the A3 and A6 reporting conditions every hour, and 10 neighboring
cells that cause the highest interference to the serving cell to form the TM9 JT
coordinating cell set. If micro cells exist, the eNodeB preferentially selects
micro cells (6 at most), and then selects macro cells to form a coordinating
cell set.
Settings related to A3 and A6 measurements are specified by the
NCellDlRsrpMeasPara.
NCellDlRsrpMeasA3Offset and
NCellDlRsrpMeasPara.DlRsrpNCellMeasA6Offset parameters, respectively.
5.1.2 Selection of TM9 JT UEs and Coordinating Cells
After the JT serving cell is selected, the serving cell selects TM9 JT UEs based on
the event A3 measurement data reported by the UE and RSRP threshold, and
determines coordinating cells.
5.1.2.1 Entering the JT Mode
The process for a UE to enter the JT mode is as follows:
-  JT serving cell selection is triggered.
When the PRB usage of the serving cell is less than or equal to the threshold
specified by the CellDlCompAlgo.
JtServingCellDlPrbThd parameter, the
eNodeB selects the serving cell as the JT serving cell.
-  The eNodeB selects the cells with the strongest RSRP in the coordinating cell
set as coordinating cells.
If the RSRP of a neighboring cell of the UE minus that of the serving cell of
the UE is greater than or equal to the value of the
CellDlCompAlgo.
JtCoCellRsrpThd parameter plus the coordinating cell RSRP
offset, and the neighboring cell belongs to the coordinating cell set, it is
selected as a coordinating cell.
–   In HomNet networking scenarios, only the cells of the same site type as
the serving cell and with the strongest RSRP in the coordinating cell set
can be selected as coordinating cells.
–   In HetNet networking scenarios, when the serving cell is a macro cell,
only the micro cells with the strongest RSRP in the coordinating cell set
can be selected as coordinating cells.
–   In HomNet and HetNet hybrid networking scenarios, the cells with the
strongest RSRP in the coordinating cell set are preferentially selected as
coordinating cells.
## NO TE
The system automatically configures the coordinating cell RSRP offset to prevent ping-
pong configuration of TM9 for UEs.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.38

-  The eNodeB selects JT UEs.
If the coordinating cells selected in 2 meet all of the following conditions, the
eNodeB selects the UEs as JT UEs and configures the TM9 mode for them.
–   The PRB usage of a coordinating cell is less than the value of the
CellDlCompAlgo.JtCoCellDlPrbThd parameter.
–   When the UE is a 256QAM UE, the spectral efficiency corresponding to
the CQI for each codeword reported by the UE is lower than that
corresponding to CQI 4. For details about CQI 4, see "Table 7.2.3-2 4-bit
CQI Table 2" in section 7.2.3 "Channel Quality Indicator (CQI) definition"
in 3GPP TS 36.213 V12.9.1.
–   When the UE is a non-256QAM UE, the spectral efficiency corresponding
to the CQI for each codeword reported by the UE is lower than that
corresponding to CQI 7. For details about CQI 7, see "Table 7.2.3-1 4-bit
CQI Table" in section 7.2.3 "Channel Quality Indicator (CQI) definition" in
## 3GPP TS 36.213 V12.9.1.
5.1.2.2 Exiting the JT Mode
If a JT UE reports exit event A3, the eNodeB disables TM9 configuration for the UE
and configures the UE as a common user.
5.1.3 Multi-Cell Coordinated Transmission
As shown in Figure 5-2, the eNodeB of the serving cell delivers a set of CSI
measurement configurations to a TM9 JT UE for measuring the CSI, including the
PMI, RI, and CQI, of the serving and coordinating cells. The eNodeB of the serving
cell transmits data in JT mode based on the CSI measurement result reported by
the UE and the scheduling information of the serving and coordinating cells.
The reporting mode used by the TM9 JT UE is determined by determining whether
both of the following conditions are met:
●  The Pusch32Switch option of the CellAlgoSwitch.
DlSchSwitch parameter is
selected.
●  The TM9 JT UE supports the PUSCH3-2 feedback mode.
If yes, the TM9 JT UE uses the PUSCH3-2 feedback mode. If not, the TM9 JT UE
uses the aperiodic CSI reporting mode (PUSCH1-2 feedback mode). This mode
does not depend on the PUSCH12Switch option of the
CellAlgoSwitch.
EmimoSwitch parameter.
For details about the PUSCH3-2 and PUSCH1-2 feedback modes, see eMIMO
## (FDD)
## .
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.39

Figure 5-2 CSI configuration for a TM9 JT UE
## NO TE
DL CoMP with TM9 supports coordinated transmission of only 2T+2T cells. Each cell uses
two ports (cell 1 uses ports 15 and 16, and cell 2 uses ports 17 and 18) to perform four-
port CSI-RS transmission (ports 15, 16, 17, and 18), as shown in Figure 5-2.
## 5.2 Network Analysis
## 5.2.1 Benefits
## Gains
This feature improves the downlink throughput and user experience of CEUs.
## Most Beneficial Scenarios
This feature is recommended when all of the following conditions are met:
●  The inter-site distance is less than 500 m in densely populated urban areas.
●  The average downlink PRB usage of cells is less than 20% in light-load
scenarios.
●  The proportion of UEs with the MCS index less than 13 is greater than 20%
when the cells have different PCI mod 3 values.
●  Most UEs on the network are stationary or moving at low speeds.
●  The penetration rate of TM9-capable UEs exceeds 20%.
## 5.2.2 Impacts
## Network Impacts
●  2T+2T: When the PRB usage of a cell is less than 20%, the downlink perceived
rate of JT UEs at the cell edge increases by 5–25%. The lower the SINR, the
higher the gain. (The gain varies according to the delta RSRP. It is
recommended that the gain be within –3 dB. When the serving cell and the
coordinating cell have different PCI mod 3 values, the MCS index of the UE
that does not enter the JT mode is less than 13.)
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.40

●  If aperiodic CQI reporting is used, this function will slightly increase the uplink
PRB usage of the serving cell.
●  In JT mode, the serving cell determines whether a UE is a CEU based on event
A3. In this case, the value returned by the L.MeasRpts.IntraFrequency
counter may increase.
## Function Impacts
## Function
## Name
Function SwitchReferenceDescription
VoIP
semi-
persistent
schedulin
g
Uplink: SpsSchSwitch
option of the
CellAlgoSwitch.UlSch
Switch parameter
## Downlink:
SpsSchSwitch option
of the
CellAlgoSwitch.
DlSch
## Switch
parameter
VoLTEResource conflicts may occur
between semi-persistent
scheduling and TM9 JT
coordinating cell scheduling.
Therefore, DL CoMP
coordinating cell scheduling is
not performed within the TTI
in which semi-persistent
scheduling is effective.
MROCellAlgoSwitch.MroS
witch
MROMRO may affect the optimal
RSRP threshold setting of
coordinating cells in DL
CoMP. As a result, the cell-
edge throughput across the
entire network cannot reach
the optimal level that DL
CoMP can achieve.
## Enhanced
downlink
frequency
selective
schedulin
g
FreqSelSwitch option
of the
CellAlgoSwitch.DlSch
Switch parameter
SchedulingFrequency-selective
scheduling can be performed
for TM9 JT UEs only in the
serving cell.
## Symbol
power
saving
SymbolShutdownS-
witch option of the
ENodeBAlgoSwitch.P
owerSaveSwitch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
When both DL CoMP with
TM9 and symbol power
saving are enabled, symbol
power saving is not triggered
in the coordinating cells for
DL CoMP with TM9 during
scheduling in these cells.
ePDCCH
## (trial)
CellPdcchAlgo.Epdcc
hAlgoSwitch
## Physical
## Channel
## Resource
## Managem
ent
When both DL CoMP with
TM9 and ePDCCH are
enabled, a UE configured
with ePDCCH cannot be
selected as a TM9 JT UE. As a
result, DL CoMP with TM9
cannot achieve optimal
performance.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.41

## Function
## Name
Function SwitchReferenceDescription
## Emergenc
y call
NoneEmergency
## Call
UEs making emergency calls
cannot be selected as TM9 JT
UEs. As a result, DL CoMP
with TM9 cannot achieve
optimal performance.
## Coordinat
ed
schedulin
g-based
power
control
## CSPC:
CellCspcPara.CellCsp
cSwitch
eCSPC:
CellCspcPara.CelleCs
pcSwitch
Intra-eNodeB CSPC:
CellCspcPara.IntraEn
bCspcSw
CSPC● DL CoMP with TM9 and
CSPC (controlled by
CellCspcPara.CellCspcSwi
tch) can be enabled
simultaneously, but CSPC
takes effect preferentially.
If CSPC has taken effect in
a cell, DL CoMP UEs are
not scheduled in
coordinating cells.
● DL CoMP with TM9 and
eCSPC (controlled by
CellCspcPara.
CelleCspcSw
itch
) cannot be enabled
simultaneously.
SFNUplink:
CellAlgoSwitch.SfnUl
SchSwitch
## Downlink:
CellAlgoSwitch.
SfnDl
SchSwitch
SFNIf the antenna modes of the
physical cells forming an SFN
cell are different, the SFN cell
cannot be selected as a
coordinating cell for DL
CoMP. DL CoMP with TM9
cannot be used in the SFN
cell.
## Adaptive
## SFN/
## SDMA
## Uplink:
CellAlgoSwitch.SfnUl
SchSwitch
## Downlink:
CellAlgoSwitch.
SfnDl
SchSwitch
SFNDL CoMP with TM9 and
adaptive SFN/SDMA can be
enabled simultaneously.
However, the joint scheduling
mode is always used for UEs
in coordinating cells because
the serving cell does not have
RSRP information about the
RRUs serving neighboring
cells and cannot determine
UE attributes.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.42

## Function
## Name
Function SwitchReferenceDescription
eMTC
introducti
on
## EMTC_SWITCH
option of the
CellEmtcAlgo.EmtcAl
goSwitch parameter
eMTCeMTC UEs do not support DL
CoMP with TM9.
If the
CellCsiRsParaCfg.CsiRsSwitc
h parameter is set to
ADAPTIVE_CFG for a cell
after DL CoMP with TM9 is
enabled in this cell, CSI-RSs
will be adaptively transmitted
based on the proportion of
TM9-capable UEs in this cell.
The CSI-RS transmission
change will indirectly cause
system information updates
for eMTC. This issue can be
resolved by selecting the
## EMTC_CSI_RS_OPT_SWITCH
option of the
CellEmtcAlgo.
EmtcAlgoSwit
ch parameter.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.43

## Function
## Name
Function SwitchReferenceDescription
## DL
## 256QAM
Dl256QamSwitch
option of the
CellAlgoSwitch.Dl256
QamAlgoSwitch
parameter
## Modulatio
n Schemes
● If the
CellDlschAlgo.Dl256Qam
CqiTblCfgStrategy
parameter is set to
ADAPTIVE_CONFIG or
## CQI_BASED_ADAPTIVE_C
ONFIG, JT UEs can be
selected as 256QAM UEs,
and non-JT UEs with
256QAM cannot be
selected as JT UEs. This is
because non-JT UEs can be
selected as 256QAM UEs
only when the SINR is high
in adaptive configuration
mode.
● If the
CellDlschAlgo.
Dl256Qam
CqiTblCfgStrategy
parameter is set to
FIX_CONFIG for the
serving cell, JT UEs can be
selected as 256QAM UEs,
and non-JT UEs with
256QAM can be selected
as JT UEs.
For details about 256QAM
UEs, see "Table 7.2.3-2 4-bit
CQI Table 2" in section
"Channel quality indicator
(CQI) definition" in 3GPP TS
36.213. The 256QAM UEs
mentioned earlier are UEs for
which this CQI table is
selected.
TM9 JT can be performed
only when the DL 256QAM
switch settings of the serving
cell and coordinating cells are
the same.
## Dynamic
## Power
## Sharing
## Between
## LTE
## Carriers
## LTE_DYN_POWER_SH
ARING_SW option of
the
CellDynPowerShar-
ing.DynamicPowerSh
aringSwitch
parameter
## Dynamic
## Power
## Sharing
## Between
## LTE
## Carriers
Jointly scheduled JT UEs do
not share power.
Independently scheduled JT
UEs can share power.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.44

## Function
## Name
Function SwitchReferenceDescription
## Downlink
## 2CC
aggregati
on
NoneCarrier
## Aggregatio
n
TM9 JT can be configured in
both the PCells and SCells of
UEs in the intra-BBU CA
state.
TM9 JT in SCells takes effect
only after TM9 JT is
configured in the
corresponding PCells.
## Downlink
## FDD+TDD
## CA
InterFddTddCaSwitch
option of the
CaMgtCfg.CellCaAlgo
Switch parameter
## Carrier
## Aggregatio
n
TM9 JT can be configured in
both the PCells and SCells of
UEs in the intra-BBU CA
state.
TM9 JT in SCells takes effect
only after TM9 JT is
configured in the
corresponding PCells.
DL CoMP
with
## TM10
FDDHomNetDlComp
Switch or
FDDHetNetDlCompS-
witch option of the
CellAlgoSwitch.DlCo
mpSwitch
parameter
DL CoMP
## (FDD)
If both DL CoMP with TM10
and DL CoMP with TM9 are
enabled and the conditions
for both TM10 JT and TM9 JT
to take effect are met, UEs
are preferentially configured
to work in TM9 mode.
## Static
## Multiple
## Beam
None3D
## Beamform
ing (FDD)
When inner and outer cells
generated using vertical
multiple sectors (VMS) are
working for CoMP, the cell
power setting must be
reduced by half. This affects
network performance.
## Precise
## AMC
PreciseAmcSwitch
option of the
CellAlgoSwitch.Emim
oSwitch parameter
eMIMO
## (FDD)
Enabling DL CoMP affects the
accuracy of calculated
interference from neighboring
cells and further affects the
performance of precise AMC.
Therefore, you are advised to
disable precise AMC when DL
CoMP is enabled.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.45

## Function
## Name
Function SwitchReferenceDescription
## NPREO
constant
optimizati
on
CellDlpcPdschPa.UeN
preoAdjThreshold
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
the accuracy of neighboring
cell interference calculation is
affected and the performance
of UE-level NPREO constant
optimization is affected.
Therefore, you are advised
not to enable UE-level
NPREO constant
optimization.
## Downlink
target
## IBLER
adaptatio
n
DlVarIBLERtargetS-
witch option of the
CellAlgoSwitch.CqiA
djAlgoSwitch
parameter
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
aperiodic CQI reporting is
used, which affects the
accuracy of the downlink
target IBLER adaptation
algorithm. Therefore, when
both DL CoMP and downlink
target IBLER adaptation are
enabled, downlink target
IBLER adaptation does not
take effect for JT UEs.
## Enhanced
downlink
target
## IBLER
adaptatio
n
DlEnVarIblerTargetS-
witch option of the
CellAlgoSwitch.CqiA
djAlgoSwitch
parameter
## Channel
## State
## Managem
ent
When DL CoMP is enabled,
aperiodic CQI reporting is
used, which affects the
accuracy of enhanced
downlink target IBLER
adaptation. Therefore, when
both DL CoMP and enhanced
downlink target IBLER
adaptation are enabled,
enhanced downlink target
IBLER adaptation does not
take effect for JT UEs.
## High
speed
mobility
Cell.HighSpeedFlagHigh
## Speed
## Mobility
In high-speed mobility
scenarios, channel conditions
and cell load change so
rapidly that DL CoMP with
TM9 cannot be promptly
performed. Therefore, DL
CoMP with TM9 cannot take
effect in high-speed mobility
scenarios.
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh
## Speed
## Mobility
## Extended
## CP
Cell.DlCyclicPrefixExtended
## CP
If extended CP is used, DL
CoMP with TM9 does not
take effect.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.46

## Function
## Name
Function SwitchReferenceDescription
## Dynamic
## TDM
eICIC
CellAlgoSwitch.EicicS
witch
TDM eICIC
## (FDD)
Both DL CoMP with TM9 and
eICIC can improve the cell
edge performance. You are
advised not to enable both of
them.
FeICICCellAlgoSwitch.Feicic
## Switch
TDM eICIC
## (FDD)
## Adaptive
inter-cell
interferen
ce
coordinati
on
NoneAdaptive
## ICIC
Adaptive ICIC is based on the
eCoordinator architecture. DL
CoMP with TM9 cannot
obtain the frequency band
divisions of neighboring cells
where adaptive ICIC takes
effect. In this case, DL CoMP
with TM9 cannot coordinate
UEs to neighboring cells for
scheduling. Therefore, DL
CoMP with TM9 cannot take
effect when it is enabled
together with adaptive ICIC.
eCSPCCellCspcPara.CelleCs
pcSwitch
CSPCeCSPC adjusts power among
cells to reduce interference
and applies to heavy-load
scenarios. The gain source
and application scenarios of
eCSPC are different from
those of JT. DL CoMP with
TM9 cannot take effect when
both DL CoMP with TM9 and
eCSPC are enabled.
## 4x4
MIMO in
the
overlappi
ng areas
between
the
physical
cells of an
SFN cell
SfnJtSwitch option of
the
CellAlgoSwitch.SfnAl
goSwitch parameter
SFNIt is recommended that DL
CoMP with TM9 not be
enabled together with 4x4
MIMO in the overlapping
areas between the physical
cells of an SFN cell due to
issues related to CSI-RS
cooperation between
features.
## Inter-
eNodeB
## SFN
based on
eNodeB
coordinati
on
Cell.EuCellStandbyM
ode
SFNDL CoMP with TM9 does not
take effect in inter-BBU SFN
scenarios.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.47

## Function
## Name
Function SwitchReferenceDescription
## Adaptive
## SFN/
## SDMA
with
## TM9/
## TM10
TM9Switch option of
the
CellAlgoSwitch.EnhM
IMOSwitch
parameter
SFNDL CoMP with TM9, when
enabled together with
adaptive SFN/SDMA with
TM9, cannot take effect.
## Adaptive
## SFN/
## SDMA
with
## TM9/
## TM10
TM10Switch option
of the
CellAlgoSwitch.EnhM
IMOSwitch
parameter
SFNDL CoMP with TM9, when
enabled together with
adaptive SFN/SDMA with
TM10, cannot take effect.
## Downlink
## MU-
MIMO in
## TM9
4TxTM9MuMimoSwit
ch option of the
CellAlgoSwitch.Emim
oSwitch parameter
eMIMO
## (FDD)
Downlink MU-MIMO in TM9
applies to heavy-load
scenarios while JT applies to
light-load scenarios. DL CoMP
with TM9 cannot take effect
when both DL CoMP with
TM9 and downlink MU-
MIMO in TM9 are enabled.
WTTx
## MU-
## MIMO
Tm9FourLayerPairSw
itch option of the
CellAlgoExtSwitch.W
ttxMuMimoSwitch
parameter
WTTx MU-
## MIMO
## (FDD)
DL CoMP with TM9 cannot
take effect when both DL
CoMP with TM9 and WTTx
MU-MIMO are enabled.
## LTE FDD
and NR
## Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.Spect
rumCloudSwitch set
to
## LTE_NR_SPECTRUM_S
## HR
## LTE FDD
and NR
## Spectrum
## Sharing
When both DL CoMP with
TM9 and LTE FDD and NR
## Flash Dynamic Spectrum
Sharing are enabled, DL
CoMP with TM9 cannot take
effect.
## RF
channel
dynamic
muting
## RF_CHN_DYN_MUTIN
G_SW option of the
CellRfChnDynMut-
ing.RfChnDynMuting
AlgoSwitch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
RF channel dynamic muting
does not take effect when
there are TM9 JT UEs in the
cell.
## Energy
saving
based on
flexible
frequency
## -domain
schedulin
g
## FLEX_FREQ_SCH_ENE
## RGY_SAVING_SW
option of the
CellPwrSavingAl-
go.PwrSavingAlgoSw
itch
parameter
## Energy
## Conservati
on and
## Emission
## Reduction
Energy saving based on
flexible frequency-domain
scheduling is not performed
for TM9 JT UEs.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.48

## Function
## Name
Function SwitchReferenceDescription
## Next
## Generatio
n eCall
over LTE
NG_ECALL_SW option
of the
Emc.EmergCallOptim
izationSw parameter
## Emergency
## Call
UEs making emergency calls
cannot be selected as TM9 JT
UEs. As a result, DL CoMP
with TM9 cannot achieve
optimal performance.
## Dynamic
## Massive
## Beam
NoneSmart
## 8T8R
## (FDD)
DL CoMP with TM9 does not
take effect when Dynamic
Massive Beam is enabled.
## Static
## Multiple
## Beam
NoneSmart
## 8T8R
## (FDD)
DL CoMP with TM9 does not
take effect when Static
Multiple Beam is enabled.

## 5.3 Requirements
## 5.3.1 Licenses
There are no license requirements for basic functions.
## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## Function
## Name
Function SwitchReferenceDescription
## Synchronizati
on with GPS
NoneSynchroniz
ation
If DL CoMP with TM9 is
performed among BBUs, time
synchronization is required
across the entire network. In
this scenario, DL CoMP with
TM9 requires either of the
two functions.
## IEEE1588 V2
clock
synchronizati
on
NoneSynchroniz
ation

eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.49

## Mutually Exclusive Functions
## Function
## Name
Function SwitchReferenceDescription
## Adaptive
power
allocation for
cell-edge UEs
AdptCellEdgePwr
AllocSw option of
the
CellAlgoSwitch.Ce
llDlCoverEnhance
## Switch
parameter
SchedulingAdaptive power allocation for
cell-edge UEs does not take
effect for TM9 JT UEs.
Extended cell
range
Cell.CellRadiusExtended
## Cell Range
In DL CoMP with TM9, UEs
need to receive data from
different cells simultaneously.
Therefore, DL CoMP with
TM9 does not apply to
extended coverage scenarios.
Virtual 4T4RVirtual4T4RSwitc
h option of the
CellAlgoSwitch.E
mimoSwitch
parameter
## Virtual
## 4T4R
## (FDD)
Currently, DL CoMP with TM9
is not supported in virtual
4T4R scenarios.
TM4 and
## TM6
## Adaptation
## CL_TM_ADAPTATI
## ON_OPT_SW
option of the
CellMimoParaCfg.
MimoSwitch
parameter
Low-Band
## Booster
TM4 and TM6 Adaptation is
incompatible with DL CoMP
with TM9.

## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
The following base stations are compatible with this function:
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  USU3910
## Boards
●  BBU: The BBU5900A/BBU5900/BBU3900/BBU3910/BBU3910A/BBU3910C
supports this function. When the BBU3910A is used, only intra-BBU DL CoMP
is supported, and inter-BBU DL CoMP is not supported.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.50

●  BBP: The LBBP does not support this function.
●  Main control board: A UMPT must be configured to support this function.
RF Modules
Micro cells in DL CoMP are those served by low-power RRUs, such as the
RRU3220E and RRU3230E.
## Cells
●  Both the serving cell and coordinating cell must support 2T.
●  The Cell.CrsPortNum settings of the cells where this function is enabled are
the same.
## 5.3.4 Networking
●  If inter-BBU DL CoMP is used, the Cloud BB network using USU3910-based
multi-BBU interconnection must be deployed.
–   For details about Cloud BB networking, see
Cloud BB Overview.
–   For details about the networking, cable connections, and clock
synchronization for the USU3910-based Cloud BB architecture, see
USU3910-based Multi-BBU Interconnection.
●  eNodeBs provide contiguous coverage with the same frequency and
bandwidth. The cell bandwidth must be greater than or equal to 5 MHz. It is
recommended that the bandwidth be greater than 5 MHz even if the function
supports the 5 MHz bandwidth.
●  The PDSCHCfg.
Pb parameter must be set to the same value for the serving
cell and coordinating cell where this feature is enabled.
●  If inter-BBU DL CoMP is used, time synchronization is required across the
entire network. The time synchronization accuracy between all cells with DL
CoMP to be enabled must be less than 500 ns, and GPS or IEEE 1588V2
synchronization can be used. For details, see
## Synchronization.
## 5.3.5 Others
## NO TICE
The performance counters of CEUs can be obtained only when the
BasedA3EdgeUserSwitch option of the
CellCounterParaGroup.CellCounterAlgoSwitch parameter is selected. The
eNodeB determines CEUs based on the setting of the
CellCounterParaGroup.EdgeUserA3Offset parameter, and determines CEUs with
weak-coverage based on the setting of the
CellCounterParaGroup.EdgeUserServRSRPThd parameter.
Before activating DL CoMP, run the following command:
MOD CELLCOUNTERPARAGROUP:LocalCellId=0, CellCounterAlgoSwitch=BasedA3EdgeUserSwitch-1,
EdgeUserA3Offset=-12;
This feature requires support from UEs. UEs must be compliant with 3GPP Release
10 or later and capable of TM9 multi-CSI measurement.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.51

To accurately evaluate whether the conditions for enabling DL CoMP are met,
collect the following information before feature deployment:
●  Penetration rate of TM9-capable UEs
Penetration rate of TM9-capable UEs in a cell =
L.Traffic.User.TM9Capability.Avg/L.Traffic.User.Avg
●  Engineering parameters of cells
–   Frequency and bandwidth configurations of cells
–   Inter-site distance and longitude and latitude of each site
–   Hardware information
●  Values of counters related to LTE network load status
## Measurement
## Item
Counter IDCounter Name
Number of UEs
in a cell
1526727378L.Traffic.User.Avg
1526727379L.Traffic.User.Max
1526728969L.Traffic.ActiveUser.DL.Avg
1526728970L.Traffic.ActiveUser.DL.Max
1526728975L.Traffic.ActiveUser.Avg
1526728976L.Traffic.ActiveUser.Max
## Average
number of
PRBs used in
the downlink
1526726740L.ChMeas.PRB.DL.Used.Avg
1526741767L.ChMeas.PRB.PDSCH.Avg.BorderUE

●  Values of counters related to LTE network interference and coverage
performance
## Measurement
## Item
Counter IDCounter Name
Number of cell
edge UEs in a
cell
1526741888L.Traffic.User.BorderUE.Avg
1526741889L.Traffic.User.BorderUE.Max
Number of
times MCS
index n (n = 0
to 31) is
selected for
## PDSCH
scheduling in a
cell
1526727444 to
## 1526727475
L.ChMeas.PDSCH.MCS.0 to
L.ChMeas.PDSCH.MCS.31
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.52

## Measurement
## Item
Counter IDCounter Name
Number of
times the
reported
wideband CQI is
n (n = 0 to 15)
in a cell
1526727396 to
## 1526727411
L.ChMeas.CQI.DL.0 to
L.ChMeas.CQI.DL.15
1526737710L.ChMeas.CQI.DL.BorderUE.Total
1526737711L.ChMeas.CQI.DL.BorderUE.Num
## Counters
related to the
number of
times ranks 1 to
4 are reported
by UEs in a cell
1526730141L.ChMeas.RI.Rank1
1526730142L.ChMeas.RI.Rank2
1526732737L.ChMeas.RI.Rank3
1526732738L.ChMeas.RI.Rank4
## Average
downlink user
data rate in a
cell
1526728261L.Thrp.bits.DL
1526728997L.Thrp.Time.Cell.DL.HighPrecision
1526728262L.Thrp.Time.DL
1526729005L.Thrp.bits.DL.LastTTI
1526729015L.Thrp.Time.DL.RmvLastTTI
Downlink data
rates of cell
edge UEs in a
cell
1526737755L.Thrp.bits.DL.BorderUE
1526741760L.Thrp.Time.DL.BorderUE
1526737758L.Thrp.bits.DL.LastTTI.BorderUE
1526737759L.Thrp.Time.DL.RmvLastTTI.BorderUE

5.4 Operation and Maintenance
## 5.4.1 Data Configuration
## 5.4.1.1 Data Preparation
Parameters Used for Activation and Parameters Used for Optimization
describe the parameters used for function activation and optimization,
respectively.
Parameters Used for Activation
DL CoMP based on USU3910-based multi-BBU interconnection requires that eX2
links be configured. For details about the parameters required for eX2 link setup,
see
eX2 Self-Management.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.53

The following table describes the parameter that must be set in the
CellAlgoSwitch MO to configure the TM9 JT switch.
Table 5-1 Parameter in the CellAlgoSwitch MO
## Parameter
## Name
Parameter IDOptionSetting Notes
## Downlink
CoMP
algorithms
switch
CellAlgoSwit
ch.DlCompS
witch
Tm9JtSwitchSelect this option.

The following table describes the parameters that must be set in the
CellDlCompAlgo MO to configure the thresholds for DL CoMP.
Table 5-2 Parameters that must be set in the CellDlCompAlgo MO
## Parameter
## Name
Parameter IDSetting Notes
## JT
## Coordinating
Cell RSRP
## Threshold
CellDlCompA
lgo.JtCoCellR
srpThd
Set this parameter to its recommended value.
## JT
## Coordinating
Cell DL PRB
## Threshold
CellDlCompA
lgo.JtCoCellD
lPrbThd
A smaller value of this parameter indicates a
lower threshold for a cell to be selected as a
coordinating cell for JT. In this case, JT gains
cannot be maximized. A larger value of this
parameter indicates a higher threshold for a
cell to be selected as a coordinating cell for JT,
increasing the probability of negative JT gains.
Set this parameter to its recommended value.
JT Serving
Cell DL PRB
## Threshold
CellDlCompA
lgo.JtServing
CellDlPrbThd
Set this parameter to its recommended value.

The following table describes the parameters that must be set in the
NCellDlRsrpMeasPara MO for coordinating cell set measurement.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.54

Table 5-3 Parameters in the NCellDlRsrpMeasPara MO
## Parameter
## Name
Parameter IDSetting Notes
## DL RSRP
NCell
## Measurement
## A3 Offset
NCellDlRsrp
MeasPara.NC
ellDlRsrpMea
sA3Offset
Set this parameter to its recommended value.
## DL RSRP
NCell
## Measurement
## A6 Offset
NCellDlRsrp
MeasPara.Dl
RsrpNCellMe
asA6Offset
This parameter is required only in intra-BBU CA
scenarios.
Set this parameter to its recommended value.

The following table describes the parameters that must be set in the
CellCsiRsParaCfg MO for the CSI-RS.
Table 5-4 Parameters in the CellCsiRsParaCfg MO
## Parameter
## Name
Parameter IDSetting Notes
CSI-RS SwitchCellCsiRsPara
Cfg.CsiRsSwit
ch
After DL CoMP is enabled, set this parameter
to ADAPTIVE_CFG.
When the preceding parameter settings are
used, the cell performs the following
operations:
● If there are UEs that can be selected as JT
UEs in the cell where TM9 JT takes effect,
and the proportion of TM9 UEs and the
threshold for the number of TM9 UEs are
satisfied, the cell sends TM9 JT-specific CSI-
RS configurations.
● If no UE can be selected as a TM9 JT UE, or
the proportion of TM9 UEs and the
threshold for the number of TM9 UEs are
not satisfied, the cell does not send TM9 JT-
specific CSI-RS configurations.
CSI-RS PeriodCellCsiRsPara
Cfg.CsiRsPeri
od
Set this parameter to its recommended value.
CSI-RS Config
## User Ratio
## Threshold
CellCsiRsPara
Cfg.CsiRsConf
igUserRatioT
h
Set this parameter to its recommended value.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.55

## Parameter
## Name
Parameter IDSetting Notes
CSI-RS Config
## User Number
## Threshold
CellCsiRsPara
Cfg.CsiRsConf
igUserNumT
h
Set this parameter to its recommended value.
## CSI-RS
## Unconfig User
## Ratio
## Threshold
CellCsiRsPara
Cfg.CsiRsUnc
onfigUserRat
ioTh
Set this parameter to its recommended value.
## CSI-RS
## Unconfig User
## Number
## Threshold
CellCsiRsPara
Cfg.CsiRsUnc
onfigUserNu
mTh
Set this parameter to its recommended value.
CSI-RS Set
## Judge
## Hysteresis
## Timer
CellCsiRsPara
Cfg.CsiRsSetJ
udgeHysTim
er
Set this parameter to its recommended value.
CSI-RS Set
## Judge Timer
CellCsiRsPara
Cfg.CsiRsSetJ
udgeTimer
Set this parameter to its recommended value.

The following table describes the parameters that must be set in the
CellDlschAlgo MO for downlink scheduling.
Table 5-5 Parameters that must be set in the CellDlschAlgo MO
## Parameter
## Name
Parameter IDOptionSetting Notes
## CSI-RS
## Subframe
## Scheduling
## Strategy
## Switch
CellDlschAlg
o.CsiRsSfSchS
trSwitch
UnconfigCsiRs
UeEnDeOrder
SchSw
You are advised to select this
option.
When this option is selected,
the UnCfgCsiRsUEDeOr-
derSchSwitch option of the
CellDlschAlgo.
CsiRsSfSchStrS
witch parameter must be
deselected.
## Downlink
## User Data
## Threshold
CellDlschAlg
o.DlUserData
## Thld
NoneSet this parameter to its
recommended value.
## FD UE
## Enhanced
Aperiodic CQI
## Trigger Period
CellDlschAlg
o.FDUEEnhAp
erCQITrigPeri
od
NoneValue 20ms is recommended.

eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.56

The following table describes the parameter that must be set in the CellUlschAlgo
MO for uplink scheduling.
Table 5-6 Parameter that must be set in the CellUlschAlgo MO
## Parameter
## Name
Parameter IDSetting Notes
## Doppler
## Measurement
## Level
CellUlschAlg
o.DopMeasLe
vel
It is recommended that this parameter be set
to CLASS_1 to obtain more measurement
information.

Parameters Used for Optimization
Table 5-7 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
## MBSFN
## Subframe
## Configuration
CellDlschAlg
o.MbsfnSfCfg
In scenarios where the TM9-capable UE
penetration rate approaches 100% or in
demonstration scenarios, it is recommended
that this parameter be set to the maximum
number of MBSFN subframes (including
subframes 1, 2, 3, 6, 7, and 8) for cells where
DL CoMP with TM9 is enabled to offset TM9
demodulation reference signal (DMRS)
overheads and reduce cell-specific reference
signal (CRS) interference.
DL CoMP with TM9 requires that the MBSFN
subframe configurations for all cells be
consistent.
## No
## Scheduling
## Stop
## Triggering
ACqi Thd
CellDlschAlg
o.NoSchStop
ACqiThd
Set this parameter to its recommended value.
DL CoMP
## Report
## Interval
CellDlCompA
lgo.DlCompR
eportInterval
Set this parameter to its recommended value.
When UL CoMP takes effect, the reporting
interval of DL CoMP measurement reports is
subject to the reporting interval of UL CoMP
measurement reports.
DL CoMP
## Scheduling
## Priority Factor
CellDlCompA
lgo.DlCompS
chPriFactor
Set this parameter to its recommended value.

eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.57

5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
## NO TICE
● All cells with this feature enabled must have the same TM9 JT configurations.
● This feature is implemented on the basis of TM9. CSI-RSs must be configured
(using the CellCsiRsParaCfg MO) in all the cells with this feature enabled.
When USU3910-based multi-BBU interconnection is adopted, configure eX2
interfaces. For details, see eX2 Self-Management.
//Configuring parameter related to event A3 or A6 measurement
MOD NCELLDLRSRPMEASPARA: LocalCellId=0, DlRsrpAutoNCellMeasSwitch=ON,
NCellDlRsrpMeasA3Offset=-12, DlRsrpNCellMeasA6Offset=-12;
//Enabling the TM9 JT algorithm
MOD CELLALGOSWITCH: LocalCellId=0, DlCompSwitch=Tm9JtSwitch-1;
//Modifying cell-level TM9 JT parameters
MOD CELLDLCOMPALGO: LocalCellId=0, JtCoCellRsrpThd=-6, JtServingCellDlPrbThd=100,
JtCoCellDlPrbThd=20, DlCompSchPriFactor=1;
//Setting CSI-RS-related parameters
MOD CELLCSIRSPARACFG: LocalCellId=0, CsiRsSwitch=ADAPTIVE_CFG, CsiRsPeriod=ms40,
CsiRsConfigUserNumTh=1, CsiRsUnconfigUserNumTh=200, CsiRsConfigUserRatioTh=1,
CsiRsUnconfigUserRatioTh=0, CsiRsSetJudgeHysTimer=1, CsiRsSetJudgeTimer=1;
//Setting a period for triggering aperiodic CSI reporting for TM9 JT
MOD CELLDLSCHALGO: LocalCellId=0, FDUEEnhAperCQITrigPeriod=20ms, NoSchStopACqiThd=40;
//Setting the packet size threshold for TM9 JT
MOD CELLDLSCHALGO: LocalCellId=0, DlUserDataThld=500;
//Setting downlink scheduling-related parameters
MOD CELLDLSCHALGO: LocalCellId=0,
CsiRsSfSchStrSwitch=UnCfgCsiRsUEDeOrderSchSwitch-0&UnconfigCsiRsUeEnDeOrderSchSw-1;
//Setting uplink scheduling-related parameters
MOD CELLULSCHALGO: LocalCellId=0, DopMeasLevel=CLASS_1;
//Setting the reporting interval of event A3 or A6 for DL CoMP
MOD CELLDLCOMPALGO: LocalCellId=0, DlCompReportInterval=1024MS;
## Deactivation Command Examples
//(Optional) Turning off the CSI-RS configuration switch when deactivating DL CoMP with TM9 if only this
feature is enabled on the network (other features based on TM9 and TM10 transmission modes are
disabled)
MOD CELLCSIRSPARACFG: LocalCellId=0, CsiRsSwitch=NOT_CFG;
//Turning off the TM9 JT switch
MOD CELLALGOSWITCH: LocalCellId=0, DlCompSwitch=Tm9JtSwitch-0;
5.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
Perform the following steps:
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.58

Step 1On the eNodeB side, run the DSP CELLDLCOMPCOCELLS command to query the
value of Cell DL CoMP Property.
Expected result: The value of Cell DL CoMP Property is
CELL_STATUS_TYPE_TM9_JT_IN or CELL_STATUS_TYPE_TM9TM10_JT_IN, and
there are coordinating cells.
Step 2Log in to the MAE-Access and choose Monitoring > Signaling Trace > Signaling
Trace Management. In the displayed window, choose Cell Performance
Monitoring > DL CoMP Monitoring in the navigation tree. In the displayed dialog
box, select the target eNodeB and create a DL CoMP monitoring task that
monitors the number of UEs that benefit from JT. Observe the number of times JT
UEs in the local cell are scheduled in coordinating cells.
Expected result: The value of JT Benefit User Number is not 0. This result shows
that this feature has taken effect.
----End
## 5.4.3 Network Monitoring
The gains offered by this feature can be observed using the following methods.
## Using Counters
Observe the counters listed in the following table before and after activating this
feature. The changes in the counter values reflect feature performance.
Counter ID
## Counter Name
1526743728L.Traffic.User.DLJT.Avg
1526749462L.Traffic.User.SCell.Active.DLJT.Avg
1526743726L.ChMeas.PRB.DL.JT.Used.Avg.OtherC
ell
1526727444 to 1526727475L.ChMeas.PDSCH.MCS.0 to
L.ChMeas.PDSCH.MCS.31

Observe the following indicators before and after activating this feature. The
changes in the values reflect feature gains.
## NO TICE
Before observing the downlink average user-perceived rate and the user-perceived
rate at the cell edge, run the MOD CELLCOUNTERPARAGROUP command with
the BasedA3EdgeUserSwitch option selected under the Cell Counter Algorithm
Switch parameter.
MML command example:
MOD CELLCOUNTERPARAGROUP: LocalCellId=0, CellCounterAlgoSwitch=BasedA3EdgeUserSwitch-1,
EdgeUserA3Offset=-12;
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.59

IndicatorFormulaExpected Result
Downlink average
perceived rate
(L.Thrp.bits.DL –
L.Thrp.bits.DL.LastTTI)/
L.Thrp.Time.DL.RmvLast
## TTI
The average downlink
user-perceived data rate
increases or remains
unchanged after feature
activation.
Average downlink CEU
throughput
(L.Thrp.bits.DL.BorderU
## E –
L.Thrp.bits.DL.LastTTI.B
orderUE)/
L.Thrp.Time.DL.RmvLast
TTI.BorderUE
The average downlink
CEU throughput
increases after feature
activation.

## Using Signaling Tracing
●  Cell-level performance monitoring
a.  On the MAE-Access, choose Monitor > Signaling Trace > Signaling
## Trace Management.
b.  In the displayed window, choose Cell Performance Monitoring > DL
CoMP (Cell) Monitoring in the navigation tree and select the target
eNodeB to create a monitoring task.
c.  Observe the number of beneficiary UEs and the number of RBs used in
the serving cell and coordinating cell.
●  UE-level performance monitoring
a.  On the MAE-Access, choose Monitor > Signaling Trace > Signaling
## Trace Management.
b.  In the displayed window, choose User Performance Monitoring > DL
CoMP (User) Monitoring in the navigation tree and select a target user
to create a monitoring task.
c.  Observe the following items in the tracing result:
## ▪
Coordinating Cell's Local Cell ID
## ▪
UE Code Count of Coordinating Cell
▪CoCell DLSCH Code0 Num/CoCell DLSCH Code1 Num
▪CoCell DLSCH Code0 RBs/CoCell DLSCH Code1 RBs
## 5.4.4 Possible Issues
If the number of UEs that benefit from JT is zero, or the CEU throughput of the
entire network does not increase after this feature is activated, perform the
following steps:
Step 1Run the LST CELLALGOSWITCH command to check whether the TM9 JT
algorithm switch is turned on.
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.60

●  If yes, go to Step 2.
●  If no, configure parameters by referring to 5.4.1.1 Data Preparation.
Step 2Run the DSP CELLDLCOMPCOCELLS command to check whether TM9 JT has
been activated for the cell.
●  If yes, check whether there is a coordinating cell list.
–   If yes, go to Step 3.
–   If no, check whether intra-frequency neighbor relationships have been
established between the local cell and neighboring cells. Check whether
there are CEUs in the cell by observing the L.Traffic.User.BorderUE.Avg
counter. Check whether the DL CoMP switch has been turned on for more
than one hour.
●  If no, check whether the local cell meets the thresholds for entering TM9 JT,
including:
–CellCsiRsParaCfg.
CsiRsConfigUserRatioTh
–CellCsiRsParaCfg.CsiRsUnconfigUserRatioTh
–CellDlCompAlgo.JtCoCellDlPrbThd and
CellDlCompAlgo.
JtServingCellDlPrbThd
Step 3Check the following performance counters to see whether the JT UE proportion is
too low, for example, lower than 15%.
Counter ID
Counter NameDescription
1526743728L.Traffic.User.DLJT.
## Avg
Average number of downlink JT UEs in
a cell

●  If no, go to Step 4.
●  If yes, the number of JT UEs is too small. In this case, DL CoMP cannot offer
noticeable gains to increase the capacity in terms of UE quantity and data
rate.
Step 4If the preceding steps fail to resolve the problem, contact Huawei technical
support.
----End
eRAN
DL CoMP (FDD) Feature Parameter Description5 DL CoMP with TM9
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.61

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
DL CoMP (FDD) Feature Parameter Description6 Parameters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.62

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
DL CoMP (FDD) Feature Parameter Description7 Counters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.63

## 8 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
DL CoMP (FDD) Feature Parameter Description8 Glossary
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.64

## 9 Reference Documents
-  3GPP TS 36.213, "Channel quality indicator (CQI) definition"
-  3GPP TS 36.331, "UE-EUTRA-Capability"
## 3.
Cloud BB Overview
## 4.CSPC
5.DRX and Signaling Control
6.eMIMO (FDD)
7.eMTC
8.eX2 Self-Management
9.LTE FDD and NR Spectrum Sharing
10.Dynamic Power Sharing Between LTE Carriers
11.Massive MIMO (FDD)
## 12.MRO
## 13.SFN
14.Smart 8T8R (FDD)
15.VoLTE
16.WTTx MU-MIMO (FDD)
17.Extended Cell Range
18.Scheduling
19.Modulation Schemes
20.Low-Band Booster
21.High Speed Mobility
22.Energy Conservation and Emission Reduction
23.USU3910-based Multi-BBU Interconnection
24.Emergency Call
25.Extended CP
26.3D Beamforming (FDD)
27.Synchronization
28.TDM eICIC (FDD)
eRAN
DL CoMP (FDD) Feature Parameter Description9 Reference Documents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.65

29.Channel State Management
30.Virtual 4T4R (FDD)
31.Physical Channel Resource Management
32.Adaptive ICIC
33.Carrier Aggregation
34.RuralLink Solution
eRAN
DL CoMP (FDD) Feature Parameter Description9 Reference Documents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.66