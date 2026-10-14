

eRAN
SRVCC Feature Parameter
## Description
## Issue04
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
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 04 (2024-06-21)..................................................................................................................................................1
1.2 eRAN18.1 03 (2023-09-14)..................................................................................................................................................1
1.3 eRAN18.1 02 (2023-02-01)..................................................................................................................................................2
1.4 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.5 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 2
2 About This Document.............................................................................................................4
2.1 General Statements................................................................................................................................................................ 4
2.2 Applicable RAT......................................................................................................................................................................... 4
2.3 Features in This Document.................................................................................................................................................. 5
3 Overview....................................................................................................................................6
4 SRVCC to UTRAN..................................................................................................................... 7
4.1 Principles.................................................................................................................................................................................... 7
4.1.1 Triggering................................................................................................................................................................................8
4.1.2 Measurement and Target Cell Selection................................................................................................................... 10
4.1.3 Handover Policy Selection for SRVCC.........................................................................................................................10
4.1.4 Retry and Penalty.............................................................................................................................................................. 14
4.2 Network Analysis.................................................................................................................................................................. 14
4.2.1 Benefits................................................................................................................................................................................. 15
4.2.2 Impacts..................................................................................................................................................................................15
4.3 Requirements......................................................................................................................................................................... 15
4.3.1 Licenses................................................................................................................................................................................. 15
4.3.2 Software................................................................................................................................................................................15
4.3.3 Hardware..............................................................................................................................................................................16
4.3.4 Others....................................................................................................................................................................................16
4.4 Operation and Maintenance.............................................................................................................................................17
4.4.1 Data Configuration (FDD)..............................................................................................................................................17
4.4.1.1 Data Preparation............................................................................................................................................................ 17
4.4.1.2 Using MML Commands............................................................................................................................................... 28
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 31
4.4.2 Activation Verification......................................................................................................................................................31
4.4.3 Network Monitoring.........................................................................................................................................................33
eRAN
SRVCC Feature Parameter DescriptionContents
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iii

5 SRVCC to GERAN................................................................................................................... 36
5.1 Principles.................................................................................................................................................................................. 36
5.1.1 Triggering............................................................................................................................................................................. 37
5.1.2 Measurement and Target Cell Selection................................................................................................................... 38
5.1.3 Handover Policy Selection for SRVCC.........................................................................................................................39
5.1.4 Retry and Penalty.............................................................................................................................................................. 42
5.2 Network Analysis.................................................................................................................................................................. 42
5.2.1 Benefits................................................................................................................................................................................. 42
5.2.2 Impacts..................................................................................................................................................................................42
5.3 Requirements......................................................................................................................................................................... 43
5.3.1 Licenses................................................................................................................................................................................. 43
5.3.2 Software................................................................................................................................................................................43
5.3.3 Hardware..............................................................................................................................................................................43
5.3.4 Others....................................................................................................................................................................................44
5.4 Operation and Maintenance.............................................................................................................................................44
5.4.1 Data Configuration........................................................................................................................................................... 44
5.4.1.1 Data Preparation............................................................................................................................................................ 44
5.4.1.2 Using MML Commands............................................................................................................................................... 53
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 55
5.4.2 Activation Verification......................................................................................................................................................55
5.4.3 Network Monitoring.........................................................................................................................................................56
6 SRVCC Flexible Steering to UTRAN...................................................................................59
6.1 Principles.................................................................................................................................................................................. 59
6.2 Network Analysis.................................................................................................................................................................. 60
6.2.1 Benefits................................................................................................................................................................................. 60
6.2.2 Impacts..................................................................................................................................................................................60
6.3 Requirements......................................................................................................................................................................... 61
6.3.1 Licenses................................................................................................................................................................................. 61
6.3.2 Software................................................................................................................................................................................61
6.3.3 Hardware..............................................................................................................................................................................61
6.3.4 Others....................................................................................................................................................................................62
6.4 Operation and Maintenance.............................................................................................................................................62
6.4.1 Data Configuration........................................................................................................................................................... 62
6.4.1.1 Data Preparation............................................................................................................................................................ 62
6.4.1.2 Using MML Commands............................................................................................................................................... 63
6.4.1.3 Using the MAE-Deployment...................................................................................................................................... 63
6.4.2 Activation Verification......................................................................................................................................................63
6.4.3 Network Monitoring.........................................................................................................................................................64
7 Parameters..............................................................................................................................65
8 Counters.................................................................................................................................. 66
9 Glossary................................................................................................................................... 67
eRAN
SRVCC Feature Parameter DescriptionContents
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iv

10 Reference Documents........................................................................................................ 68
11 Appendix............................................................................................................................... 69
11.1 Signaling Procedures......................................................................................................................................................... 69
eRAN
SRVCC Feature Parameter DescriptionContents
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.v

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 04 (2024-06-21)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions of the principles of voice-quality-based SRVCC. For details, see
4.1.1 Triggering, 4.1.2 Measurement and Target Cell Selection, and 5.1.1
## Triggering.
1.2 eRAN18.1 03 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document, which do not involve changes in meanings
and therefore are not detailed.
eRAN
SRVCC Feature Parameter Description1 Change History
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.1

1.3 eRAN18.1 02 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.5 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 03 (2021-06-26).
## Technical Changes
## Change Description
## Paramete
r Change
RATBase Station Model
Added support for the
optimized mechanism of
determining whether to
perform voice-quality-based
SRVCC by micro base stations.
For details, see the following
sections:
## ●4.1.3 Handover Policy
Selection for SRVCC
## ●5.1.3 Handover Policy
Selection for SRVCC
NoneFDD● BTS3203E
## ● BTS3202E
Added support for the
decoupling of voice-quality-
based SRVCC from coverage-
based SRVCC by micro base
stations. For details, see the
following sections:
## ●4.1 Principles
## ●5.1 Principles
NoneFDD● BTS3203E
## ● BTS3202E
eRAN
SRVCC Feature Parameter Description1 Change History
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.2

Change DescriptionParamete
r Change
RATBase Station Model
Replaced the
ErabFlowFirstSwitch option
of the
GlobalProcSwitch.HoProcCtrl
Switch parameter with the
ERAB_FLOW_FIRST value of
the
GlobalProcSwitch.
HoErabConf
lProcessingStrat
parameter.
For details, see the following
sections:
●4.1.2 Measurement and
## Target Cell Selection
## ●4.4.1.1 Data Preparation
●4.4.1.2 Using MML
## Commands
●5.1.2 Measurement and
## Target Cell Selection
## ●5.4.1.1 Data Preparation
●5.4.1.2 Using MML
## Commands
## Modified
paramete
r: Deleted
the
ErabFlow
FirstSwit
ch option
of the
GlobalPr
ocSwitch.
HoProcCt
rlSwitch
paramete
r.
## FDD● BTS3912E
## ● BTS3203E
## ● BTS3202E

## Editorial Changes
Revised descriptions in this document.
eRAN
SRVCC Feature Parameter Description1 Change History
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.3

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
SRVCC Feature Parameter Description2 About This Document
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.4

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LOFD-001022SRVCC to UTRAN4 SRVCC to UTRAN
LOFD-001023SRVCC to GERAN5 SRVCC to GERAN
LOFD-001087SRVCC Flexible
Steering to UTRAN
6 SRVCC Flexible Steering to UTRAN
eRAN
SRVCC Feature Parameter Description2 About This Document
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.5

## 3 Overview
In the early phase of evolved universal terrestrial radio access network (E-UTRAN)
deployment, when UEs running voice over Long Term Evolution (VoLTE) services
move out of an E-UTRAN network, single radio voice call continuity (SRVCC) can
be used to hand over the VoLTE services to the circuit switched (CS) domain of the
universal terrestrial radio access network (UTRAN) or GSM/EDGE radio access
network (GERAN) to ensure voice call continuity.
SRVCC is a type of inter-RAT handover. For details, see 4.1.2 "Architectural
Principles for 3GPP UTRAN/GERAN SRVCC and vSRVCC" in 3GPP TS 23.216
## V11.1.0.
## NO TE
This document focuses on eNodeB functions. The eNodeB has the same function
requirements for SRVCC and enhanced single radio voice call continuity (eSRVCC).
Therefore, this document does not distinguish between SRVCC and eSRVCC.
eRAN
SRVCC Feature Parameter Description3 Overview
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.6

4 SRVCC to UTRAN
## 4.1 Principles
In this document, the SRVCC to UTRAN function refers to coverage-based SRVCC
to UTRAN. This function is controlled by the UtranSrvccSwitch option of the
CellHoParaCfg.
HoModeSwitch parameter.
Coverage-based SRVCC to UTRAN is a type of inter-RAT handover. For details on
its triggering mechanism, see the descriptions of coverage-based inter-RAT
handover to UTRAN in
Mobility Management in Connected Mode. This function
serves as a basis for SRVCC triggered by other causes. For details about SRVCC
triggered by other causes, see 4.1.1 Triggering.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.7

Figure 4-1 SRVCC procedure
## 4.1.1 Triggering
SRVCC can be triggered for different causes. SRVCC triggered for different causes
is controlled by separate parameters.
Voice-Quality-based SRVCC
This function is controlled by the UtranVolteQualityHoSwitch option of the
CellHoParaCfg.
VoLTEQualityHoAlgoSwitch parameter.
After this function is enabled, if the uplink packet loss rate of the bearer with QCI
1 or downlink packet loss rate of the bearer with QCI 1 of a VoLTE UE exceeds the
threshold specified by the CellHoParaCfg.
Qci1PlrThldForVolteQualHo parameter
within a voice quality decision period specified by the
CellHoParaCfg.
VolteQualPktLossPeriod parameter, the eNodeB determines that
the voice quality of the UE is poor and starts event B1 measurement for a
handover to the UTRAN. The threshold for event B1 related to voice-quality-based
SRVCC is the same as that for coverage-based SRVCC.
## NO TE
●  In high-speed railway scenarios, the high voice packet loss rate persists due to high
speed mobility even after UEs are handed over to a UTRAN. Voice quality cannot be
improved. Therefore, it is not recommended that voice-quality-based SRVCC be used in
high-speed railway scenarios.
●  To reduce the gap-assisted measurement's impact on voice quality and incurred air
interface signaling overheads, the eNodeB triggers voice-quality-based inter-RAT
handover measurement only once for a UE in a cell during a voice call.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.8

LCS-based SRVCC
This function is controlled by the LcsSrvccSwitch option of the
ENodeBAlgoSwitch.HoModeSwitch parameter. This function also depends on the
UTRAN location service (LCS) capability, which is controlled by the
CSFallBackBlindHoCfg.UtranLcsCap parameter.
LCS-based SRVCC is used when a UE triggers LCS in an E-UTRAN network that
supports VoLTE services but does not support LCS. When the UE initiates LCS, the
mobility management entity (MME) delivers a CS Fallback Indicator to the
eNodeB. The eNodeB performs SRVCC to hand over the UE to the CS domain for
LCS while maintaining voice service continuity.
LCS-based SRVCC has the same target cell signal requirements as CSFB to UTRAN.
For details on the requirements, see
CS Fallback.
SRVCC Triggered by Other Causes
SRVCC TypeSwitch for SRVCC to
## UTRAN
## Reference Document
## Service-based
## SRVCC
UtranServiceHoSwitch
option of the
ENodeBAlgoSwitch.HoAl
goSwitch parameter
Service-, distance-, and uplink-
quality-based SRVCC
handovers are inter-RAT
handovers. For details on the
triggering mechanisms of
these handovers, see
corresponding sections in
Mobility Management in
## Connected Mode
## .
## Distance-based
## SRVCC
UTRAN option of the
DistBasedHO.DistBasedM
easObjType parameter,
and the
CellAlgoSwitch.DistBased
HoSwitch
parameter
## Uplink-quality-
based SRVCC
UlQualityInterRATHoS-
witch option of the
ENodeBAlgoSwitch.HoAl
goSwitch parameter
## Load-based
## SRVCC
UtranMlbSwitch option
of the
CellAlgoSwitch.MlbAlgoS
witch parameter
Load-based SRVCC handover
is a load transfer method. For
details on its triggering
mechanisms, see Inter-RAT
## Mobility Load Balancing
## .
SPID-based
SRVCC (SPID is
short for
subscriber profile
## ID)
InterPlmnHoSwitch
option of the
ENodeBAlgoSwitch.HoAl
goSwitch parameter, and
the
SpidCfg.
HoBackToHPLM
NSwitch parameter
For details, see descriptions of
the SPID-specific handover
back to HPLMN policy in
## Flexible User Steering.

eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.9

4.1.2 Measurement and Target Cell Selection
Coverage-, service-, distance-, and uplink-quality-based SRVCC handovers are
inter-RAT handovers. For details on measurement and target cell selection for
these handovers, see the descriptions of the basic functions of mobility
management in connected mode and the descriptions of coverage-, service-,
distance-, and uplink-quality-based inter-RAT handovers in
## Mobility Management
in Connected Mode.
For details on measurement and target cell selection for load-based SRVCC, see
Inter-RAT Mobility Load Balancing.
If SRVCC is triggered by the SPID-based inter-RAT handover function, SPID-based
filtering is used during measurement and target cell selection. For details, see
## Flexible User Steering.
The measurement, target cell selection, and execution procedures for voice-
quality-based SRVCC are the same as those for coverage-, service-, distance-, and
uplink-quality-based SRVCC. If both the uplink packet loss rate of the bearer with
QCI 1 and downlink packet loss rate of the bearer with QCI 1 of a VoLTE UE are
less than or equal to the threshold specified by the
CellHoParaCfg.
VolteQualRecoveryQci1PlrThld parameter within a voice quality
decision period, the eNodeB considers that the voice quality of the UE has
recovered and instructs the UE to stop inter-RAT measurements for voice-quality-
based SRVCC.
If SRVCC to UTRAN and SRVCC to GERAN are supported on the network, the
eNodeB delivers measurement configurations, instructing the UEs to measure
neighboring UTRAN and GERAN cells. Cells in the first valid measurement report
are selected as target cells for SRVCC. It is recommended that the
GlobalProcSwitch.
HoErabConflProcessingStrat parameter be set to
ERAB_FLOW_FIRST to increase the SRVCC handover success rate. Under this
setting, the eNodeB preferentially handles the QCI-1 bearer deletion procedure
when the SRVCC and QCI-1 bearer deletion procedure conflict.
4.1.3 Handover Policy Selection for SRVCC
Figure 4-2 shows the procedure for selecting a handover policy for SRVCC to
UTRAN when QCI-1 bearers exist. The following handover policies are selected in
sequence:
-  VoLTE packet switched (PS) handover
## 2.  CS+PS SRVCC
-  CS-only SRVCC
If the requirements of the preceding three handover policies are not met, a
handover will not be performed.
## NO TE
Redirection cannot be used as a handover policy for QCI-1 VoLTE services. Otherwise, call
drops occur. Redirection is controlled by the REDIRECTION option of the
InterRatPolicyCfgGroup.
UtranHoCfg parameter.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.10

Figure 4-2 Procedure for selecting a handover policy for SRVCC from E-UTRAN to
## UTRAN
VoLTE PS Handover
If the UTRAN supports VoIP, the VoLTE PS handover policy can be used to hand
over VoLTE services from the E-UTRAN to the UTRAN. VoLTE PS handover from E-
UTRAN to UTRAN is controlled by the UtranVoipCapSwitch option of the
ENodeBAlgoSwitch.
HoModeSwitch parameter and the UtranPsHoSwitch option
of the CellHoParaCfg.
HoModeSwitch parameter.
For FDD, if some operators or RNCs on the network do not support VoLTE PS
handover, operators' or RNCs' capability to support VoLTE PS handover can be set
as follows:
●  Enable the Separate Mobility Policies to UTRAN for Multi PLMN function,
which is controlled by the UtranSepOpMobilitySwitch option of the
ENodeBAlgoSwitch.
MultiOpCtrlSwitch parameter.
●Configure the VoIP capability of specific operators or RNCs, which is specified
by the following parameters (VoIP is supported by an operator or RNC by
default if the VoIP capability is not configured):
–UtranNetworkCapCfg.
## Mcc
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.11

–UtranNetworkCapCfg.Mnc
–UtranNetworkCapCfg.RncId
–VoipCapCfg option of the UtranNetworkCapCfg.NetworkCapCfg
parameter
●Configure the PS handover capability of specific operators or RNCs, which is
specified by the following parameters:
–UtranNetworkCapCfg.Mcc
–UtranNetworkCapCfg.Mnc
–UtranNetworkCapCfg.RncId
–PsHoCapCfg option of the UtranNetworkCapCfg.NetworkCapCfg
parameter
## NO TE
When the UeVoipOnHspaCapSwitch option of the ENodeBAlgoSwitch.HoModeSwitch
parameter is selected, the number of SRVCC execution times increases and the number of
PS handover execution times decreases.
## CS+PS SRVCC
CS+PS SRVCC can be triggered if the following requirements are met:
●  SRVCC to UTRAN and PS handover from E-UTRAN to UTRAN are enabled. PS
handover from E-UTRAN to UTRAN is controlled by the UtranPsHoSwitch
option of the cell-level parameter CellHoParaCfg.HoModeSwitch.
For FDD, if some operators or RNCs on the network do not support SRVCC or
PS handover, operators' or RNCs' capability to support SRVCC or PS handover
can be set as follows:
–   Enable the Separate Mobility Policies to UTRAN for Multi PLMN function,
which is controlled by the UtranSepOpMobilitySwitch option of the
ENodeBAlgoSwitch.
MultiOpCtrlSwitch parameter.
–Configure the SRVCC capability of specific operators or RNCs, which is
specified by the UtranNetworkCapCfg.
Mcc, UtranNetworkCapCfg.Mnc,
and UtranNetworkCapCfg.RncId parameters, and the SrvccCapCfg
option of the UtranNetworkCapCfg.
NetworkCapCfg parameter. SRVCC
is supported by an operator or RNC by default if the SRVCC capability is
not configured.
–Configure the PS handover capability of specific operators or RNCs, which
is specified by the UtranNetworkCapCfg.
## Mcc,
UtranNetworkCapCfg.Mnc, and UtranNetworkCapCfg.RncId
parameters, and the PsHoCapCfg option of the
UtranNetworkCapCfg.
NetworkCapCfg parameter.
●  SRVCC and PS handover are specified as QCI-specific handover policies. SRVCC
and PS handover are controlled by the SRVCC and PS_HO options of the
InterRatPolicyCfgGroup.
UtranHoCfg parameter, respectively. These handover
policies can be associated with a specific QCI by setting the
QciPara.
InterRatPolicyCfgGroupId parameter.
If services with different QCIs exist, the handover policy for the highest-
priority QCI prevails. The handover policy priority for each QCI is specified by
the CellQciPara.
QciPriorityForHo parameter. It is recommended that the
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.12

handover policy priority be set to the highest priority (1) for QCI 1 and the
lowest priority (9) for QCI 5.
## NO TE
●  For necessary handovers, for example, voice-quality-based, coverage-based, and uplink-
quality-based handovers, SRVCC can be triggered when SRVCC is configured in the inter-
RAT handover policy group for the highest-priority QCI.
●  For unnecessary handovers, for example, load-based, service-based, and CSFB-based
handovers, SRVCC can be triggered when SRVCC is configured in the inter-RAT handover
policy groups for all QCIs. If the Handover Command message sent from the MME to
the eNodeB for an unnecessary handover contains the "E-RABs To Release List" IE, the
eNodeB will cancel the handover.
●  The UtranExternalCell.
CsPsHOInd parameter, which specifies whether an
external UTRAN cell supports CS+PS SRVCC, is set to BOOLEAN_TRUE.
Before triggering CS+PS SRVCC, a macro or LampSite eNodeB determines
whether to check the CS+PS handover capability of external UTRAN cells
based on the setting of the CnOperatorHoCfg.
SrvccWithPsBasedCellCapSw
parameter.
–   If this parameter is set to ON, the eNodeB does not check the
UtranExternalCell.CsPsHOInd parameter setting of external UTRAN
cells.
–   If this parameter is set to OFF, the eNodeB checks the
UtranExternalCell.
CsPsHOInd parameter setting of external UTRAN
cells.
Before triggering CS+PS SRVCC, a micro eNodeB always checks the
UtranExternalCell.CsPsHOInd parameter setting of external UTRAN cells,
because micro eNodeBs do not support the
CnOperatorHoCfg.
SrvccWithPsBasedCellCapSw parameter.
CS-only SRVCC
CS-only SRVCC can be triggered if the following requirements are met:
●  SRVCC to UTRAN is enabled.
For FDD, if some operators or RNCs on the network do not support SRVCC,
operators' or RNCs' capability to support SRVCC can be set as follows:
–   Enable the Separate Mobility Policies to UTRAN for Multi PLMN function,
which is controlled by the UtranSepOpMobilitySwitch option of the
ENodeBAlgoSwitch.
MultiOpCtrlSwitch parameter.
–Configure the SRVCC capability of specific operators or RNCs, which is
specified by the UtranNetworkCapCfg.
Mcc, UtranNetworkCapCfg.Mnc,
and UtranNetworkCapCfg.
RncId parameters, and the SrvccCapCfg
option of the UtranNetworkCapCfg.NetworkCapCfg parameter. SRVCC
is supported by an operator or RNC by default if the SRVCC capability is
not configured.
●  SRVCC is specified as a QCI-specific handover policy. The SRVCC policy is
controlled by the SRVCC option of the InterRatPolicyCfgGroup.
UtranHoCfg
parameter. The policy can be associated with a specific QCI by setting the
QciPara.InterRatPolicyCfgGroupId parameter.
If services with different QCIs exist, the handover policy for the highest-
priority QCI prevails. The handover policy priority for each QCI is specified by
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.13

the CellQciPara.QciPriorityForHo parameter. It is recommended that the
handover policy priority be set to the highest priority (1) for QCI 1 and the
lowest priority (9) for QCI 5.
## NO TE
●  For necessary handovers, for example, voice-quality-based, coverage-based, and uplink-
quality-based handovers, SRVCC can be triggered when SRVCC is configured in the inter-
RAT handover policy group for the highest-priority QCI.
●  For unnecessary handovers, for example, load-based, service-based, and CSFB-based
handovers, SRVCC can be triggered when SRVCC is configured in the inter-RAT handover
policy groups for all QCIs. If the Handover Command message sent from the MME to
the eNodeB for an unnecessary handover contains the "E-RABs To Release List" IE, the
eNodeB will cancel the handover.
4.1.4 Retry and Penalty
Table 4-1 describes retry and penalty mechanisms for SRVCC triggered by various
causes.
Table 4-1 Retry and penalty mechanisms for SRVCC triggered by various causes
Triggering CauseRetry and Penalty Mechanism
● Coverage-based SRVCC
● Service-based SRVCC
● Distance-based SRVCC
● Uplink-quality-based SRVCC
● SPID-based SRVCC
● Voice-quality-based SRVCC
● LCS-based SRVCC
See Mobility Management in
## Connected Mode.
Load-based SRVCCSee Inter-RAT Mobility Load Balancing.

If the handover preparation for CS+PS SRVCC fails, the UE may re-initiate a
handover attempt, depending on the SRVCCWITHPSCSRETRYSWITCH option
setting of the CellHoParaCfg.
SrvccHoOptSwitch parameter.
●  If this option is selected, the UE re-initiates a CS-only SRVCC attempt for a
handover to the same target cell. This function applies only to SRVCC to
## UTRAN.
●  If this option is deselected, the UE does not initiate a CS handover attempt for
a handover to the same target cell.
## 4.2 Network Analysis
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.14

## 4.2.1 Benefits
By handing VoLTE services over to the CS domain of a UTRAN, SRVCC to UTRAN
ensures call continuity for UEs when the UEs move out of an E-UTRAN to a
## UTRAN.
## 4.2.2 Impacts
## Network Impacts
If the target network of a CS-only SRVCC procedure is a UTRAN, only bearers with
QCI 1 are diverted to the CS domain of the target network. Bearers with other
QCIs are reestablished in the PS domain of the target network only after an RAU
procedure. The CS-only SRVCC procedure results in a service interruption period of
several seconds for PS services while the CS+PS SRVCC procedure results in a
service interruption period of only hundreds of milliseconds for PS services.
Activating voice-quality-based SRVCC also has the following impacts on network
performance:
●  UEs with poor voice quality are handed over to a UTRAN through SRVCC,
which improves their voice quality.
●  After UEs with poor voice quality are handed over to the UTRAN through
SRVCC, the percentage of VoLTE UEs in the LTE network decreases.
## Function Impacts
## None
## 4.3 Requirements
## 4.3.1 Licenses
The following are FDD license requirements.
## RAT
Feature IDFeature
## Name
ModelSales Unit
FDDLOFD-001022SRVCC to
## UTRAN
LT1SSRVCCU00per RRC
## Connected
## User

## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.15

## Prerequisite Functions
RATFunction NameFunction SwitchReferenceDescription
FDDCoverage-based
inter-RAT
handover to
## UTRAN
UtranRedirectSwi
tch or
UtranPsHoSwitch
option of the
CellHoParaCfg.H
oModeSwitch
parameter
## Mobility
## Management
in Connected
## Mode
## CS+PS SRVCC
depends on
this function.

## Mutually Exclusive Functions
## None
## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
No requirements
## Boards
No requirements
RF Modules
No requirements
## 4.3.4 Others
## UTRAN
For CS+PS SRVCC, if the UTRAN equipment is provided by Huawei, corresponding
licenses must be activated on the UTRAN. For details, see descriptions of SRVCC
from LTE to UMTS with PS Handover in Interoperability Between UMTS and LTE of
RAN Feature Documentation.
## Core Network
●  If the core network equipment is provided by Huawei, the core network
version for eRAN6.0 or later is required. If the core network version is not for
eRAN6.0 or later, exceptions such as message parsing failure may occur.
If the CS+PS SRVCC policy is used and the core network equipment is provided
by Huawei, the corresponding license on the core network side must be
activated. For details, see the related documents for the core network.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.16

●  If the core network equipment is provided by another vendor, check the
software version of the core network to make sure that the core network
supports SRVCC complying with 3GPP Release 8 or later.
4.4 Operation and Maintenance
4.4.1 Data Configuration (FDD)
## 4.4.1.1 Data Preparation
Before configuring SRVCC to UTRAN, collect the data related to neighbor
relationships with UTRAN cells. This section provides only the information about
managed objects (MOs) related to neighboring UTRAN cells. For more
information about how to collect data for the parameters in these MOs, see the
MML-based configurations for basic mobility management functions in
## Mobility
Management in Connected Mode. Collect data for the parameters in the following
MOs:
1.UtranNFreq: used to configure a neighboring UTRAN frequency.
2.UtranExternalCell: used to configure external UTRAN cells. If VoLTE PS
handover or CS+PS SRVCC is enabled, you need to set the
UtranExternalCell.
Rac parameter.
-  (Optional) UtranExternalCellPlmn: used to configure additional PLMN IDs
for an external UTRAN cell. This MO is required only if the NodeB that serves
the external UTRAN cell works in RAN sharing with common carriers mode
and two or more operators share this cell.
4.UtranNCell: used to configure the neighbor relationship with a UTRAN cell.
Parameters Used for Activation
●  Scenario 1: Coverage-based SRVCC to UTRAN
–   SRVCC to UTRAN using the VoLTE PS handover policy
Table 4-2 Parameters used for the activation of coverage-based VoLTE PS
handover for SRVCC to UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
UtranSrvccSwitch
option of this
parameter.
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
UtranPsHoSwitch
option of this
parameter.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.17

## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
ENodeBAlgoSwitch.HoModeS
witch
Select the
UtranVoipCapSwitch
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Select the PS_HO
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Deselect the SRVCC
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Deselect the
REDIRECTION option
of this parameter.
## No
handover
flag
InterRatPolicyCfgGroup.NoH
oFlag
It is recommended that
the default value be
used if there is no
special requirement for
forbidding certain
handovers.
InterRAT
policy
config
group ID
InterRatPolicyCfgGroup.Inter
RatPolicyCfgGroupId
Set this parameter to
the same value as the
QciPara.InterRatPolicy
CfgGroupId parameter.
QoS Class
## Identifier
QciPara.QciSet this parameter as
required. For example,
set this parameter to 1.
InterRAT
## Policy
## Config
Group ID
QciPara.InterRatPolicyCfg-
GroupId
Set this parameter to
the same value as the
InterRatPolicyCfgGrou
p.InterRatPolicyCfg-
GroupId
parameter.
QCI Priority
## For
## Handover
CellQciPara.QciPriorityForHoIt is recommended that
this parameter be set
to the highest priority
(1) for QCI 1.

–   CS-only SRVCC to UTRAN
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.18

Table 4-3 Parameters used for the activation of coverage-based CS-only
SRVCC to UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
UtranSrvccSwitch
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Deselect the PS_HO
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Select the SRVCC
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Deselect the
REDIRECTION option
of this parameter.
## No
handover
flag
InterRatPolicyCfgGroup.NoH
oFlag
It is recommended that
the default value be
used if there is no
special requirement for
forbidding certain
handovers.
InterRAT
policy
config
group ID
InterRatPolicyCfgGroup.Inter
RatPolicyCfgGroupId
Set this parameter to
the same value as the
QciPara.InterRatPolicy
CfgGroupId parameter.
QoS Class
## Identifier
QciPara.QciSet this parameter as
required. For example,
set this parameter to 1.
InterRAT
## Policy
## Config
Group ID
QciPara.InterRatPolicyCfg-
GroupId
Set this parameter to
the same value as the
InterRatPolicyCfgGrou
p.InterRatPolicyCfg-
GroupId
parameter.
QCI Priority
## For
## Handover
CellQciPara.QciPriorityForHoIt is recommended that
this parameter be set
to the highest priority
(1) for QCI 1.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.19


–   CS+PS SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only
SRVCC to UTRAN has been enabled.
Table 4-4 Parameters used for the activation of coverage-based CS+PS
SRVCC to UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
UtranSrvccSwitch
option of this
parameter.
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
UtranPsHoSwitch
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Select the PS_HO
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Select the SRVCC
option of this
parameter.
## UTRAN
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Utra
nHoCfg
Deselect the
REDIRECTION option
of this parameter.
## No
handover
flag
InterRatPolicyCfgGroup.NoH
oFlag
It is recommended that
the default value be
used if there is no
special requirement for
forbidding certain
handovers.
InterRAT
policy
config
group ID
InterRatPolicyCfgGroup.Inter
RatPolicyCfgGroupId
Set this parameter to
the same value as the
QciPara.InterRatPolicy
CfgGroupId parameter.
QoS Class
## Identifier
QciPara.QciSet this parameter as
required. For example,
set this parameter to 1.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.20

## Parameter
## Name
Parameter IDSetting Notes
InterRAT
## Policy
## Config
Group ID
QciPara.InterRatPolicyCfg-
GroupId
Set this parameter to
the same value as the
InterRatPolicyCfgGrou
p.InterRatPolicyCfg-
GroupId parameter.
QCI Priority
## For
## Handover
CellQciPara.QciPriorityForHoIt is recommended that
this parameter be set
to the highest priority
(1) for QCI 1.
CS and PS
handover
indicator
UtranExternalCell.CsPsHOIndSet this parameter to
## BOOLEAN_TRUE.

●  Scenario 2: LCS-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-5 Parameters used for the activation of LCS-based SRVCC to UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## UTRAN LCS
capability
CSFallBackBlind-
HoCfg.UtranLcsCap
Set this parameter to
## ON.
## Handover
Mode switch
ENodeBAlgoSwitch.HoModeSw
itch
Select the
LcsSrvccSwitch option
of this parameter.

●  Scenario 3: Voice-quality-based SRVCC to UTRAN
Table 4-6 Parameters used for the activation of voice-quality-based SRVCC to
## UTRAN
## Parameter
## Name
Parameter IDSetting Notes
VoLTE
## Quality
## Handover
## Algo Switch
CellHoParaCfg.VoLTEQualityHo
AlgoSwitch
Select the
UtranVolteQualityHoS-
witch option of this
parameter.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.21

## Parameter
## Name
Parameter IDSetting Notes
PLR Evaluate
Period for
VoLTE
Quality HO
CellHoParaCfg.VolteQualPktLo
ssPeriod
To promptly hand over
UEs suffering from low
voice quality through
SRVCC, you are advised
to set this parameter to
a value less than 5. (The
unit is second.)
VoLTE Qual
## Based Inter-
## RAT HO
## QCI1 PLR
## Thld
CellHoParaCfg.Qci1PlrThldForV
olteQualHo
To achieve favorable
voice quality in a cell,
you are advised to set
this parameter to a
value ranging from 10 to
- (The unit is %.)
VoLTE
## Quality
## Recovery
## QCI1 PLR
## Thld
CellHoParaCfg.VolteQualRecov
eryQci1PlrThld
The value of this
parameter must be less
than that of the
CellHoParaCfg.Qci1PlrT
hldForVolteQualHo
parameter. The default
value is recommended.

●  Scenario 4: Service-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-7 Parameters used for the activation of service-based SRVCC to
## UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
Algo switch
ENodeBAlgoSwitch.HoAlgoSwi
tch
Select the
UtranServiceHoSwitch
option of this parameter.
CN Operator
## ID
CnOperatorQciPara.CnOperato
rId
Set these parameters
based on QCI-specific
handover policies.
QoS Class
## Indication
CnOperatorQciPara.Qci
## Service-
based Inter-
## RAT
## Handover
## Policy Group
## ID
CnOperatorQciPara.ServiceIrHo
CfgGroupId
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.22

## Parameter
## Name
Parameter IDSetting Notes
CN Operator
## ID
ServiceIrHoCfgGroup.CnOperat
orId
## Service-
based inter-
## RAT
handover
policy group
## ID
ServiceIrHoCfgGroup.ServiceIr
HoCfgGroupId
Inter-RAT
handover
state
ServiceIrHoCfgGroup.InterRatH
oState

●  Scenario 5: Distance-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-8 Parameters used for the activation of distance-based SRVCC to
## UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Distance-
based
## Handover
## Switch
CellAlgoSwitch.DistBasedHoSw
itch
Set this parameter to
## ON.
## Distance-
based
## Measuremen
t Object Type
DistBasedHO.DistBasedMeasO
bjType
Set this parameter to
## UTRAN.

●  Scenario 6: Uplink-quality-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-9 Parameters used for the activation of uplink-quality-based SRVCC
to UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
Algo switch
ENodeBAlgoSwitch.HoAlgoSwi
tch
Select the
UlQualityInterRATHoS-
witch option of this
parameter.

eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.23

●  Scenario 7: Load-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-10 Parameters used for the activation of load-based SRVCC to
## UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Load
balancing
algorithm
switch
CellAlgoSwitch.MlbAlgoSwitchSelect the
UtranMlbSwitch option
of this parameter.
## Load
balancing
algorithm
switch
CellAlgoSwitch.MlbAlgoSwitchSelect the
MlbLoadInfoSwitch
option of this parameter.
## Overlap
## Indicator
UtranNCell.OverlapIndIf a neighboring cell is
manually identified as a
cell that has coverage
overlap with the local
cell, it is recommended
that this parameter be
set to YES for the
neighboring cell.
Support RIM
by
eCoordinator
## Switch
ENodeBAlgoSwitch.RimOnEcoS
witch
Set this parameter to
## OFF.
## Choose
UMTS Cell
## Load Info
## Trans
## Channel
GlobalProcSwitch.UtranLoadTr
ansChan
The value
BASED_ON_RIM is
recommended.

●  Scenario 8: SPID-based SRVCC to UTRAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to UTRAN has been enabled.
Table 4-11 Parameters used for the activation of SPID-based SRVCC to
## UTRAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
Algo switch
ENodeBAlgoSwitch.HoAlgoSwi
tch
Select the
InterPlmnHoSwitch
option of this parameter.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.24

## Parameter
## Name
Parameter IDSetting Notes
## RAT
frequency
priority
group ID
RatFreqPriorityGroup.RatFreqP
riorityGroupId
Set these parameters as
required.
RAT TypeRatFreqPriorityGroup.RatType
DL Earfcn or
## Bandclass
RatFreqPriorityGroup.DlEarfcn
PriorityRatFreqPriorityGroup.Priority
SpidSpidCfg.Spid
CN Operator
## ID
InterPlmnHoList.CnOperatorId
## Target
## Mobile
country code
InterPlmnHoList.TarMcc
## Target
## Mobile
network
code
InterPlmnHoList.TarMnc
## RAT
frequency
priority
indication
SpidCfg.RatFreqPriorityIndSet this parameter to
## CFG.
SPID-based
## Handover
## Back To
## HPLMN
## Switch
SpidCfg.HoBackToHPLMNSwitc
h
Set this parameter to
## TRUE.

Parameters Used for Optimization
Table 4-12 lists the parameters used for optimization.
Table 4-12 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
HO and E-
RAB Conflict
## Processing
## Strategy
GlobalProcSwitch.HoErabConflPr
ocessingStrat
Set this parameter to
## ERAB_FLOW_FIRST.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.25

## Parameter
## Name
Parameter IDSetting Notes
## Protocol
## Message
## Optimization
## Switch
GlobalProcSwitch.ProtocolMsgO
ptSwitch
It is recommended that
the
SRVCCHoBasedUeCapS-
witch option of this
parameter be selected in
the following scenarios:
● UTRAN-to-EUTRAN PS
handover is activated
on the live network
and some UEs cannot
report SRVCC capability
information to the core
network while
performing services in
the UTRAN.
● On the live network,
there are voice service
UEs handed over from
NG-RAN to E-UTRAN
or EPS fallback UEs,
and these UEs need to
be handed over to the
UTRAN through SRVCC.
However, the SRVCC
will fail because the
SRVCCOperationPossi-
ble IE will not be
delivered from the core
network in this
scenario.
SRVCC with
PSHO Based
UTRAN Cell
## Capb Switch
CnOperatorHoCfg.SrvccWithPsBa
sedCellCapSw
If the CS+PS SRVCC policy
is used and this parameter
is set to ON, the eNodeB
does not check the
UtranExternalCell.CsPsH
OInd
parameter setting
for external UTRAN cells.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.26

## Parameter
## Name
Parameter IDSetting Notes
## SRVCC
## Handover
## Optimization
## Switch
CellHoParaCfg.SrvccHoOptSwitc
h
If the CS+PS SRVCC policy
is used, it is recommended
that the
## SRVCCWITHPSCSRETRY-
SWITCH option of this
parameter be selected to
ensure that the eNodeB
initiates a CS handover
preparation attempt in the
original target cell in case
the handover preparation
for CS+PS SRVCC fails.
## Multi-
## Operator
## Control
## Switch
ENodeBAlgoSwitch.MultiOpCtrlS
witch
Select the
UtranSepOpMobility-
Switch option of this
parameter if some
operators or RNCs do not
support PS handover to
UTRAN, VoIP, or SRVCC.
## Mobile
country code
UtranNetworkCapCfg.MccIf the neighboring cell
works in RAN sharing
mode, set this parameter
to the MCC of the primary
operator.
If the peer UTRAN
equipment is provided by
Huawei, set this
parameter to the same
value as the
corresponding parameter
in the URNCBASIC MO of
the peer RNC.
## Mobile
network code
UtranNetworkCapCfg.MncIf the neighboring cell
works in RAN sharing
mode, set this parameter
to the MNC of the
primary operator.
If the peer UTRAN
equipment is provided by
Huawei, set this
parameter to the same
value as the
corresponding parameter
in the URNCBASIC MO of
the peer RNC.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.27

## Parameter
## Name
Parameter IDSetting Notes
RNC IDUtranNetworkCapCfg.RncIdIf the peer UTRAN
equipment is provided by
Huawei, set this
parameter to the same
value as the
corresponding parameter
in the URNCBASIC MO of
the peer RNC.
## Network
## Capability
## Configuration
UtranNetworkCapCfg.NetworkC
apCfg
The VoipCapCfg option is
selected by default.
Deselect this option for
operators or RNCs that do
not support PS handover,
VoIP, or SRVCC.
## Network
## Capability
## Configuration
UtranNetworkCapCfg.NetworkC
apCfg
Select the PsHoCapCfg
option for operators or
RNCs that support PS
handover, VoIP, or SRVCC.
## Network
## Capability
## Configuration
UtranNetworkCapCfg.NetworkC
apCfg
The SrvccCapCfg option is
selected by default.
Deselect this option for
operators or RNCs that do
not support PS handover,
VoIP, or SRVCC.

4.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
Before using MML commands, refer to 4.3.2 Software and complete the
parameter configurations for related functions based on the dependency
relationships between the functions, as well as the actual network scenario.
## Activation Command Examples
Before running the following MML commands, add neighboring UTRAN
frequencies and neighbor relationships with UTRAN cells, and set parameters for
inter-RAT measurements. For details about parameter settings, see the MML-
based configurations for basic mobility management functions in
## Mobility
Management in Connected Mode
## .
●  Scenario 1: Coverage-based SRVCC to UTRAN
–   SRVCC to UTRAN using the VoLTE PS handover policy
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.28

//Selecting the UtranVoipCapSwitch option of the Handover Mode switch parameter
MOD ENODEBALGOSWITCH: HoModeSwitch=UtranVoipCapSwitch-1;
//Selecting the UtranSrvccSwitch and UtranPsHoSwitch options of the Handover Mode switch
parameter
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=UtranSrvccSwitch-1&UtranPsHoSwitch-1;
//Setting the InterRAT policy config group ID parameter to 0, selecting the PS_HO option of the
UTRAN handover policy Configuration parameter and deselecting the SRVCC and REDIRECTION
options of this parameter, and setting the No handover flag parameter to PERMIT_HO_ENUM
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0,
UtranHoCfg=SRVCC-0&PS_HO-1&REDIRECTION-0, NoHoFlag=PERMIT_HO_ENUM;
//Setting the InterRAT Policy Config Group ID parameter to 0 for QCI 1
MOD QCIPARA: Qci=1, InterRatPolicyCfgGroupId=0;
//Setting the routing area code
MOD UTRANEXTERNALCELL: Mcc="460", Mnc="20", RncId=48, CellId=12, RacCfgInd=CFG,
## Rac=89;
–   CS-only SRVCC to UTRAN
//Selecting the UtranSrvccSwitch option of the Handover Mode switch parameter
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=UtranSrvccSwitch-1;
//Setting the InterRAT policy config group ID parameter to 0, selecting the SRVCC option of the
UTRAN handover policy Configuration parameter and deselecting the PS_HO and REDIRECTION
options of this parameter, and setting the No handover flag parameter to PERMIT_HO_ENUM
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0,
UtranHoCfg=SRVCC-1&PS_HO-0&REDIRECTION-0, NoHoFlag=PERMIT_HO_ENUM;
//Setting the HO and E-RAB Conflict Processing Strategy parameter to ERAB_FLOW_FIRST
MOD GLOBALPROCSWITCH: HoErabConflProcessingStrat=ERAB_FLOW_FIRST;
//Setting the InterRAT Policy Config Group ID parameter to 0 for QCI 1
MOD QCIPARA: Qci=1, InterRatPolicyCfgGroupId=0;
//Setting the QCI Priority For Handover parameter for QCI 1 and QCI 5. Ensure that the priority
for QCI 1 is higher than that for QCI 5.
MOD CELLQCIPARA: LocalCellId=0, Qci=1, QciPriorityForHo=1;
MOD CELLQCIPARA: LocalCellId=0, Qci=5, QciPriorityForHo=9;
–   CS+PS SRVCC to UTRAN (Before running following commands, ensure
that CS-only SRVCC to UTRAN has been enabled.)
//Selecting the UtranSrvccSwitch and UtranPsHoSwitch options of the Handover Mode switch
parameter
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=UtranSrvccSwitch-1&UtranPsHoSwitch-1;
//Setting the InterRAT policy config group ID parameter to 0 and selecting the PS_HO option of
the UTRAN handover policy Configuration parameter
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0, UtranHoCfg=PS_HO-1;
//Setting the SRVCC with PSHO Based UTRAN Cell Capb Switch parameter to OFF
MOD CNOPERATORHOCFG: CnOperatorId=0, SrvccWithPsBasedCellCapSw=OFF;
//Setting the routing area code, and setting the CS and PS handover indicator parameter to
## BOOLEAN_TRUE
MOD UTRANEXTERNALCELL: Mcc="460", Mnc="20", RncId=48, CellId=12, RacCfgInd=CFG,
Rac=89, CsPsHOInd=BOOLEAN_TRUE;
●  Scenario 2: LCS-based SRVCC to UTRAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to UTRAN
has been enabled.)
//Selecting the LcsSrvccSwitch option of the Handover Mode switch parameter
MOD ENODEBALGOSWITCH: HoModeSwitch=LcsSrvccSwitch-1;
//Setting the UTRAN LCS capability parameter to ON
MOD CSFALLBACKBLINDHOCFG: CnOperatorId=0, UtranLcsCap=ON;
●  Scenario 3: Voice-quality-based SRVCC to UTRAN
//Selecting the UtranVolteQualityHoSwitch option of the VoLTE Quality Handover Algo Switch
parameter and setting the PLR Evaluate Period for VoLTE Quality HO, VoLTE Qual Based Inter-RAT HO
QCI1 PLR Thld, and VoLTE Quality Recovery QCI1 PLR Thld parameters
MOD CELLHOPARACFG: LocalCellId=0, VoLTEQualityHoAlgoSwitch=UtranVolteQualityHoSwitch-1,
VolteQualPktLossPeriod=2, Qci1PlrThldForVolteQualHo=10, VolteQualRecoveryQci1PlrThld=5;
●  Scenario 4: Service-based SRVCC to UTRAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to UTRAN
has been enabled.)
//Selecting the UtranServiceHoSwitch option of the Handover Algo switch parameter
MOD ENODEBALGOSWITCH: HoAlgoSwitch=UtranServiceHoSwitch-1;
//Selecting the SRVCC option of the UTRAN handover policy Configuration parameter and setting the
No handover flag parameter to PERMIT_HO_ENUM for all inter-RAT policy configuration groups
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.29

MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0, UtranHoCfg=SRVCC-1,
NoHoFlag=PERMIT_HO_ENUM;
//Setting the handover parameters for services with a specified QCI
MOD CNOPERATORQCIPARA: CnOperatorId=0, Qci=1, ServiceIrHoCfgGroupId=0;
MOD SERVICEIRHOCFGGROUP: CnOperatorId=0, ServiceIrHoCfgGroupId=0,
InterRatHoState=MUST_HO;
●  Scenario 5: Distance-based SRVCC to UTRAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to UTRAN
has been enabled.)
MOD CELLALGOSWITCH: LocalCellId=0, DistBasedHoSwitch=ON;
MOD DISTBASEDHO: LocalCellId=0, DistBasedMeasObjType=UTRAN-1;
●  Scenario 6: Uplink-quality-based SRVCC to UTRAN (Before running the
following commands, ensure that CS-only or CS+PS coverage-based SRVCC to
UTRAN has been enabled.)
MOD ENODEBALGOSWITCH: HoAlgoSwitch=UlQualityInterRATHoSwitch-1;
●  Scenario 7: Load-based SRVCC to UTRAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to UTRAN
has been enabled.)
//Enabling MLB by transferring UL-sync UEs
MOD CELLALGOSWITCH: LocalCellId=0, MlbAlgoSwitch=UtranMlbSwitch-1;
//Enabling load information acquisition
MOD CELLALGOSWITCH: LocalCellId=0, MlbAlgoSwitch=MlbLoadInfoSwitch-1;
//Setting the Choose UMTS Cell Load Info Trans Channel parameter to BASED_ON_RIM
MOD GLOBALPROCSWITCH: UtranLoadTransChan=BASED_ON_RIM;
//Enabling core-network-based RIM
MOD ENODEBALGOSWITCH: RimOnEcoSwitch=OFF;
●  Scenario 8: SPID-based SRVCC to UTRAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to UTRAN
has been enabled.)
//Selecting the InterPlmnHoSwitch option of the Handover Algo switch parameter
MOD ENODEBALGOSWITCH: HoAlgoSwitch=InterPlmnHoSwitch-1;
//Configuring a RAT/frequency priority group
ADD RATFREQPRIORITYGROUP: RatFreqPriorityGroupId=0, RatType=UTRAN, DlEarfcn=40340,
## Priority=4;
//Setting the SPID-based Handover Back To HPLMN Switch parameter to TRUE
ADD SPIDCFG: Spid=1, RatFreqPriorityInd=CFG, HoBackToHPLMNSwitch=TRUE;
//Configuring the PLMN information for inter-PLMN handovers
ADD INTERPLMNHOLIST: CnOperatorId=0, TarMcc="460", TarMnc="30";
## Optimization Configuration Examples
●  (Optional) If some operators or neighboring UTRAN cells do not support
SRVCC to UTRAN, run the following commands:
ADD UTRANNETWORKCAPCFG: Mcc="460", Mnc="32", RncId=0, NetworkCapCfg=SrvccCapCfg-0;
MOD ENODEBALGOSWITCH: MultiOpCtrlSwitch=UtranSepOpMobilitySwitch-1;
●  (Optional) If the CS+PS SRVCC policy is used, turn on
SRVCCWITHPSCSRETRYSWITCH to ensure that the eNodeB initiates a CS
handover preparation attempt in the target cell in case the handover
preparation for CS+PS SRVCC fails.
MOD CELLHOPARACFG: LocalCellId=0, SrvccHoOptSwitch=SRVCCWITHPSCSRETRYSWITCH-1;
●  (Optional) The eNodeB may fail to obtain the "SRVCC operation possible" IE
from the MME when a UE initiates an SRVCC procedure. To address this issue,
turn on SRVCCHoBasedUeCapSwitch so that the eNodeB can trigger SRVCC
without the need to check whether it has obtained the "SRVCC operation
possible" IE from the MME.
MOD GLOBALPROCSWITCH: ProtocolMsgOptSwitch=SRVCCHoBasedUeCapSwitch-1;
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.30

## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=UtranSrvccSwitch-0;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
Coverage-based SRVCC to UTRAN
The activation of coverage-based SRVCC to UTRAN can be verified by using the
methods described below.
●  Tracing signaling messages of a single UE
Perform S1 interface tracing for a single UE. If the traced Handover Required
message contains the SRVCC HO Indication IE, as shown in Figure 4-3,
coverage-based SRVCC to UTRAN has been activated.
Figure 4-3 Handover Required message containing the SRVCC HO Indication
## IE
Figure 4-4 Signaling traced for CS+PS SRVCC
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.31

Figure 4-5 Signaling traced for CS-only SRVCC
●  Observing performance counters
Observe the L.IRATHO.SRVCC.E2W.ExecAttOut counter. If this counter
produces a non-zero value, the function has taken effect.
Voice-quality-based SRVCC to UTRAN
Verify the activation of this function when coverage-based SRVCC to UTRAN has
taken effect. If the L.IRATHO.E2W.VolteQuality.ExecAttOut counter produces a
non-zero value, this function has taken effect.
LCS-based SRVCC
Verify the activation of this function when coverage-based SRVCC to UTRAN has
taken effect. If a CS fallback triggering cause is included in the Handover Required
message traced in the single-UE standard S1 signaling tracing, this function has
taken effect.
SRVCC Triggered by Other Causes
Verify the activation of SRVCC triggered by other causes when coverage-based
SRVCC to UTRAN has taken effect. For the verification methods, refer to Table
## 4-13.
Table 4-13 Verification methods
SRVCC Type
## Reference Document
Service-based SRVCCService-, distance-, and uplink-quality-based SRVCC
handovers are inter-RAT handovers. For details on the
activation verification methods of these handovers, see
corresponding "Activation Verification" sections in
Mobility Management in Connected Mode.
Distance-based SRVCC
## Uplink-quality-based
## SRVCC
Load-based SRVCCLoad-based SRVCC handovers are performed for load
transfer. For details on the activation verification
method of load-based SRVCC, see the "Activation
Verification" section for the "MLB by transferring UL-
Sync UEs" function in Inter-RAT Mobility Load
## Balancing
## .
SPID-based SRVCCFor details, see the "Activation Verification" section for
the SPID-specific handover back to HPLMN policy in
## Flexible User Steering.
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.32


## 4.4.3 Network Monitoring
The performance counters related to SRVCC to UTRAN are listed in Table 4-14.
The following KPIs can be used to monitor the SRVCC success rate. To obtain
statistics on the voice interruption period and PS service interruption period,
collect and analyze logs on the UE side.
●SRVCC Success Rate (LTE to WCDMA)
●SRVCC Success Rate (LTE to TD-SCDMA)
Table 4-14 Performance counters for monitoring SRVCC to UTRAN
Counter IDCounter Name
1526728400L.IRATHO.SRVCC.E2W.PrepAttOut
1526728401L.IRATHO.SRVCC.E2W.ExecAttOut
1526728402L.IRATHO.SRVCC.E2W.ExecSuccOut
1526728406L.IRATHO.SRVCC.E2T.PrepAttOut
1526728407L.IRATHO.SRVCC.E2T.ExecAttOut
1526728408L.IRATHO.SRVCC.E2T.ExecSuccOut
1526728894L.IRATHO.SRVCC.E2W.MMEAbnormRsp
1526728896L.IRATHO.SRVCC.E2T.MMEAbnormRsp

Table 4-15 lists the performance counters for monitoring LCS-based SRVCC when
UEs are running services with QCI 1.
●  Success rate of LCS-based SRVCC from E-UTRAN to WCDMA network =
(L.IRATHO.SRVCC.LCS.E2W.ExecSuccOut –
L.IRATHO.SRVCC.E2W.MMEAbnormRsp)/
L.IRATHO.SRVCC.LCS.E2W.ExecAttOut x 100%
●  Success rate of LCS-based SRVCC from E-UTRAN to TD-SCDMA network =
(L.IRATHO.SRVCC.LCS.E2T.ExecSuccOut –
L.IRATHO.SRVCC.E2T.MMEAbnormRsp)/
L.IRATHO.SRVCC.LCS.E2T.ExecAttOut x 100%
Table 4-15 Performance counters for monitoring LCS-based SRVCC
Counter ID
## Counter Name
1526728409L.CSFB.LCS.PrepAtt
1526728410L.CSFB.LCS.PrepSucc
1526728753L.IRATHO.SRVCC.LCS.E2W.PrepAttOut
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.33

Counter IDCounter Name
1526728754L.IRATHO.SRVCC.LCS.E2W.ExecAttOut
1526728755L.IRATHO.SRVCC.LCS.E2W.ExecSuccOut
1526728759L.IRATHO.SRVCC.LCS.E2T.PrepAttOut
1526728760L.IRATHO.SRVCC.LCS.E2T.ExecAttOut
1526728761L.IRATHO.SRVCC.LCS.E2T.ExecSuccOut

Table 4-16 lists the performance counters for monitoring voice-quality-based
## SRVCC.
Success rate of voice-quality-based SRVCC to UTRAN =
L.IRATHO.E2W.VolteQuality.ExecSuccOut/
L.IRATHO.E2W.VolteQuality.ExecAttOut x 100%
Table 4-16 Performance counters for monitoring voice-quality-based SRVCC
Counter IDCounter Name
1526743689L.IRATHO.E2W.VolteQuality.ExecSuccOut
1526743688L.IRATHO.E2W.VolteQuality.ExecAttOut
1526743687L.IRATHO.E2W.VolteQuality.PrepAttOut

For voice-quality-based SRVCC, check the values of UL.FER and DL.FER in the
results of the VQI Monitoring task on the MAE-Access to monitor the uplink and
downlink voice packet loss rates.
## NO TE
For details about real-time monitoring on the MAE-Access, see Fault Management in MAE
## Product Documentation
## .
Table 4-17 lists the performance counters for monitoring SRVCC triggered for
emergency calls.
●  Success rate of handovers from E-UTRAN to WCDMA network for SRVCC
triggered for emergency calls = (L.EMC.SRVCC.E2W.ExecSuccOut –
L.IRATHO.SRVCC.E2W.MMEAbnormRsp)/L.EMC.SRVCC.E2W.ExecAttOut x
## 100%
●  Success rate of handovers from E-UTRAN to TD-SCDMA network for SRVCC
triggered for emergency calls = (L.EMC.SRVCC.E2T.ExecSuccOut –
L.IRATHO.SRVCC.E2T.MMEAbnormRsp)/L.EMC.SRVCC.E2T.ExecAttOut x
## 100%
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.34

Table 4-17 Performance counters for monitoring SRVCC triggered for emergency
calls
Counter IDCounter Name
1526729517L.EMC.SRVCC.E2W.PrepAttOut
1526729518L.EMC.SRVCC.E2W.ExecAttOut
1526729519L.EMC.SRVCC.E2W.ExecSuccOut
1526729523L.EMC.SRVCC.E2T.PrepAttOut
1526729524L.EMC.SRVCC.E2T.ExecAttOut
1526729525L.EMC.SRVCC.E2T.ExecSuccOut

Table 4-18 lists the performance counters related to the causes of the failures of
SRVCC to UTRAN.
Table 4-18 Performance counters related to the causes of the failures of SRVCC to
## UTRAN
Counter ID
## Counter Name
1526730082L.IRATHO.E2W.SRVCC.Prep.FailOut.MME
1526730083L.IRATHO.E2W.SRVCC.Prep.FailOut.PrepFailure
1526730084L.IRATHO.E2W.SRVCC.Prep.FailOut.NoReply
1526730085L.IRATHO.E2T.SRVCC.Prep.FailOut.MME
1526730086L.IRATHO.E2T.SRVCC.Prep.FailOut.PrepFailure
1526730087L.IRATHO.E2T.SRVCC.Prep.FailOut.NoReply
1526742170L.IRATHO.SRVCC.FailOut.HOCancel.ReEst
eRAN
SRVCC Feature Parameter Description4 SRVCC to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.35

5 SRVCC to GERAN
## 5.1 Principles
In this document, the SRVCC to GERAN function refers to coverage-based SRVCC
to GERAN. This function is controlled by the GeranSrvccSwitch option of the
CellHoParaCfg.
HoModeSwitch parameter.
Coverage-based SRVCC to GERAN is a type of inter-RAT handover. For details on
its triggering mechanism, see the descriptions of coverage-based inter-RAT
handover to GERAN in
Mobility Management in Connected Mode. This function
serves as a basis for SRVCC triggered by other causes. For details about SRVCC
triggered by other causes, see 5.1.1 Triggering.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.36

Figure 5-1 SRVCC procedure
## 5.1.1 Triggering
SRVCC can be triggered for different causes. SRVCC triggered for different causes
is controlled by separate parameters.
Voice-Quality-based SRVCC
This function is controlled by the GeranVolteQualityHoSwitch option of the
CellHoParaCfg.
VoLTEQualityHoAlgoSwitch parameter.
After this function is enabled, if the uplink packet loss rate of the bearer with QCI
1 or downlink packet loss rate of the bearer with QCI 1 of a VoLTE UE exceeds the
threshold specified by the CellHoParaCfg.
Qci1PlrThldForVolteQualHo parameter
within a voice quality decision period specified by the
CellHoParaCfg.
VolteQualPktLossPeriod parameter, the eNodeB determines that
the voice quality of the UE is poor and starts event B1 measurement for a
handover to the GERAN. The threshold for event B1 related to voice-quality-based
SRVCC is the same as that for coverage-based SRVCC.
## NO TE
●  In high-speed railway scenarios, the high voice packet loss rate persists due to high
speed mobility even after UEs are handed over to a GERAN. Voice quality cannot be
improved. Therefore, it is not recommended that voice-quality-based SRVCC be used in
high-speed railway scenarios.
●  To reduce the gap-assisted measurement's impact on voice quality and incurred air
interface signaling overheads, the eNodeB triggers voice-quality-based inter-RAT
handover measurement only once for a UE in a cell during a voice call.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.37

LCS-based SRVCC
This function is controlled by the LcsSrvccSwitch option of the
ENodeBAlgoSwitch.HoModeSwitch parameter. This function also depends on the
GERAN LCS capability, which is controlled by the
CSFallBackBlindHoCfg.GeranLcsCap parameter.
LCS-based SRVCC is used when a UE triggers LCS in an E-UTRAN network that
supports VoLTE services but does not support LCS. When the UE initiates LCS, the
MME delivers a CS Fallback Indicator to the eNodeB. The eNodeB performs SRVCC
to hand over the UE to the CS domain for LCS while maintaining voice service
continuity.
LCS-based SRVCC has the same target cell signal requirements as CSFB to GERAN.
For details on the requirements, see
CS Fallback.
SRVCC Triggered by Other Causes
SRVCC TypeSwitch for SRVCC to
## GERAN
## Reference Document
## Service-based
## SRVCC
GeranServiceHoSwitch
option of the
ENodeBAlgoSwitch.HoAl
goSwitch parameter
Service-, distance-, and uplink-
quality-based SRVCC
handovers are inter-RAT
handovers. For details on the
triggering mechanisms of
these handovers, see
corresponding sections in
Mobility Management in
## Connected Mode
## .
## Distance-based
## SRVCC
GERAN option of the
DistBasedHO.DistBasedM
easObjType parameter,
and
CellAlgoSwitch.DistBased
HoSwitch
parameter
## Uplink-quality-
based SRVCC
UlQualityInterRATHoS-
witch option of the
ENodeBAlgoSwitch.HoAl
goSwitch parameter
## Load-based
## SRVCC
GeranMlbSwitch option
of the
CellAlgoSwitch.MlbAlgoS
witch parameter
Load-based SRVCC handover
is a load transfer method. For
details on its triggering
mechanisms, see Inter-RAT
## Mobility Load Balancing
## .

5.1.2 Measurement and Target Cell Selection
The measurement and target cell selection for SRVCC to GERAN are similar to
those for SRVCC to UTRAN. For details, see 4.1.2 Measurement and Target Cell
Selection. The measurement for coverage-based SRVCC to GERAN is enhanced.
The enhancement is controlled by the GSM_MEAS_DEL_INTERFREQ_SW option of
the CellAlgoSwitch.
MeasOptAlgoSwitch parameter. With the enhancement, the
eNodeB flexibly configures the coexistence duration of GERAN measurements and
inter-frequency measurements for VoLTE UEs that are moving out of the E-UTRAN
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.38

coverage, regardless of whether coverage-based GERAN measurements are
triggered before or after VoLTE services are started. The configuration is as follows:
●  If the GERAN A2 triggering quantity is RSRP, the
InterRatHoCommGroup.
DelIfMeasA2ThdRsrpOffset parameter is used to
specify the offset to the threshold for deleting inter-frequency measurements
("offset" is used for short in the following description). The threshold for
deleting inter-frequency measurements ("threshold" is used for short in the
following description) is InterRatHoCommGroup.
InterRatHoA2ThdRsrp +
CnOperatorHoCfg.GeranA2ThdRsrpOffset (excluding –100) + Offset.
–   If the offset is set to 0, the eNodeB does not deliver the threshold and
deletes inter-frequency measurements when starting GERAN
measurements.
–   If the offset is set to a value less than 0, the eNodeB delivers the
threshold when starting GERAN measurements.
●  If the GERAN A2 triggering quantity is RSRQ, the
InterRatHoCommGroup.
DelIfMeasA2ThdRsrqOffset parameter is used to
specify the offset to the threshold for deleting inter-frequency measurements
("offset" is used for short in the following description). The threshold for
deleting inter-frequency measurements ("threshold" is used for short in the
following description) is InterRatHoCommGroup.
InterRatHoA2ThdRsrq +
## Offset.
–   If the offset is set to 0, the eNodeB does not deliver the threshold and
deletes inter-frequency measurements when starting GERAN
measurements.
–   If the offset is set to a value less than 0, the eNodeB delivers the
threshold when starting GERAN measurements.
The larger the offset, the sooner the deletion of inter-frequency measurements. As
a result, the GERAN measurement time is shortened and the service drop rate is
decreased. In addition, the GSM_MEAS_RECOVER_INTERFREQ_SW option of the
CellAlgoSwitch
.MeasOptAlgoSwitch parameter can be selected to resume inter-
frequency measurements when UEs move to E-UTRAN coverage areas.
If SRVCC to UTRAN and SRVCC to GERAN are supported on the network, the
eNodeB delivers measurement configurations, instructing the UEs to measure
neighboring UTRAN and GERAN cells. Cells in the first valid measurement report
are selected as target cells for SRVCC. It is recommended that the
GlobalProcSwitch.
HoErabConflProcessingStrat parameter be set to
ERAB_FLOW_FIRST to increase the SRVCC handover success rate. Under this
setting, the eNodeB preferentially handles the QCI-1 bearer deletion procedure
when the SRVCC and QCI-1 bearer deletion procedure conflict.
5.1.3 Handover Policy Selection for SRVCC
Figure 5-2 shows the procedure for selecting a handover policy for SRVCC to
GERAN when QCI-1 bearers exist. The following handover policies are selected in
sequence:
## 1.  CS+PS SRVCC
-  CS-only SRVCC
If the requirements of the preceding two handover policies are not met, a
handover will not be performed.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.39

## NO TE
QCI-1 bearers are used to carry VoLTE services. If redirection is used as the handover policy
for QCI 1, a call drop will occur during redirection. Therefore, redirection cannot be used as
the handover policy for VoLTE services (of QCI 1). The redirection handover policy is
controlled by the REDIRECTION option of the
InterRatPolicyCfgGroup.
GeranGprsEdgeHoCfg parameter.
Figure 5-2 Procedure for selecting a handover policy for SRVCC to GERAN
## CS+PS SRVCC
CS+PS SRVCC can be triggered if the following requirements are met:
●  SRVCC to GERAN is enabled.
If some operators or neighboring GERAN cells on the network do not support
SRVCC, operators' or neighboring GERAN cells' capability to support SRVCC
can be set as follows:
–   Enable the Separate Mobility Policies to GERAN for Multi PLMN function,
which is controlled by the GeranSepOpMobilitySwitch option of the
CellAlgoSwitch.
HoAllowedSwitch parameter.
–Configure the SRVCC capability of specific operators or neighboring
GERAN cells, which is specified by the GeranNetworkCapCfg.
## Mcc,
GeranNetworkCapCfg.
Mnc, and GeranNetworkCapCfg.Lac parameters,
and the SrvccCapCfg option of the
GeranNetworkCapCfg.
NetworkCapCfg parameter. SRVCC is supported
by an operator or a neighboring GERAN cell by default if the SRVCC
capability is not configured.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.40

●  PS handover from E-UTRAN to GERAN is enabled. This function is controlled
by the GeranPsHoSwitch option of the ENodeBAlgoSwitch.HoModeSwitch
parameter.
●  The GeranNfreqGroup.
GeranVersion parameter is set to GPRS or EDGE.
●  SRVCC and PS handover are specified as QCI-specific handover policies. SRVCC
and PS handover are controlled by the SRVCC and PS_HO options of the
InterRatPolicyCfgGroup.
GeranGprsEdgeHoCfg parameter, respectively.
These handover policies can be associated with a specific QCI by setting the
QciPara.
InterRatPolicyCfgGroupId parameter.
If services with different QCIs exist, the handover policy for the highest-
priority QCI prevails. The handover policy priority for each QCI is specified by
the CellQciPara.QciPriorityForHo parameter. It is recommended that the
handover policy priority be set to the highest priority (1) for QCI 1 and the
lowest priority (9) for QCI 5.
## NO TE
●  For necessary handovers, for example, voice-quality-based, coverage-based, and
uplink-quality-based handovers, SRVCC can be triggered when SRVCC is configured
in the inter-RAT handover policy group for the highest-priority QCI.
●  For unnecessary handovers, for example, load-based, service-based, and CSFB-
based handovers, SRVCC can be triggered when SRVCC is configured in the inter-
RAT handover policy groups for all QCIs. If the Handover Command message sent
from the MME to the eNodeB for an unnecessary handover contains the "E-RABs
To Release List" IE, the eNodeB will cancel the handover.
●  The GeranExternalCell.
CsPsHOInd parameter, which specifies whether an
external GERAN cell supports CS+PS SRVCC, is set to BOOLEAN_TRUE.
●  The GeranExternalCell.
DtmInd parameter, which specifies whether a GERAN
cell supports dual transmission mode (DTM), is set to DTM_AVAILABLE.
CS-only SRVCC
CS-only SRVCC can be triggered if the following requirements are met:
●  SRVCC to GERAN is enabled.
If some operators or neighboring GERAN cells on the network do not support
SRVCC, operators' or neighboring GERAN cells' capability to support SRVCC
can be set as follows:
–   Enable the Separate Mobility Policies to GERAN for Multi PLMN function,
which is controlled by the GeranSepOpMobilitySwitch option of the
CellAlgoSwitch.
HoAllowedSwitch parameter.
–Configure the SRVCC capability of specific operators or neighboring
GERAN cells, which is specified by the GeranNetworkCapCfg.
## Mcc,
GeranNetworkCapCfg.Mnc, and GeranNetworkCapCfg.Lac parameters,
and the SrvccCapCfg option of the
GeranNetworkCapCfg.
NetworkCapCfg parameter. SRVCC is supported
by an operator or a neighboring GERAN cell by default if the SRVCC
capability is not configured.
●  SRVCC is specified as a QCI-specific handover policy. The SRVCC policy is
controlled by the SRVCC option of the
InterRatPolicyCfgGroup.
GeranGsmHoCfg and
InterRatPolicyCfgGroup.
GeranGprsEdgeHoCfg parameters. The policy can
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.41

be associated with a specific QCI by setting the
QciPara.InterRatPolicyCfgGroupId parameter.
If services with different QCIs exist, the handover policy for the highest-
priority QCI prevails. The handover policy priority for each QCI is specified by
the CellQciPara.QciPriorityForHo parameter. It is recommended that the
handover policy priority be set to the highest priority (1) for QCI 1 and the
lowest priority (9) for QCI 5.
## NO TE
●  For necessary handovers, for example, voice-quality-based, coverage-based, and
uplink-quality-based handovers, SRVCC can be triggered when SRVCC is configured
in the inter-RAT handover policy group for the highest-priority QCI.
●  For unnecessary handovers, for example, load-based, service-based, and CSFB-
based handovers, SRVCC can be triggered when SRVCC is configured in the inter-
RAT handover policy groups for all QCIs. If the Handover Command message sent
from the MME to the eNodeB for an unnecessary handover contains the "E-RABs
To Release List" IE, the eNodeB will cancel the handover.
5.1.4 Retry and Penalty
The handling for SRVCC to GERAN is similar to that for SRVCC to UTRAN. For
details, see 4.1.4 Retry and Penalty. The special handling for SRVCC to GERAN is
as follows:
SRVCC failures mostly occur during SRVCC to GERAN. To reduce such failures, a
penalty timer (specified by the HoMeasComm.
SrvccHoFailurePenaltyTimer
parameter) can be set for the source E-UTRAN cell and target neighboring GERAN
cell involved in SRVCC failures. Before the timer expires, the eNodeB forbids all
UEs in the source E-UTRAN cell from initiating SRVCC to the neighboring GERAN
cell.
## 5.2 Network Analysis
## 5.2.1 Benefits
By handing VoLTE services over to the CS domain of a GERAN, SRVCC to GERAN
ensures call continuity for UEs when the UEs move out of an E-UTRAN to a
## GERAN.
## 5.2.2 Impacts
## Network Impacts
If the target GERAN of a CS-only SRVCC procedure supports DTM, only QCI-1
bearers are diverted to the CS domain of the GERAN. Bearers with other QCIs are
reestablished for PS services in the GERAN only after an RAU procedure. If the
GERAN does not support DTM, QCI-1 bearers are diverted to the GERAN but PS
services are suspended.
Activating voice-quality-based SRVCC also has the following impacts on network
performance:
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.42

●  UEs with poor voice quality are handed over to a GERAN through SRVCC,
which improves their voice quality.
●  After UEs with poor voice quality are handed over to the GERAN through
SRVCC, the percentage of VoLTE UEs in the LTE network decreases.
Deleting inter-frequency measurements during SRVCC to GERAN reduces the
service drop rate in the following scenarios:
●  There is GSM coverage but no inter-frequency LTE coverage.
●  GSM coverage and inter-frequency LTE coverage coexist.
●  Signals of the serving cell attenuate quickly but maintain at least 3s.
## Function Impacts
## None
## 5.3 Requirements
## 5.3.1 Licenses
The following are FDD license requirements.
## RAT
Feature IDFeature
## Name
ModelSales Unit
FDDLOFD-001023SRVCC to
## GERAN
LT1SSRVCCG00per RRC
## Connected
## User

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
No requirements
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.43

## Boards
No requirements
RF Modules
No requirements
## 5.3.4 Others
## Core Network
●  If the core network equipment is provided by Huawei, the core network
version for eRAN6.0 or later is required. If the core network version is not for
eRAN6.0 or later, exceptions such as message parsing failure may occur.
●  If the core network equipment is provided by another vendor, check the
software version of the core network to make sure that the core network
supports SRVCC complying with 3GPP Release 8 or later.
5.4 Operation and Maintenance
## 5.4.1 Data Configuration
## 5.4.1.1 Data Preparation
Before configuring SRVCC to GERAN, collect the data related to neighbor
relationships with GERAN cells. This section provides only the information about
MOs related to neighboring GERAN cells. For more information about how to
collect data for the parameters in these MOs, see
Mobility Management in
## Connected Mode
## .
1.GeranNfreqGroup: used to configure neighboring GERAN carrier frequency
groups.
2.GeranNfreqGroupArfcn: used to configure absolute radio frequency channel
numbers (ARFCNs) in each neighboring GERAN carrier frequency group.
3.GeranExternalCell: used to configure external GERAN cells. If CS+PS SRVCC is
enabled, you need to set the GeranExternalCell.
Rac and
GeranExternalCell.CsPsHOInd parameters.
-  (Optional) GeranExternalCellPlmn: used to configure additional PLMN IDs
for each shared external GERAN cell. This MO is required only if the BTS that
serves the external GERAN cell works in RAN sharing with common carriers
mode and two or more operators share the external GERAN cell.
5.GeranNcell: used to configure neighbor relationships with GERAN cells.
Parameters Used for Activation
●  Scenario 1: Coverage-based SRVCC to GERAN
–   CS-only SRVCC to GERAN
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.44

Table 5-1 Parameters used for the activation of coverage-based CS-only
SRVCC to GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
GeranSrvccSwitch
option of this
parameter.
## GERAN
## GSM
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGsmHoCfg
Select the SRVCC
option of this
parameter.
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Select the SRVCC
option of this
parameter.
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Deselect the PS_HO
option of this
parameter.
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Deselect the
REDIRECTION option
of this parameter.
## No
handover
flag
InterRatPolicyCfgGroup.NoH
oFlag
It is recommended that
the default value be
used if there is no
special requirement for
forbidding certain
handovers.
InterRAT
policy
config
group ID
InterRatPolicyCfgGroup.Inter
RatPolicyCfgGroupId
Set this parameter to
the same value as the
QciPara.InterRatPolicy
CfgGroupId parameter.
QoS Class
## Identifier
QciPara.QciSet this parameter as
required. For example,
set this parameter to 1.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.45

## Parameter
## Name
Parameter IDSetting Notes
InterRAT
## Policy
## Config
Group ID
QciPara.InterRatPolicyCfg-
GroupId
Set this parameter to
the same value as the
InterRatPolicyCfgGrou
p.InterRatPolicyCfg-
GroupId parameter.
QCI Priority
## For
## Handover
CellQciPara.QciPriorityForHoIt is recommended that
this parameter be set
to the highest priority
(1) for QCI 1.

–   CS+PS SRVCC to GERAN
Set parameters in the following table when CS-only SRVCC to GERAN has
been enabled.
Table 5-2 Parameters used for the activation of coverage-based CS+PS
SRVCC to GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
## Mode
switch
CellHoParaCfg.HoModeSwitc
h
Select the
GeranSrvccSwitch
option of this
parameter.
## Handover
## Mode
switch
ENodeBAlgoSwitch.HoModeS
witch
Select the
GeranPsHoSwitch
option of this
parameter.
## GERAN
version
GeranNfreqGroup.GeranVersi
on
Set this parameter to
GPRS or EDGE.
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Select the SRVCC
option of this
parameter.
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Select the PS_HO
option of this
parameter.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.46

## Parameter
## Name
Parameter IDSetting Notes
## GERAN
## GPRS EDGE
handover
policy
## Configuratio
n
InterRatPolicyCfgGroup.Gera
nGprsEdgeHoCfg
Deselect the
REDIRECTION option
of this parameter.
## No
handover
flag
InterRatPolicyCfgGroup.NoH
oFlag
It is recommended that
the default value be
used if there is no
special requirement for
forbidding certain
handovers.
InterRAT
policy
config
group ID
InterRatPolicyCfgGroup.Inter
RatPolicyCfgGroupId
Set this parameter to
the same value as the
QciPara.InterRatPolicy
CfgGroupId parameter.
QoS Class
## Identifier
QciPara.QciSet this parameter as
required. For example,
set this parameter to 1.
InterRAT
## Policy
## Config
Group ID
QciPara.InterRatPolicyCfg-
GroupId
Set this parameter to
the same value as the
InterRatPolicyCfgGrou
p.InterRatPolicyCfg-
GroupId
parameter.
QCI Priority
## For
## Handover
CellQciPara.QciPriorityForHoIt is recommended that
this parameter be set
to the highest priority
(1) for QCI 1.
CS and PS
handover
indication
GeranExternalCell.CsPsHOIndSet this parameter to
## BOOLEAN_TRUE.
## DTM
indication
GeranExternalCell.DtmIndSet this parameter to
## DTM_AVAILABLE.

●  Scenario 2: LCS-based SRVCC to GERAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to GERAN has been enabled.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.47

Table 5-3 Parameters used for the activation of LCS-based SRVCC to GERAN
## Parameter
## Name
Parameter IDSetting Notes
## GERAN LCS
capability
CSFallBackBlind-
HoCfg.GeranLcsCap
Set this parameter to
## ON.
## Handover
Mode switch
ENodeBAlgoSwitch.HoModeSw
itch
Select the
LcsSrvccSwitch option
of this parameter.

●  Scenario 3: Voice-quality-based SRVCC to GERAN
Table 5-4 Parameters used for the activation of voice-quality-based SRVCC to
## GERAN
## Parameter
## Name
Parameter IDSetting Notes
VoLTE
## Quality
## Handover
## Algo Switch
CellHoParaCfg.VoLTEQualityHo
AlgoSwitch
Select the
GeranVolteQualityHoS-
witch option of this
parameter.
PLR Evaluate
Period for
VoLTE
Quality HO
CellHoParaCfg.VolteQualPktLo
ssPeriod
To promptly hand over
UEs suffering from low
voice quality through
SRVCC, you are advised
to set this parameter to
a value less than 5. (The
unit is second.)
VoLTE Qual
## Based Inter-
## RAT HO
## QCI1 PLR
## Thld
CellHoParaCfg.Qci1PlrThldForV
olteQualHo
To achieve favorable
voice quality in a cell,
you are advised to set
this parameter to a
value ranging from 10 to
- (The unit is %.)
VoLTE
## Quality
## Recovery
## QCI1 PLR
## Thld
CellHoParaCfg.VolteQualRecov
eryQci1PlrThld
The value of this
parameter must be less
than that of the
CellHoParaCfg.Qci1PlrT
hldForVolteQualHo
parameter. The default
value is recommended.

●  Scenario 4: Service-based SRVCC to GERAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to GERAN has been enabled.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.48

Table 5-5 Parameters used for the activation of service-based SRVCC to
## GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
Algo switch
ENodeBAlgoSwitch.HoAlgoSwi
tch
Select the
GeranServiceHoSwitch
option of this parameter.
CN Operator
## ID
CnOperatorQciPara.CnOperato
rId
Set these parameters
based on QCI-specific
handover policies.
QoS Class
## Indication
CnOperatorQciPara.Qci
## Service-
based Inter-
## RAT
## Handover
## Policy Group
## ID
CnOperatorQciPara.ServiceIrHo
CfgGroupId
CN Operator
## ID
ServiceIrHoCfgGroup.CnOperat
orId
## Service-
based inter-
## RAT
handover
policy group
## ID
ServiceIrHoCfgGroup.ServiceIr
HoCfgGroupId
Inter-RAT
handover
state
ServiceIrHoCfgGroup.InterRatH
oState

●  Scenario 5: Distance-based SRVCC to GERAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to GERAN has been enabled.
Table 5-6 Parameters used for the activation of distance-based SRVCC to
## GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Distance-
based
## Handover
## Switch
CellAlgoSwitch.DistBasedHoSw
itch
Set this parameter to
## ON.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.49

## Parameter
## Name
Parameter IDSetting Notes
## Distance-
based
## Measuremen
t Object Type
DistBasedHO.DistBasedMeasO
bjType
Set this parameter to
## GERAN.

●  Scenario 6: Uplink-quality-based SRVCC to GERAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to GERAN has been enabled.
Table 5-7 Parameters used for the activation of uplink-quality-based SRVCC
to GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Handover
Algo switch
ENodeBAlgoSwitch.HoAlgoSwi
tch
Select the
UlQualityInterRATHoS-
witch option of this
parameter.

●  Scenario 7: Load-based SRVCC to GERAN
Set parameters in the following table when coverage-based CS-only or CS+PS
SRVCC to GERAN has been enabled.
Table 5-8 Parameters used for the activation of load-based SRVCC to GERAN
## Parameter
## Name
Parameter IDSetting Notes
## Load
balancing
algorithm
switch
CellAlgoSwitch.MlbAlgoSwitchSelect the
GeranMlbSwitch option
of this parameter.

Parameters Used for Optimization
Table 5-9 lists the parameters used for optimization.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.50

Table 5-9 Parameters used for optimization
## Parameter
## Name
Parameter IDSetting Notes
## Measurement
## Optimization
## Algorithm
## Switch
CellAlgoSwitch.MeasOptAlgoSwi
tch
Select the
## GSM_MEAS_DEL_INTERF
REQ_SW option of this
parameter.
## Measurement
## Optimization
## Algorithm
## Switch
CellAlgoSwitch.MeasOptAlgoSwi
tch
Select the
## GSM_MEAS_RECOVER_IN
TERFREQ_SW option of
this parameter.
Del Inter-Freq
## Meas A2 Thld
RSRP Offset
InterRatHoCommGroup.DelIfMe
asA2ThdRsrpOffset
A larger value of each
parameter indicates
earlier deletion of inter-
frequency measurements
after GERAN
measurements are started.
As a result, GERAN
measurements and inter-
frequency measurements
co-exist for a shorter
period and the delay in
GERAN measurement
reporting is shorter.
Del Inter-Freq
## Meas A2 Thld
RSRQ Offset
InterRatHoCommGroup.DelIfMe
asA2ThdRsrqOffset
HO and E-
RAB Conflict
## Processing
## Strategy
GlobalProcSwitch.HoErabConflPr
ocessingStrat
Set this parameter to
## ERAB_FLOW_FIRST.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.51

## Parameter
## Name
Parameter IDSetting Notes
## Protocol
## Message
## Optimization
## Switch
GlobalProcSwitch.ProtocolMsgO
ptSwitch
It is recommended that
the
SRVCCHoBasedUeCapS-
witch option of this
parameter be selected in
the following scenarios:
● GERAN-to-EUTRAN PS
handover is activated
on the live network
and some UEs cannot
report SRVCC capability
information to the core
network while
performing services in
the GERAN.
● On the live network,
there are voice service
UEs handed over from
NG-RAN to E-UTRAN
or EPS fallback UEs,
and these UEs need to
be handed over to the
GERAN through SRVCC.
However, the SRVCC
will fail because the
SRVCCOperationPossi-
ble IE will not be
delivered from the core
network in this
scenario.
## Handover
## Allowed
## Switch
CellAlgoSwitch.HoAllowedSwitc
h
Select the
GeranSepOpMobility-
Switch option of this
parameter if some
operators or neighboring
GERAN cells do not
support the RIM
procedure to the GERAN.
## Mobile
country code
GeranNetworkCapCfg.MccIf the peer GERAN
equipment is provided by
Huawei, set each
parameter to the same
value as the
corresponding parameter
in the GCELL MO of the
peer BSC.
## Mobile
network code
GeranNetworkCapCfg.Mnc
## Location Area
## Code
GeranNetworkCapCfg.Lac
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.52

## Parameter
## Name
Parameter IDSetting Notes
## Network
## Capability
## Configuration
GeranNetworkCapCfg.NetworkC
apCfg
The SrvccCapCfg option is
selected by default.
Deselect it for operators
or neighboring GERAN
cells that do not support
SRVCC to GERAN.

5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
●  Scenario 1: Coverage-based SRVCC to GERAN
–   CS-only SRVCC to GERAN
//Selecting the GeranSrvccSwitch option of the Handover Mode switch parameter
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=GeranSrvccSwitch-1;
//Setting the InterRAT policy config group ID parameter to 0, selecting the SRVCC option of the
GERAN GSM handover policy Configuration parameter, selecting the SRVCC option of the
GERAN GPRS EDGE handover policy Configuration parameter and deselecting the PS_HO and
REDIRECTION options of this parameter, and setting the No handover flag parameter to
## PERMIT_HO_ENUM
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0, GeranGsmHoCfg=SRVCC-1,
GeranGprsEdgeHoCfg=SRVCC-1&PS_HO-0&REDIRECTION-0, NoHoFlag=PERMIT_HO_ENUM;
//Setting the HO and E-RAB Conflict Processing Strategy parameter to ERAB_FLOW_FIRST
MOD GLOBALPROCSWITCH: HoErabConflProcessingStrat=ERAB_FLOW_FIRST;
//Setting the InterRAT Policy Config Group ID parameter to 0 for QCI 1
MOD QCIPARA: Qci=1, InterRatPolicyCfgGroupId=0;
//Setting the QCI Priority For Handover parameter for QCI 1 and QCI 5. Ensure that the priority
for QCI 1 is higher than that for QCI 5.
MOD CELLQCIPARA: LocalCellId=0, Qci=1, QciPriorityForHo=1;
MOD CELLQCIPARA: LocalCellId=0, Qci=5, QciPriorityForHo=9;
–   CS+PS SRVCC to GERAN (Before running following commands, ensure
that CS-only SRVCC to GERAN has been enabled.)
//Deselecting the UtranPsHoSwitch option of the Handover Mode switch parameter
MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=UtranPsHoSwitch-0;
//Selecting the GeranPsHoSwitch option of the Handover Mode switch parameter
MOD ENODEBALGOSWITCH: HoModeSwitch=GeranPsHoSwitch-1;
//Setting the InterRAT policy config group ID parameter to 0 and selecting the PS_HO option of
the GERAN GPRS EDGE handover policy Configuration parameter
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0,
GeranGprsEdgeHoCfg=PS_HO-1;
//Setting the CS and PS handover indication parameter to BOOLEAN_TRUE and DTM indication
parameter to DTM_AVAILABLE
MOD GERANEXTERNALCELL: Mcc="460", Mnc="20", GeranCellId=15, Lac=12, RacCfgInd=CFG,
Rac=89, BandIndicator=GSM_dcs1800, DtmInd=DTM_AVAILABLE, CsPsHOInd=BOOLEAN_TRUE;
●  Scenario 2: LCS-based SRVCC to GERAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to GERAN
has been enabled.)
MOD ENODEBALGOSWITCH: HoModeSwitch=LcsSrvccSwitch-1;
MOD CSFALLBACKBLINDHOCFG: CnOperatorId=0, GeranLcsCap=ON;
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.53

●  Scenario 3: Voice-quality-based SRVCC to GERAN
MOD CELLHOPARACFG: LocalCellId=0, VoLTEQualityHoAlgoSwitch=GeranVolteQualityHoSwitch-1,
VolteQualPktLossPeriod=2, Qci1PlrThldForVolteQualHo=10, VolteQualRecoveryQci1PlrThld=5;
●  Scenario 4: Service-based SRVCC to GERAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to GERAN
has been enabled.)
//Selecting the GeranServiceHoSwitch option of the Handover Algo switch parameter
MOD ENODEBALGOSWITCH: HoAlgoSwitch=GeranServiceHoSwitch-1;
//Selecting the SRVCC options of the GERAN GSM handover policy Configuration and GERAN GPRS
EDGE handover policy Configuration parameters and setting the No handover flag parameter to
PERMIT_HO_ENUM for all inter-RAT policy configuration groups
MOD INTERRATPOLICYCFGGROUP: InterRatPolicyCfgGroupId=0,
GeranGsmHoCfg=SRVCC-1,GeranGprsEdgeHoCfg=SRVCC-1, NoHoFlag=PERMIT_HO_ENUM;
//Setting the handover parameters for services with a specified QCI
MOD CNOPERATORQCIPARA: CnOperatorId=0, Qci=1, ServiceIrHoCfgGroupId=0;
MOD SERVICEIRHOCFGGROUP: CnOperatorId=0, ServiceIrHoCfgGroupId=0,
InterRatHoState=MUST_HO;
●  Scenario 5: Distance-based SRVCC to GERAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to GERAN
has been enabled.)
MOD CELLALGOSWITCH: LocalCellId=0, DistBasedHoSwitch=ON;
MOD DISTBASEDHO: LocalCellId=0, DistBasedMeasObjType=GERAN-1;
●  Scenario 6: Uplink-quality-based SRVCC to GERAN (Before running the
following commands, ensure that CS-only or CS+PS coverage-based SRVCC to
GERAN has been enabled.)
MOD ENODEBALGOSWITCH: HoAlgoSwitch=UlQualityInterRATHoSwitch-1;
●  Scenario 7: Load-based SRVCC to GERAN (Before running the following
commands, ensure that CS-only or CS+PS coverage-based SRVCC to GERAN
has been enabled.)
MOD CELLALGOSWITCH: LocalCellId=0, MlbAlgoSwitch=GeranMlbSwitch-1;
## Optimization Configuration Examples
●  (Optional) If some operators or neighboring GSM cells do not support SRVCC
to GERAN, run the following commands:
ADD GERANNETWORKCAPCFG: Mcc="460", Mnc="32", Lac=1, NetworkCapCfg=SrvccCapCfg-0;
MOD CELLALGOSWITCH: LocalCellId=0, HoAllowedSwitch=GeranSepOpMobilitySwitch-1;
●  (Optional) To enable fast return from GERAN to E-UTRAN after SRVCC, run
the following command:
MOD GLOBALPROCSWITCH: ProtocolMsgOptSwitch=IratMeasCfgTransSwitch-1;
●  (Optional) If inter-frequency measurements need to be deleted after GERAN
measurements for SRVCC are started, run the following commands:
MOD CELLALGOSWITCH: LocalCellId=0,
MeasOptAlgoSwitch=GSM_MEAS_DEL_INTERFREQ_SW-1&GSM_MEAS_RECOVER_INTERFREQ_SW-1;
MOD INTERRATHOCOMMGROUP: LocalCellId=0, InterRatHoCommGroupId=0,
DelIfMeasA2ThdRsrqOffset=0, DelIfMeasA2ThdRsrpOffset=0;
●  (Optional) The eNodeB may fail to obtain the "SRVCC operation possible" IE
from the MME when a UE initiates an SRVCC procedure. To address this issue,
turn on SRVCCHoBasedUeCapSwitch so that the eNodeB can trigger SRVCC
without the need to check whether it has obtained the "SRVCC operation
possible" IE from the MME.
MOD GLOBALPROCSWITCH: ProtocolMsgOptSwitch=SRVCCHoBasedUeCapSwitch-1;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.54

MOD CELLHOPARACFG: LocalCellId=0, HoModeSwitch=GeranSrvccSwitch-0;
5.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
Coverage-based SRVCC to GERAN
Trace signaling messages of a single UE and observe counters to verify function
activation. The procedure for verification by tracing the signaling messages of a
single UE for coverage-based SRVCC to GERAN is the same as that for coverage-
based SRVCC to UTRAN. For details, see 4.4.2 Activation Verification.
Observe the counters described in Table 5-10. If a counter produces a non-zero
value, the related function has been activated.
Table 5-10 Mapping between counters and functions
FunctionCounter IDCounter Name
SRVCC to GERAN1526728404L.IRATHO.SRVCC.E2G.ExecAttOut
## Voice-quality-based
SRVCC to GERAN
1526743691L.IRATHO.E2G.VolteQuality.ExecAttOu
t

Voice-quality-based SRVCC to GERAN
Verify the activation of this function when coverage-based SRVCC to GERAN has
taken effect. If the L.IRATHO.E2G.VolteQuality.ExecAttOut counter produces a
non-zero value, this function has taken effect.
LCS-based SRVCC
Verify the activation of this function when coverage-based SRVCC to UTRAN has
taken effect. If a CS fallback triggering cause is included in the Handover Required
message traced in the single-UE standard S1 signaling tracing, this function has
taken effect.
SRVCC Triggered by Other Causes
Verify the activation of SRVCC triggered by other causes when coverage-based
SRVCC to GERAN has taken effect. For the verification methods, refer to Table
## 5-11.
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.55

Table 5-11 Verification methods
SRVCC TypeReference Document
Service-based SRVCCService-, distance-, and uplink-quality-based SRVCC
handovers are inter-RAT handovers. For details on the
activation verification methods of these handovers, see
corresponding "Activation Verification" sections in
Mobility Management in Connected Mode.
Distance-based SRVCC
## Uplink-quality-based
## SRVCC
Load-based SRVCCLoad-based SRVCC handovers are performed for load
transfer. For details on the activation verification
method of load-based SRVCC, see the "Activation
Verification" section for the "MLB by transferring UL-
Sync UEs" function in Inter-RAT Mobility Load
## Balancing
## .

## 5.4.3 Network Monitoring
The performance counters related to SRVCC to GERAN are listed in Table 5-12.
The following KPIs can be used to monitor the SRVCC success rate. To obtain
statistics on the voice interruption period and PS service interruption period when
the GERAN supports DTM, collect and analyze logs on the UE side.
SRVCC Success Rate (LTE to GSM)
Table 5-12 Performance counters for monitoring SRVCC to GERAN
Counter ID
## Counter Name
1526728403L.IRATHO.SRVCC.E2G.PrepAttOut
1526728404L.IRATHO.SRVCC.E2G.ExecAttOut
1526728405L.IRATHO.SRVCC.E2G.ExecSuccOut
1526728895L.IRATHO.SRVCC.E2G.MMEAbnormRsp

Table 5-13 lists the performance counters for monitoring LCS-based SRVCC when
UEs are running services with QCI 1.
Success rate of LCS-based SRVCC to GERAN =
(L.IRATHO.SRVCC.LCS.E2G.ExecSuccOut –
L.IRATHO.SRVCC.E2G.MMEAbnormRsp)/L.IRATHO.SRVCC.LCS.E2G.ExecAttOut x
## 100%
Table 5-13 Performance counters for monitoring LCS-based SRVCC
Counter ID
## Counter Name
1526728409L.CSFB.LCS.PrepAtt
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.56

Counter IDCounter Name
1526728410L.CSFB.LCS.PrepSucc
1526728756L.IRATHO.SRVCC.LCS.E2G.PrepAttOut
1526728757L.IRATHO.SRVCC.LCS.E2G.ExecAttOut
1526728758L.IRATHO.SRVCC.LCS.E2G.ExecSuccOut

Table 5-14 lists the performance counters for monitoring voice-quality-based
SRVCC to GERAN.
Success rate of voice-quality-based SRVCC to GERAN =
L.IRATHO.E2G.VolteQuality.ExecSuccOut/
L.IRATHO.E2G.VolteQuality.ExecAttOut x 100%
Table 5-14 Performance counters for monitoring voice-quality-based SRVCC to
## GERAN
Counter IDCounter Name
1526743690L.IRATHO.E2G.VolteQuality.PrepAttOut
1526743691L.IRATHO.E2G.VolteQuality.ExecAttOut
1526743692L.IRATHO.E2G.VolteQuality.ExecSuccOut

For voice-quality-based SRVCC, check the values of UL.FER and DL.FER in the
results of the VQI Monitoring task on the MAE-Access to monitor the uplink and
downlink voice packet loss rates.
## NO TE
For details about real-time monitoring on the MAE-Access, see Fault Management in MAE
## Product Documentation
## .
Table 5-15 lists the performance counters for monitoring SRVCC triggered for
emergency calls.
Success rate of SRVCC to GERAN triggered for emergency calls =
(L.EMC.SRVCC.E2G.ExecSuccOut – L.IRATHO.SRVCC.E2G.MMEAbnormRsp)/
L.EMC.SRVCC.E2G.ExecAttOut x 100%
Table 5-15 Performance counters for monitoring SRVCC triggered for emergency
calls
Counter ID
## Counter Name
1526729520L.EMC.SRVCC.E2G.PrepAttOut
1526729521L.EMC.SRVCC.E2G.ExecAttOut
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.57

Counter IDCounter Name
1526729522L.EMC.SRVCC.E2G.ExecSuccOut

Table 5-16 lists the counters related to the causes of the failures of SRVCC to
## GERAN.
Table 5-16 Counters related to the causes of the failures of SRVCC to GERAN
Counter IDCounter Name
1526730088L.IRATHO.E2G.SRVCC.Prep.FailOut.MME
1526730089L.IRATHO.E2G.SRVCC.Prep.FailOut.PrepFailure
1526730090L.IRATHO.E2G.SRVCC.Prep.FailOut.NoReply
1526742170L.IRATHO.SRVCC.FailOut.HOCancel.ReEst
1526747674L.IRATHO.E2G.SRVCC.FailOut.S1WaitingTimerOut
eRAN
SRVCC Feature Parameter Description5 SRVCC to GERAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.58

6 SRVCC Flexible Steering to UTRAN
## 6.1 Principles
This function can be used when the UTRAN is a multi-frequency network and CS
and PS steering is used for these frequencies. In this scenario, the eNodeB
considers the SRVCC service priorities for the frequencies, and the operator can
achieve SRVCC from E-UTRAN to specific UTRAN frequencies carrying SRVCC
services. With this function, fewer UTRAN frequencies are measured, which
reduces the measurement time and the probability of UE errors.
This function is an enhancement of SRVCC to UTRAN and requires that E-UTRAN
to UTRAN CS/PS steering be activated. This function works only for coverage-
based SRVCC.
This function is controlled by the UtranSrvccSteeringSwitch option of the
CellAlgoSwitch.
FreqLayerSwitch parameter.
This function uses the SRVCC priorities specified by the UtranNFreq.SrvccPriority
parameter in the measurement phase.
Table 6-1 describes measurement frequency selection for different services based
on the status of this function and E-UTRAN to UTRAN CS/PS steering.
Table 6-1 Measurement frequency selection for different services
E-UTRAN to
## UTRAN CS/PS
## Steering
## SRVCC
## Flexible
Steering to
## UTRAN
## Measuremen
t Frequency
Selection for
CSFB Services
## Measuremen
t Frequency
Selection for
## SRVCC
## Services
## Measuremen
t Frequency
Selection for
PS Services
OffOffAll UTRAN
frequencies
All UTRAN
frequencies
All UTRAN
frequencies
OffOnAll UTRAN
frequencies
All UTRAN
frequencies
All UTRAN
frequencies
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.59

E-UTRAN to
## UTRAN CS/PS
## Steering
## SRVCC
## Flexible
Steering to
## UTRAN
## Measuremen
t Frequency
Selection for
CSFB Services
## Measuremen
t Frequency
Selection for
## SRVCC
## Services
## Measuremen
t Frequency
Selection for
PS Services
OnOffOnly UTRAN
frequencies
with the
highest CS
service
priority
Only UTRAN
frequencies
with the
highest PS
service
priority
Only UTRAN
frequencies
with the
highest PS
service
priority
OnOnOnly UTRAN
frequencies
with the
highest CS
service
priority
Only UTRAN
frequencies
with the
highest
SRVCC service
priority
Only UTRAN
frequencies
with the
highest PS
service
priority
Note: If there are multiple highest-priority frequencies, the eNodeB randomly
selects a maximum permissible number of these frequencies and instructs the
UE to measure the selected frequencies. The maximum permissible number is
specified by the CellUeMeasControlCfg.MaxUtranFddMeasFreqNum
parameter.

## NO TE
For details about RAT priority parameter settings for inter-RAT handovers, see related
descriptions in Mobility Management in Connected Mode.
## 6.2 Network Analysis
## 6.2.1 Benefits
With this function, fewer UTRAN frequencies are measured, which reduces the
measurement time and the probability of UE errors.
## 6.2.2 Impacts
## Network Impacts
With SRVCC flexible steering to UTRAN, UEs measure only UTRAN frequencies
with the highest SRVCC service priority. They do not measure UTRAN frequencies
with a low SRVCC service priority even if the measurement of the frequencies with
the highest SRVCC service priority fails. If there are coverage holes in the area
covered by the UTRAN frequencies with the highest SRVCC service priority, the
SRVCC success rate may decrease.
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.60

## Function Impacts
## None
## 6.3 Requirements
## 6.3.1 Licenses
The following are FDD license requirements.
Feature IDFeature NameModelSales Unit
LOFD-001087SRVCC Flexible
Steering to UTRAN
## LT1S00SFSU0
## 0
per RRC
## Connected User

## 6.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## Function Name
Function SwitchReference
SRVCC to UTRANUtranSrvccSwitch option of the
CellHoParaCfg.HoModeSwitch
parameter
## SRVCC
## Coverage-based
E-UTRAN to
## UTRAN CS/PS
steering
UtranFreqLayerMeasSwitch option of
the CellAlgoSwitch.FreqLayerSwitch
parameter
## Mobility
Management in
## Connected Mode

## Mutually Exclusive Functions
## None
## 6.3.3 Hardware
This section is the same as the counterpart for SRVCC to UTRAN. For details, see
## 4.3.3 Hardware.
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.61

## 6.3.4 Others
## Core Network
●  If the core network equipment is provided by Huawei, the core network
version for eRAN6.0 or later is required. If the core network version is not for
eRAN6.0 or later, exceptions such as message parsing failure may occur.
●  If the core network equipment is provided by another vendor, check the
software version of the core network to make sure that the core network
supports SRVCC complying with 3GPP Release 8 or later.
6.4 Operation and Maintenance
## 6.4.1 Data Configuration
## 6.4.1.1 Data Preparation
Table 6-2 describes the parameters used for function activation.
Table 6-2 Parameters used for activation
## Parameter
## Name
Parameter IDSetting Notes
## Frequency
## Layer Switch
CellAlgoSwitch.FreqLayerSwitchSelect the
UtranSrvccSteeringS-
witch and
UtranFreqLayerMeasS-
witch options of this
parameter.
SRVCC Service
## Priority
UtranNFreq.SrvccPriorityIf this parameter is set to
Priority_0, the eNodeB
does not select the
frequency. The values
Priority_16 and Priority_1
indicate the highest and
lowest priorities,
respectively.
Set a high priority for a
UTRAN frequency with
good coverage.

## NO TE
As described in section 8.1.2.1.1.1 of 3GPP TS 36.133 V10.1.0, a UE is capable of measuring
at least three UTRAN frequencies. To ensure compatibility with UE capabilities, assign the
highest SRVCC priority to three UTRAN frequencies at most.
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.62

6.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
Before using MML commands, refer to 6.3.2 Software and complete the
parameter configurations for related functions based on the dependency
relationships between the functions, as well as the actual network scenario.
//Selecting the UtranFreqLayerMeasSwitch and UtranSrvccSteeringSwitch options of the Frequency Layer
Switch parameter
MOD CELLALGOSWITCH: LocalCellId=0,
FreqLayerSwitch=UtranFreqLayerMeasSwitch-1&UtranSrvccSteeringSwitch-1;
//Setting the SRVCC Service Priority parameter to Priority_16
MOD UTRANNFREQ: LocalCellId=0, UtranDlArfcn=10800, SrvccPriority=Priority_16;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Deactivating SRVCC flexible steering to UTRAN
MOD CELLALGOSWITCH: LocalCellId=0, FreqLayerSwitch=UtranSrvccSteeringSwitch-0;
6.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 6.4.2 Activation Verification
Perform Uu interface tracing for a single UE. If the tracing result indicates that the
eNodeB delivered only the UTRAN frequencies with the highest SRVCC priority to
the UE, SRVCC flexible steering to UTRAN has been activated. Figure 6-1 shows
that the eNodeB sends the measurement configuration to the UE.
Figure 6-1 Measurement configuration for SRVCC
Set SRVCC Service Priority to 16 and 2 for UTRAN frequencies 10700 and 10710,
respectively. If SRVCC flexible steering to UTRAN has been activated, the eNodeB
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.63

delivers only the UTRAN frequency 10700, which has the highest SRVCC service
priority, to the UE, as shown in Figure 6-2.
Figure 6-2 UTRAN frequency to be measured
## 6.4.3 Network Monitoring
This section is the same as the counterpart for SRVCC to UTRAN. For details, see
## 4.4.3 Network Monitoring.
eRAN
SRVCC Feature Parameter Description6 SRVCC Flexible Steering to UTRAN
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.64

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
SRVCC Feature Parameter Description7 Parameters
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.65

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
SRVCC Feature Parameter Description8 Counters
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.66

## 9 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
SRVCC Feature Parameter Description9 Glossary
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.67

## 10 Reference Documents
-  3GPP TS 23.216, "Single Radio Voice Call Continuity (SRVCC)"
-  3GPP TS 23.272, "Circuit Switched (CS) fallback in Evolved Packet System
## (EPS)"
## 3.  3GPP TS 36.133 V10.1.0
## 4.
CS Fallback
5.Mobility Management in Connected Mode
6.Flexible User Steering
7.Inter-RAT Mobility Load Balancing
8.Interoperability Between UMTS and LTE in RAN Feature Documentation
9.Fault Management in MAE Product Documentation
eRAN
SRVCC Feature Parameter Description10 Reference Documents
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.68

## 11 Appendix
## 11.1 Signaling Procedures
SRVCC to UTRAN/GERAN
Figure 11-1 shows the signaling procedure for SRVCC to UTRAN/GERAN. The
procedure is common for voice-quality-, coverage-, service-, distance-, uplink-
quality-, load-, and SPID-based SRVCC.
For details, see section 6.2 "E-UTRAN and 3GPP GERAN/UTRAN SRVCC" in 3GPP
## TS 23.216 V9.4.0.
Figure 11-1 Signaling procedure for SRVCC to UTRAN/GERAN
eRAN
SRVCC Feature Parameter Description11 Appendix
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.69

-  The eNodeB delivers the inter-RAT measurement configuration to the UE.
-  The UE responds to the eNodeB with an RRC Connection Reconfiguration
Complete message.
-  After detecting that a neighboring cell meets the condition for triggering an
inter-RAT handover, the UE sends measurement reports to the eNodeB.
-  The eNodeB determines that a handover should be performed and sends a
Handover Required message containing an SRVCC HO Indication IE to the
## MME.
-  The MME splits voice bearers from non-voice bearers, and then transmits a
Relocation Request message to the target MSC server and target SGSN.
-  After receiving the Relocation Request message, the SRVCC MSC server
instructs the target RNC or BSC to prepare for a handover. After resources are
ready, the target RNC or BSC informs the target MSC server. The preparation
process for the PS service handover on the target SGSN is the same as that
for inter-RAT PS service handover. The conversion of the media plane is
implemented in the IMS.
## NO TE
If the value of the SRVCC HO Indication IE is "CS Only" in the Handover Required
message sent from the eNodeB to the MME, the MME instructs only the MSC server to
prepare for a handover. If the value of the SRVCC HO Indication IE is "PS and CS", the
MME instructs both the MSC server and SGSN to prepare for handovers.
For a CS-only SRVCC procedure, if the target network is UTRAN, the PS services of the
UE resume during a routing area update (RAU) procedure in the UTRAN. If the target
network is GERAN, PS service handling depends on whether the UE and BSC support
DTM. If both the UE and BSC support DTM, the PS services of the UE resume during
an RAU procedure in the GERAN. If either the UE or the BSC does not support DTM,
the PS services of the UE are suspended.
-  The MME receives responses from relevant NEs, which are different depending
on scenarios:
–   In the CS-only SRVCC scenario, the MME receives a handover preparation
complete indication from the target MSC server.
–   In the CS+PS SRVCC scenario, the MME receives handover preparation
complete indications from the target MSC server and target SGSN.
-  The MME delivers a handover command to the eNodeB.
-  The eNodeB delivers the handover command to the UE.
- After receiving the handover command, the UE accesses the target network.
- The UE sends the target RAN a Handover Complete message, indicating that
the handover procedure for SRVCC is complete.
LCS-based SRVCC
Figure 11-2 shows the signaling procedure for LCS-based SRVCC.
eRAN
SRVCC Feature Parameter Description11 Appendix
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.70

Figure 11-2 Signaling procedure for LCS-based SRVCC
Steps in the preceding figure are described as follows:
-  Steps 1 to 5: A CSFB procedure is triggered for a UE performing VoIP services
in an E-UTRAN network that does not support LCS when the eNodeB or core
network needs to trigger LCS. The UE sends the MME an Extended Service
Request message containing a CS Fallback Indicator.
-  Step 6: The MME sends a CS Fallback Indicator to the eNodeB. The eNodeB
determines that QCI 1 VoIP services exist, indicating that the UE is performing
voice services instead of initiating voice services and needs to be handed over
to another inter-RAT system with LCS enabled. Then, the eNodeB instructs the
UE to measure an inter-RAT system with LCS enabled and selects a target cell
for the UE.
-  Step 7: The eNodeB determines the target cell and initiates an SRVCC
procedure to hand the UE over to the inter-RAT cell that supports LCS.
## NO TE
For details on LCS-based SRVCC procedure, see section 8.3 "Location Services (LCS)" in
## 3GPP TS 23.272 V11.9.0.
eRAN
SRVCC Feature Parameter Description11 Appendix
Issue 04 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.71