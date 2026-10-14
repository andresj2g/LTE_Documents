

eRAN
Uplink Timing Control (FDD)
## Feature Parameter Description
## Issue06
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
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 06 (2024-06-21)..................................................................................................................................................1
1.2 eRAN18.1 05 (2023-09-14)..................................................................................................................................................1
1.3 eRAN18.1 04 (2023-02-01)..................................................................................................................................................2
1.4 eRAN18.1 03 (2022-10-25)..................................................................................................................................................2
1.5 eRAN18.1 02 (2022-06-27)..................................................................................................................................................2
1.6 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.7 eRAN18.1 Draft B (2022-02-08)........................................................................................................................................ 3
1.8 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 3
2 About This Document.............................................................................................................4
2.1 General Statements................................................................................................................................................................ 4
2.2 Applicable RAT......................................................................................................................................................................... 4
2.3 Features in This Document.................................................................................................................................................. 5
3 Overview....................................................................................................................................6
4 Uplink Timing Control............................................................................................................7
4.1 Principles.................................................................................................................................................................................... 7
4.1.1 Procedure for Uplink Timing Control............................................................................................................................ 8
4.1.2 Timers Related to Uplink Timing Control................................................................................................................. 11
4.1.2.1 Uplink Time Alignment Timer................................................................................................................................... 12
4.1.2.2 Uplink Synchronization Timer................................................................................................................................... 14
4.1.2.3 UE Inactivity Timer........................................................................................................................................................ 15
4.2 Network Analysis.................................................................................................................................................................. 16
4.2.1 Benefits................................................................................................................................................................................. 16
4.2.2 Impacts..................................................................................................................................................................................17
4.3 Requirements......................................................................................................................................................................... 19
4.3.1 Licenses................................................................................................................................................................................. 19
4.3.2 Software................................................................................................................................................................................19
4.3.3 Hardware..............................................................................................................................................................................20
4.3.4 Others....................................................................................................................................................................................21
4.4 Operation and Maintenance.............................................................................................................................................21
4.4.1 Data Configuration........................................................................................................................................................... 21
4.4.1.1 Data Preparation............................................................................................................................................................ 21
eRAN
Uplink Timing Control (FDD) Feature Parameter
DescriptionContents
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iii

4.4.1.2 Using MML Commands............................................................................................................................................... 23
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 24
4.4.2 Activation Verification......................................................................................................................................................24
4.4.3 Network Monitoring.........................................................................................................................................................24
5 Parameters..............................................................................................................................26
6 Counters.................................................................................................................................. 27
7 Glossary................................................................................................................................... 28
8 Reference Documents...........................................................................................................29
eRAN
Uplink Timing Control (FDD) Feature Parameter
DescriptionContents
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 06 (2024-06-21)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Added descriptions about the counter used to observe the number of DMRS TA
scheduling times on the PUSCH. For details, see 4.4.3 Network Monitoring.
1.2 eRAN18.1 05 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description1 Change History
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.1

1.3 eRAN18.1 04 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 03 (2022-10-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 02 (2022-06-27)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.6 eRAN18.1 01 (2022-03-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description1 Change History
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.2

1.7 eRAN18.1 Draft B (2022-02-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.8 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 04 (2021-09-29).
## Technical Changes
## Change Description
## Parameter
## Change
RATBase Station
## Model
Enabled micro base stations
to support the SPID-specific
UE inactivity timer. For
details, see 4 Uplink Timing
## Control.
Added the
SpidCfg.Spid
UeInactivityT
imer
parameter.
## FDDBTS3912E
Optimized the configuration
of the interval for sending
TA commands in uplink
timing control after a
successful RA. For details,
see 4.1.1 Procedure for
## Uplink Timing Control.
NoneFDD● 3900 and
5900 series
base stations
(macro base
stations)
## ● DBS3900
LampSite
and DBS5900
LampSite
## ● BTS3912E
## ● BTS3911E
## ● BTS3203E
## ● BTS3202E

## Editorial Changes
Revised descriptions in this document.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description1 Change History
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.3

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
Uplink Timing Control (FDD) Feature Parameter
## Description2 About This Document
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.4

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-070101Uplink Timing Based on PUCCH4 Uplink Timing Control
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description2 About This Document
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.5

## 3 Overview
In a Long Term Evolution (LTE) system, multipath propagation of signals from a
UE causes intersymbol interference. Moreover, varied distances between UEs in a
cell and the eNodeB serving the cell negatively affect the orthogonality among
UEs, causing inter-UE interference.
To reduce interference, the time for sending uplink signals needs to be adjusted,
thereby ensuring an acceptable difference in time when uplink signals from
different UEs reach the eNodeB. Such adjustment is frequently required due to UE
mobility, multipath effect, and other factors.
During uplink timing control, the eNodeB measures the timing offset based on the
uplink signals received from a UE. The eNodeB then converts the timing offset into
a Timing Advance Command and delivers the command to the UE. After receiving
the command, the UE adjusts the time for sending uplink signals. This ensures
uplink synchronization between the UE and the eNodeB.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description3 Overview
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.6

## 4 Uplink Timing Control
## 4.1 Principles
Uplink timing control can be performed during or after random access (RA).
●  Uplink timing control during RA
Non-synchronized UEs, including UEs that are newly powered on, UEs
performing an incoming RRC connection reestablishment, UEs performing an
incoming handover, and UEs in RRC_IDLE mode, establish or restore uplink
synchronization based on RA.
●  Uplink timing control after RA
A synchronized UE maintains the synchronization state based on periodic
uplink timing adjustment.
A UE in RRC_CONNECTED mode can be in the synchronization or out-of-
synchronization state. The uplink time alignment timer, uplink synchronization
timer, and UE inactivity timer maintain and manage the UE states. For details
about working principles and settings of these timers, see 4.1.2.1 Uplink
Time Alignment Timer, 4.1.2.2 Uplink Synchronization Timer, and 4.1.2.3
UE Inactivity Timer.
–   If the uplink time alignment timer expires, a synchronized UE enters the
out-of-synchronization state.
–   If the uplink synchronization timer expires, this causes the uplink time
alignment timer to expire, which further makes a synchronized UE enter
the out-of-synchronization state.
–   If the UE inactivity timer expires, a synchronized UE enters the RRC_IDLE
mode.
A non-synchronized UE enters the synchronization state after completing RA.
Figure 4-1 shows how the timers maintain the UE states in uplink timing control.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.7

Figure 4-1 Timers maintaining UE states
4.1.1 Procedure for Uplink Timing Control
Uplink timing control is required to achieve uplink synchronization between a UE
and the eNodeB during RA. After a successful RA, periodic uplink timing control is
required to maintain uplink synchronization between the UE and the eNodeB.
Figure 4-2 shows the procedure for uplink timing control.
Figure 4-2 Procedure for uplink timing control
-  A UE sends a Random Access Preamble message to the eNodeB during RA.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.8

-  The eNodeB measures the timing offset of the UE based on the received
Random Access Preamble message.
-  The eNodeB converts the timing offset into a Timing Advance Command.
-  The eNodeB sends the UE a Random Access Response message containing the
## Timing Advance Command.
-  After receiving the Timing Advance Command, the UE adjusts the time for
sending uplink signals.
For details, see section 4.2.3 "Transmission timing adjustments" in 3GPP TS
## 36.213 V10.10.0.
-  After a successful RA, the eNodeB allocates uplink resources to the UE, and
the UE sends uplink signals. The resources allocated to the UE can be used for
transmitting sounding reference signals (SRS), demodulation reference signals
for the physical uplink shared channel (DMRS for PUSCH), or channel quality
indicators on the physical uplink control channel (CQI on PUCCH).
-  The eNodeB measures the timing offset of the UE based on the uplink signals
received from the UE.
For details about timing offset measurement, see Timing Offset
## Measurement.
-  The eNodeB converts the timing offset into a Timing Advance Command.
-  The eNodeB delivers the Timing Advance Command to the UE.
For details about the policy of delivering the Timing Advance Command, see
## Timing Advance Command Delivery Policy.
- After receiving the Timing Advance Command, the UE adjusts the time for
sending uplink signals.
For details, see section 4.2.3 "Transmission timing adjustments" in 3GPP TS
## 36.213 V10.10.0.
After a successful RA, steps 6 through 10 will be repeated to maintain uplink
synchronization between the UE and the eNodeB.
## Timing Offset Measurement
The timing offset can be measured based on SRS, DMRS for PUSCH, or CQI on
PUCCH. The method for measuring uplink timing offsets can be specified by the
TimeAlignmentTimer.
TimingMeasMode parameter.
●  If this parameter is set to INVALID, the timing offset of a UE is measured
based on SRS or DMRS for PUSCH.
–   If the eNodeB has allocated SRS resources to the UE (that is, the
SRSCfg.
SrsCfgInd parameter is set to BOOLEAN_TRUE), it measures the
timing offset of the UE based on SRS. If the UE has PUSCH resources, the
eNodeB measures the timing offset of the UE based on both SRS and
DMRS for PUSCH, but the timing offset measured based on SRS is
preferentially used.
–   If the eNodeB has not allocated SRS resources to the UE (that is, the
SRSCfg.
SrsCfgInd parameter is set to BOOLEAN_FALSE), it measures the
timing offset of the UE based on DMRS for PUSCH. If the UE does not
have any PUSCH resources, the eNodeB allocates PUSCH resources to the
UE and then measures the timing offset based on DMRS for PUSCH.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.9

●  If this parameter is set to ALLMEASMODE, the timing offset of a UE is
measured based on SRS, DMRS for PUSCH, or CQI on PUCCH.
–   If the eNodeB has allocated SRS resources to the UE, it measures the
timing offset of the UE based on SRS. If the UE has PUSCH resources, the
eNodeB measures the timing offset of the UE based on both SRS and
DMRS for PUSCH, but the timing offset measured based on DMRS for
PUSCH is preferentially used.
–   If the eNodeB has not allocated SRS resources to the UE, it measures the
timing offset of the UE based on DMRS for PUSCH or CQI on PUCCH.
▪If the eNodeB has configured periodic CQI resources for the UE, it
measures the timing offset of the UE based on CQI on PUCCH, and
Uplink Timing Based on PUCCH takes effect. If the UE has PUSCH
resources, the eNodeB measures the timing offset of the UE based
on both CQI on PUCCH and DMRS for PUSCH, but the timing offset
measured based on DMRS for PUSCH is preferentially used.
When the eNodeB measures the timing offset based on CQI on
PUCCH, selecting the TaEnhancePucch option of the
TimeAlignmentTimer.
TaEnhance parameter can further improve
the accuracy of PUCCH timing advance (TA) measurements.
## ▪
If the eNodeB has not configured periodic CQI resources for the UE,
it measures the timing offset of the UE based on DMRS for PUSCH. If
the UE does not have any PUSCH resources, the eNodeB allocates
PUSCH resources to the UE and then measures the timing offset
based on DMRS for PUSCH.
CQI on PUCCH occupies only a small number of resource blocks (RBs) at two ends
of a bandwidth, while SRS and DMRS for PUSCH can adaptively occupy multiple
RBs in the middle. Therefore, the time offset measured based on SRS or DMRS for
PUSCH is more accurate than that measured based on CQI on PUCCH.
You can set the TimeAlignmentTimer.
TimingResOptSwitch parameter to ON to
reduce the resources allocated by the eNodeB for timing offset measurements
based on DMRS for PUSCH and reduce unnecessary delivery of TA adjustment
commands.
If the TimeAlignmentTimer.
TimingResOptSwitch parameter is set to ON,
selecting the TaEnhancePuschDmrs option of the
TimeAlignmentTimer.TaEnhance parameter can further reduce the DMRS for
PUSCH resources allocated by the eNodeB to UEs.
## Timing Advance Command Delivery Policy
After a successful RA, a Timing Advance Command is delivered based on the
policy specified by the TimeAlignmentTimer.
TimingAdvCmdOptSwitch,
TimeAlignmentTimer.TimingMeasMode, and
TimeAlignmentTimer.
TimingResOptSwitch parameters.
●  The Timing Advance Command is periodically delivered when all of the
following conditions are met:
–   The TimeAlignmentTimer.TimingAdvCmdOptSwitch parameter is set
to OFF.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.10

–   The TimeAlignmentTimer.TimingMeasMode parameter is set to
## INVALID.
–   The TimeAlignmentTimer.TimingResOptSwitch parameter is set to
## OFF.
The interval for sending TA commands is calculated by the formula
"floor(Uplink time alignment timer length/2 – 32 ms)" and cannot be
manually set.
The uplink time alignment timer length is specified by the
TimeAlignmentTimer.
TimeAlignmentTimer parameter. If the
TimeAlignmentTimer.
TimeAlignmentTimer parameter is set to INFINITY,
the uplink time alignment timer length is 65535 ms.
●  The Timing Advance Command is delivered based on the periodic
determination and event triggering policy when any of the following
conditions is met:
–   The TimeAlignmentTimer.
TimingAdvCmdOptSwitch parameter is set
to ON.
–   The TimeAlignmentTimer.
TimingMeasMode parameter is set to
## ALLMEASMODE.
–   The TimeAlignmentTimer.TimingResOptSwitch parameter is set to ON.
The eNodeB periodically determines whether a timing offset occurs on the
## UE.
–   If a timing offset occurs on the UE, the eNodeB delivers a Timing
Advance Command to the UE.
–   If no timing offset occurs on the UE and the uplink time alignment timer
has not expired, the eNodeB does not deliver the Timing Advance
Command to the UE.
–   If no timing offset occurs on the UE before the uplink time alignment
timer expires, the UE will not receive a Timing Advance Command for a
long time. In this case, the eNodeB will deliver a Timing Advance
Command to the UE when the uplink time alignment timer is about to
expire.
The interval is specified by the TimeAlignmentTimer.
TACmdSendPeriod
parameter, which takes effect only for common cells. For high-speed cells, see
## High Speed Mobility.
–   A smaller value of this parameter indicates that TA commands are sent
more frequently. As a result, more air interface resources are consumed
and a higher UE moving speed is supported.
–   A larger value of this parameter indicates that TA commands are sent less
frequently. As a result, fewer air interface resources are consumed and a
lower UE moving speed is supported.
–   If this parameter is set to INVALID, the effective interval for sending TA
commands is min(928 ms, Uplink time alignment timer length/2 – 32
ms).
4.1.2 Timers Related to Uplink Timing Control
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.11

## 4.1.2.1 Uplink Time Alignment Timer
## Working Principles
The UE and eNodeB perform uplink synchronization using their respective uplink
time alignment timers.
●  The eNodeB uses its uplink time alignment timer to determine whether the
UE is in the uplink synchronization state. Before the timer expires, the eNodeB
determines that the UE is in the uplink synchronization state. After the timer
expires, the eNodeB determines that the UE is in the uplink out-of-
synchronization state. When the UE is in the uplink out-of-synchronization
state, the eNodeB stops delivering the Timing Advance Command to the UE,
excluding the Timing Advance Command included in the Random Access
Response message during RA.
●  The UE uses its uplink time alignment timer to determine whether it is in the
uplink synchronization state. Before the timer expires, the UE considers itself
to be in the uplink synchronization state. After the timer expires, the UE
considers itself to be in the uplink out-of-synchronization state.
Table 4-1 describes the working principles of the uplink time alignment timers.
Table 4-1 Working principles of uplink time alignment timers
## Timer
ActionDescription
Uplink time
alignment
timer on the
eNodeB side
Start● During RA:
– For a non-contention-based RA, the
eNodeB starts or restarts the timer after
receiving an acknowledgment (ACK)
from the UE that replies to the delivered
Random Access Response message
(containing the Timing Advance
## Command).
– For a contention-based RA, the eNodeB
starts or restarts the timer for the UE
that has successfully accessed the
network.
For definitions about the non-contention-
based RA and contention-based RA, see
## Random Access Control.
● After a successful RA, the eNodeB starts or
restarts the timer after receiving an ACK
from the UE that replies to the delivered
## Timing Advance Command.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.12

TimerActionDescription
Expired● If the eNodeB does not receive an ACK from
the UE after delivering the Timing Advance
Command, the eNodeB does not restart the
timer. As a result, the timer will expire.
● After the uplink synchronization timer
expires, the eNodeB no longer delivers the
Timing Advance Command to the UE and
will not receive an ACK from the UE. As
such, the eNodeB does not restart the
uplink time alignment timer, which will
therefore expire. For details about the
uplink synchronization timer, see 4.1.2.2
## Uplink Synchronization Timer.
Uplink time
alignment
timer on the
UE side
Start● When the UE receives the Timing Advance
Command included in the Random Access
Response message during RA:
– For a non-contention-based RA, the UE
starts or restarts the timer.
– For a contention-based RA, if the timer
has not started, the UE starts the timer;
if the timer has started, the UE does not
need to restart the timer. The timer stops
if the contention-based RA fails.
● Upon receiving the Timing Advance
Command after a successful RA, the UE
starts or restarts the timer.
Expired● If the UE does not receive the Timing
Advance Command from the eNodeB, the
UE does not restart the timer. As a result,
the timer will expire.
● After the uplink synchronization timer on
the eNodeB side expires, the eNodeB no
longer delivers the Timing Advance
Command to the UE. As such, the UE
cannot receive the Timing Advance
Command from the eNodeB and does not
restart the uplink time alignment timer,
which will therefore expire. For details about
the uplink synchronization timer, see 4.1.2.2
## Uplink Synchronization Timer.

Both uplink time alignment timers can be restarted before expiration to prolong
the duration of uplink synchronization. Upon receiving the Timing Advance
Command from the eNodeB, the UE restarts its uplink time alignment timer and
sends an ACK to the eNodeB. Upon receiving the ACK, the eNodeB restarts its
uplink time alignment timer, as shown in Figure 4-3.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.13

Figure 4-3 Time to restart the uplink time alignment timers
## Timer Settings
The uplink time alignment timers on the UE and eNodeB sides are controlled
independently. The TimeAlignmentTimer.
TimeAlignmentTimer parameter
specifies the uplink time alignment timer length on the eNodeB side. After being
set, the timer length is sent to the UE through air interface signaling.
●  When the TimeAlignmentTimer.
TimingAdvCmdOptSwitch parameter is set
to OFF, you are advised to set the
TimeAlignmentTimer.
TimeAlignmentTimer parameter to SF1920.
–   A smaller value of the TimeAlignmentTimer.TimeAlignmentTimer
parameter indicates that the eNodeB delivers the Timing Advance
Command to the UE more frequently, more radio resources are
consumed, and a higher UE moving speed is supported.
–   A larger value of the TimeAlignmentTimer.
TimeAlignmentTimer
parameter results in the opposite effects.
●  When the TimeAlignmentTimer.
TimingAdvCmdOptSwitch parameter is set
to ON, you are advised to set the
TimeAlignmentTimer.
TimeAlignmentTimer parameter to SF10240.
A smaller value of the TimeAlignmentTimer.TimeAlignmentTimer
parameter (for example, smaller than SF5120) leads to a higher probability of
UEs in discontinuous reception (DRX) mode entering the uplink out-of-
synchronization state. For details about the relationship between the
TimeAlignmentTimer.
TimeAlignmentTimer parameter value and the DRX
mode, see
DRX and Signaling Control.
## 4.1.2.2 Uplink Synchronization Timer
## Working Principles
The uplink synchronization timer controls whether the eNodeB continues to
maintain uplink synchronization between a UE and the eNodeB. The eNodeB
maintains an uplink synchronization timer for each UE. Table 4-2 describes the
working principles of this timer.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.14

Table 4-2 Working principles of the uplink synchronization timer
ActionDescription
StartThe eNodeB starts or restarts the timer for a UE when it
successfully sends data radio bearer (DRB) data packets to or
receives DRB data packets from the UE. Before this timer
expires, the eNodeB continuously delivers the Timing Advance
Command to the UE.
ExpireWhen the uplink synchronization timer expires, the eNodeB
no longer delivers the Timing Advance Command to the UE.
After the uplink time alignment timer on the eNodeB side
expires, the eNodeB determines that the UE enters the out-
of-synchronization state.

## Timer Settings
The uplink synchronization timer is specified by the QciPara.
UlSynTimerForQci
parameter, and is maintained only on the eNodeB side.
●  A smaller value of QciPara.UlSynTimerForQci results in a higher probability
of the UE entering the out-of-synchronization state, a shorter time for the UE
to occupy PUCCH and SRS resources, and a larger number of RA requests
initiated by the UE.
●  A larger value of QciPara.
UlSynTimerForQci results in a lower probability of
the UE entering the out-of-synchronization state, a longer time for the UE to
occupy PUCCH and SRS resources, and a smaller number of RA requests
initiated by the UE.
●  If QciPara.
UlSynTimerForQci is set to 0, the uplink synchronization timer will
never expire.
4.1.2.3 UE Inactivity Timer
## Working Principles
The eNodeB determines whether a UE is in RRC_CONNECTED mode based on the
state of the UE inactivity timer. Table 4-3 describes the working principles of this
timer.
Table 4-3 Working principles of the UE inactivity timer
## Action
## Description
StartThe eNodeB starts or restarts the timer for a UE when it
successfully sends data packets to or receives data packets
from the UE. Before this timer expires, the eNodeB
determines that the UE is in RRC_CONNECTED mode.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.15

ActionDescription
ExpireWhen the UE inactivity timer for a UE in the synchronization
state expires, the eNodeB sends an RRC Connection Release
message to the UE. The UE is then released and enters
RRC_IDLE mode. This prevents an inactive UE from occupying
radio resources for a long time.
When the UE inactivity timer for a UE in the out-of-
synchronization state expires, the UE enters the
synchronization state first. Then, the eNodeB releases the RRC
connection for the UE, and the UE enters RRC_IDLE mode.

## Timer Settings
The UE inactivity timer can be configured based on the QoS class identifier (QCI)
using the QciPara.
UeInactiveTimerForQci parameter or based on the subscriber
profile ID (SPID) using the SpidCfg.
SpidUeInactivityTimer parameter. If the
parameter specifying the SPID-specific UE inactivity timer is set to the invalid
value 65535, the QCI-specific timer takes effect. If the parameter specifying the
SPID-specific UE inactivity timer is set to a value other than 65535, the SPID-
specific timer takes effect. The UE inactivity timer is maintained only on the
eNodeB side. If the settings of the parameters for the UE inactivity timer are
changed, the changes apply only to UEs that access the network afterwards.
When a UE is not performing services:
●  A shorter UE inactivity timer length results in earlier RRC connection release
for the UE and more frequent RRC connection setup requests from the UE.
Because the number of UEs released normally increases, the service drop rate
decreases.
●  A longer UE inactivity timer length results in later RRC connection release and
longer RRC connection duration for the UE, which occupies radio resources for
a longer time. Because the number of UEs released normally decreases, the
service drop rate increases.
●  If the UE inactivity timer length is zero, the UE is always in RRC_CONNECTED
mode.
If the uplink synchronization timer length specified by the
QciPara.
UlSynTimerForQci parameter is greater than the UE inactivity timer
length specified by the QciPara.UeInactiveTimerForQci or
SpidCfg.
SpidUeInactivityTimer parameter, the UE enters RRC_IDLE mode directly.
## 4.2 Network Analysis
## 4.2.1 Benefits
With uplink timing control, the eNodeB adjusts the time for sending uplink signals
from each UE so that the time for uplink signals from different UEs to reach the
eNodeB is aligned. This ensures orthogonality of uplink signals sent by different
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.16

UEs, mitigates intra-cell interference, and maintains the demodulation
performance.
It is recommended that Uplink Timing Based on PUCCH be enabled when all of
the following conditions are met:
●  The SRS resources cannot support uplink timing required by all the UEs in the
cell.
–   The average number of uplink-synchronized UEs in a cell (measured
using the L.Traffic.User.Ulsync.Avg counter) is greater than the average
number of UEs configured with SRS resources in the cell (measured using
the L.Traffic.User.SRS.Avg counter).
–   No SRS resources are available in the cell. (The SRSCfg.
SrsCfgInd
parameter is set to BOOLEAN_FALSE.)
●  Preallocation or smart preallocation does not take effect.
When preallocation (controlled by the PreAllocationSwitch option of the
CellAlgoSwitch.
UlSchSwitch parameter) or smart preallocation (controlled
by the SmartPreAllocationSwitch option of the CellAlgoSwitch.UlSchSwitch
parameter) is enabled, the eNodeB proactively initiates uplink scheduling for
UEs that are not allocated SRS resources. In this situation, the eNodeB
measures timing offsets of UEs based on DMRS for PUSCH. If Uplink Timing
Based on PUCCH is enabled in this scenario, the eNodeB measures timing
offsets of UEs based on both DMRS for PUSCH and CQI on PUCCH. However,
the timing offsets measured based on DMRS for PUSCH are preferentially
used for uplink timing adjustment. In this situation, Uplink Timing Based on
PUCCH provides small gains.
In Uplink Timing Based on PUCCH, when the Timing Advance Command is
delivered based on the periodic determination and event triggering policy, fewer
physical downlink control channel (PDCCH) control channel elements (CCEs) and
PUSCH physical resource blocks (PRBs) are consumed for measuring uplink timing
offsets based on DMRS for PUSCH. As such, the PDCCH can support more UEs and
the uplink PRB usage decreases.
## 4.2.2 Impacts
## Network Impacts
When Uplink Timing Based on PUCCH is enabled in a cell serving a large number
of UEs and the Timing Advance Command is delivered based on the periodic
determination and event triggering policy, the number of service drops and the
number of E-RAB setup failures may increase slightly.
The changes in all the preceding indicators vary according to the number of UEs,
UE distribution, and service type in a cell, and therefore cannot be quantified.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.17

## Function Impacts
## Function
## Name
## Function
## Switch
ReferenceDescription
DRXCellDrxPara.
DrxAlgSwitch
DRX and
## Signaling
## Control
When DRX is enabled, it will
be affected by uplink timing
control.
a
Dynamic DRXDynDrxSwitc
h option of
the
CellAlgoSwit
ch.DynDrxSw
itch
parameter
DRX and
## Signaling
## Control
The impacts of uplink timing
control on dynamic DRX are
the same as those on DRX.
## Massive
## MIMO
introduction
NoneMassive
## MIMO (FDD)
In massive MIMO scenarios,
the TaEnhancePucch option
of the TimeAlignmentTim-
er.TaEnhance parameter
cannot be selected.
SFN cellCellAlgoSwit
ch.SfnUlSchS
witch
SFNWhen Uplink Timing Based on
PUCCH is enabled, the
TaEnhancePucch option of
the TimeAlignmentTim-
er.TaEnhance parameter takes
effect by default if the
following conditions are both
met:
● SFN is enabled.
● The PucchMeasOptSwitch
option of the
CellAlgoSwitch.
PucchAlgo
Switch parameter is
selected.
Short TTISHORT_TTI_S
W option of
the
CellShortTtiA
lgo.SttiAlgoS
witch
parameter
Short TTI
## (FDD)
TA enhancement is not
applicable to UEs scheduled in
short TTI mode.
## Superior
uplink
coverage
CellAlgoExtS
witch.UlCove
rageEnhance
mentSw
## Superior
## Uplink
## Coverage
## (FDD)
TA enhancement is not
applicable to UEs under
enhanced coverage.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.18

## Function
## Name
## Function
## Switch
ReferenceDescription
a: Uplink timing control has the following impacts on DRX:
● When the TimeAlignmentTimer.TimingMeasMode parameter is set to
INVALID, DRX parameter settings are restrained by uplink timing. For details
about the restrictions, see DRX and Signaling Control. When the
TimeAlignmentTimer.TimingMeasMode parameter is set to
ALLMEASMODE, DRX parameter settings are no longer restrained by uplink
timing, which further reduces the power consumption of UEs.
● The eNodeB receives CQI on PUCCH from UEs only when the UEs are in the
DRX active time. The timing offset measurement accuracy depends on the
number of resources for reporting CQI on PUCCH. If the long DRX cycle
duration is greater than or equal to 160 ms, to ensure that the eNodeB can
measure a timing offset accurately before delivering the Timing Advance
Command, the interval for sending the Timing Advance Command must be
prolonged to enable the eNodeB to obtain sufficient resources for reporting
CQI on PUCCH. However, this decreases the supported UE moving speed.
● Scheduling request (SR) false detection will cause unnecessary uplink
scheduling, which consumes air interface resources and reduces the gains
provided by Uplink Timing Based on PUCCH. You are advised to enable
PUSCH DTX detection by selecting the PuschDtxSwitch option of the
CellAlgoSwitch.
UlSchSwitch parameter. PUSCH DTX detection helps avoid
unnecessary uplink scheduling caused by SR false detection.
● If the eNodeB does not receive a valid periodic CQI report within eight
consecutive CQI reporting periods from a UE in DRX sleep time, the eNodeB
instructs the UE to send an aperiodic CQI report in the DRX active time. The
aperiodic CQI report must be sent based on CQI_ONLY scheduling if the UE
does not have uplink data to transmit. CQI_ONLY scheduling consumes air
interface resources and reduces the gains provided by Uplink Timing Based
on PUCCH.

## 4.3 Requirements
## 4.3.1 Licenses
There are no license requirements for basic functions.
## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.19

## Mutually Exclusive Functions
## Function
## Name
## Function
## Switch
ReferenceDescription
High speed
mobility
Cell.HighSpe
edFlag
## High Speed
## Mobility
High speed mobility takes
precedence over Uplink Timing
Based on PUCCH. When high
speed mobility is enabled,
Uplink Timing Based on
PUCCH does not take effect.
Ultra high
speed
mobility
Cell.HighSpe
edFlag
## High Speed
## Mobility
Ultra high speed mobility
takes precedence over Uplink
Timing Based on PUCCH.
When ultra high speed
mobility is enabled, Uplink
Timing Based on PUCCH does
not take effect.
Extended CPCell.UlCyclicP
refix
Cell.DlCyclicP
refix
Extended CPExtended CP takes precedence
over Uplink Timing Based on
PUCCH. When extended CP is
enabled, Uplink Timing Based
on PUCCH does not take
effect.
## Static
## Multiple
## Beam
NoneMassive
## MIMO (FDD)
Static Multiple Beam cannot
work with Uplink Timing
Based on PUCCH.
## Dynamic
## Massive Beam
NoneMassive
## MIMO (FDD)
## Dynamic Massive Beam
cannot work with Uplink
Timing Based on PUCCH.
## Intelligent
beam shaping
## MM_INTELLI
## GENT_BEAM_
## SHAPING_SW
option of the
SectorSplitGr
oup.
SectorSp
litSwitch
parameter
## Massive
## MIMO (FDD)
Intelligent beam shaping
cannot work with Uplink
Timing Based on PUCCH.
The TimeAlignmentTim-
er.TimingMeasMode
parameter must be set to
INVALID for cells with
intelligent beam shaping
enabled.

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.20

## Base Station Models
●  3900 and 5900 series base stations (macro base stations)
●  DBS3900 LampSite and DBS5900 LampSite
## ●  BTS3912E
## ●  BTS3911E
## ●  BTS3203E
## ●  BTS3202E
## NO TE
BTS3202E does not support Uplink Timing Based on PUCCH and optimized accuracy of
PUCCH TA measurements.
The following base stations do not support the SPID-specific UE inactivity timer:
## ●  BTS3203E
## ●  BTS3202E
## Boards
No requirements
RF Modules
No requirements
## 4.3.4 Others
## None
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Table 4-4 and Table 4-5 describe the parameters used for function activation and
optimization, respectively.
Table 4-4 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
## Timing
## Measurement
## Mode
TimeAlignme
ntTimer.Timi
ngMeasMode
NoneSet this parameter to
ALLMEASMODE if Uplink
Timing Based on PUCCH is
required.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.21

## Parameter
## Name
Parameter IDOptionSetting Notes
Uplink timing
advance
command
optimization
switch
TimeAlignme
ntTimer.Timi
ngAdvCmdO
ptSwitch
NoneSet this parameter to ON for
common cells and OFF for
high-speed or ultra-high-
speed cells.
## TA
## Enhancement
TimeAlignme
ntTimer.TaEn
hance
TaEnhancePuc
ch
You are advised to select this
option to further improve the
accuracy of PUCCH TA
measurements when the
eNodeB measures the timing
offset based on CQI on
## PUCCH.
TimeAlignme
ntTimer.TaEn
hance
TaEnhancePus
chDmrs
You are advised to select this
option to further reduce the
DMRS for PUSCH resources
allocated by the eNodeB to
UEs when the
TimeAlignmentTim-
er.
TimingResOptSwitch
parameter is set to ON.
## Timing
## Resource
## Optimization
## Switch
TimeAlignme
ntTimer.Timi
ngResOptSwi
tch
NoneYou are advised to set this
parameter to ON to reduce
the resources consumed by
timing offset measurements
based on DMRS for PUSCH.

Table 4-5 Parameters used for optimization
## Parameter Name
Parameter IDSetting Notes
TA Command Sending
## Period
TimeAlignmentTim-
er.TACmdSendPeriod
Set this parameter based on
the network plan.
Uplink time alignment
timer
TimeAlignmentTim-
er.TimeAlignmentTi
mer
Set this parameter based on
the network plan.
## Uplink
## Synchronization Timer
for QCI
QciPara.UlSynTimerF
orQci
Set this parameter based on
the network plan.
UE Inactive Timer for
## QCI
QciPara.UeInactiveTi
merForQci
Set this parameter based on
the network plan.
SPID-Specific UE
## Inactivity Timer
SpidCfg.SpidUeInacti
vityTimer
Set this parameter based on
the network plan.

eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.22

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
//Enabling Uplink Timing Based on PUCCH
MOD TATIMER: LocalCellId=0, TimingMeasMode=ALLMEASMODE;
//Enabling the Timing Advance Command to be delivered based on the periodic determination and event
triggering policy
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF10240, TimingAdvCmdOptSwitch=ON,
TACmdSendPeriod=SF928, TimingMeasMode=ALLMEASMODE;
//Selecting the TaEnhancePucch option
MOD TATIMER: LocalCellId=0, TaEnhance=TaEnhancePucch-1;
//Selecting the TaEnhancePuschDmrs option when the TimingResOptSwitch parameter is set to ON
MOD TATIMER: LocalCellId=0, TimingResOptSwitch=ON, TaEnhance=TaEnhancePuschDmrs-1;
## Optimization Command Examples
●Configuring the TimeAlignmentTimer, TimingAdvCmdOptSwitch,
TACmdSendPeriod, and TimingMeasMode parameters
–   Scenario 1: Configuring the TimeAlignmentTimer,
TimingAdvCmdOptSwitch, TACmdSendPeriod, and TimingMeasMode
parameters when DRX is disabled or when DRX is enabled and the long
DRX cycle is less than 160 ms
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF10240, TimingAdvCmdOptSwitch=ON,
TACmdSendPeriod=SF928, TimingMeasMode=ALLMEASMODE;
–   Scenario 2: Configuring the TimeAlignmentTimer,
TimingAdvCmdOptSwitch, TACmdSendPeriod, and TimingMeasMode
parameters when DRX is enabled and the long DRX cycle is greater than
or equal to 160 ms
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF10240, TimingAdvCmdOptSwitch=ON,
TACmdSendPeriod=SF5088, TimingMeasMode=ALLMEASMODE;
●Configuring timers
//Configuring the UlSynTimerForQci parameter
MOD QCIPARA: Qci=9, UlSynTimerForQci=180;
//Configuring the UeInactiveTimerForQci parameter
MOD QCIPARA: Qci=9, UeInactiveTimerForQci=20;
//Configuring the SpidUeInactivityTimer parameter
MOD SPIDCFG: Spid=1, SpidUeInactivityTimer=20;
## Deactivation Command Examples
The following provides only deactivation command examples. You can determine
whether to restore the settings of other parameters based on actual network
conditions.
//Deselecting the TaEnhancePucch option
MOD TATIMER: LocalCellId=0, TaEnhance=TaEnhancePucch-0;
//Deselecting the TaEnhancePuschDmrs option
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.23

MOD TATIMER: LocalCellId=0, TimingResOptSwitch=OFF, TaEnhance=TaEnhancePuschDmrs-0;
//Disabling Uplink Timing Based on PUCCH
●  Scenario 1: Configuring the following parameters when DRX is disabled or
when DRX is enabled and the long DRX cycle is less than 160 ms
//Setting the TimeAlignmentTimer parameter to SF1920 and disabling Uplink Timing Based on
PUCCH when TimeAlignmentTimer.TimingAdvCmdOptSwitch is set to OFF
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF1920, TimingMeasMode=INVALID;
//Setting the TimeAlignmentTimer parameter to SF10240 and disabling Uplink Timing Based on
PUCCH when TimeAlignmentTimer.TimingAdvCmdOptSwitch is set to ON
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF10240, TimingMeasMode=INVALID;
●  Scenario 2: Setting the TimeAlignmentTimer parameter to SF10240, turning
off the TimingAdvCmdOptSwitch, and disabling Uplink Timing Based on
PUCCH when DRX is enabled and the long DRX cycle is greater than or equal
to 160 ms
MOD TATIMER: LocalCellId=0, TimeAlignmentTimer=SF10240, TimingAdvCmdOptSwitch=OFF,
TimingMeasMode=INVALID;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
Uplink timing control is a basic function that ensures basic service performance. It
takes effect by default and does not require separate activation verification.
To verify that Uplink Timing Based on PUCCH has been activated, perform the
following steps:
Step 1Run the LST TATIMER command.
When the TimingMeasMode parameter value is ALLMEASMODE in the
command output, you can preliminarily determine that Uplink Timing Based on
PUCCH has taken effect.
Step 2Check the counters listed in Table 4-6.
If the value of any counter is greater than 0, Uplink Timing Based on PUCCH has
taken effect in the cell.
Table 4-6 Counters used to verify activation of Uplink Timing Based on PUCCH
Counter ID
## Counter Name
1526730143L.Traffic.User.TAMeas.PUCCH.Avg
1526730144L.Traffic.User.TAMeas.PUCCH.Max

----End
## 4.4.3 Network Monitoring
Uplink timing control ensures basic network performance and does not require
separate monitoring.
After Uplink Timing Based on PUCCH is enabled, its benefits and impacts can be
monitored based on the indicators described in 4.2 Network Analysis. The
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.24

operation of Uplink Timing Based on PUCCH can be monitored based on the
counters listed in Table 4-7.
Table 4-7 Counters used to monitor performance of Uplink Timing Based on
## PUCCH
Counter IDCounter Name
1526730143L.Traffic.User.TAMeas.PUCCH.Avg
1526730144L.Traffic.User.TAMeas.PUCCH.Max
1526728764L.ChMeas.PRB.PUSCH.Avg
1526728304L.ChMeas.CCE.ULUsed
1526727412 to
## 1526727443
L.ChMeas.PUSCH.MCS.0 to
L.ChMeas.PUSCH.MCS.31

After Uplink Timing Based on PUCCH is enabled, the uplink timing offsets of some
UEs in a cell are measured based on the PUCCH, which reduces air interface
resources consumed by uplink timing offset measurement based on DMRS for
PUSCH. Therefore,
●  Observe the L.Traffic.User.TAMeas.PUCCH.Avg counter to obtain the average
number of UEs whose uplink timing offsets are measured based on the
PUCCH in the cell.
●  Observe the L.Traffic.User.TAMeas.PUCCH.Max counter to obtain the
maximum number of UEs whose uplink timing offsets are measured based on
the PUCCH in the cell.
●  Observe the L.ChMeas.PRB.PUSCH.Avg counter to learn that the number of
used PUSCH PRBs decreases.
●  Observe the L.ChMeas.CCE.ULUsed counter to learn that the number of
PDCCH CCEs used for downlink control information (DCI) containing uplink
scheduling information decreases.
●  Observe counters L.ChMeas.PUSCH.MCS.0 to L.ChMeas.PUSCH.MCS.31 to
learn that the number of scheduling times on the PUSCH decreases. The
number of scheduling times on the PUSCH is equal to the total number of
times each MCS index is selected for scheduling on the PUSCH.
●  Observe the L.ChMeas.PUSCH.DmrsTaSch counter to learn that the number
of DMRS TA scheduling times on the PUSCH decreases.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description4 Uplink Timing Control
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.25

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
Uplink Timing Control (FDD) Feature Parameter
## Description5 Parameters
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.26

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
Uplink Timing Control (FDD) Feature Parameter
## Description6 Counters
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.27

## 7 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description7 Glossary
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.28

## 8 Reference Documents
●  3GPP TS 36.213: "Evolved Universal Terrestrial Radio Access (E-UTRA);
Physical layer procedures"
## ●
DRX and Signaling Control
●Random Access Control
## ●SFN
●Massive MIMO (FDD)
●Short TTI (FDD)
●High Speed Mobility
●Extended CP
●Superior Uplink Coverage (FDD)
eRAN
Uplink Timing Control (FDD) Feature Parameter
## Description8 Reference Documents
Issue 06 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.29