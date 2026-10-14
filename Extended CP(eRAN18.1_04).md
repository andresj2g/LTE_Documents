

eRAN
Extended CP Feature Parameter
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
1.2 eRAN18.1 03 (2023-02-01)..................................................................................................................................................1
1.3 eRAN18.1 02 (2022-10-25)..................................................................................................................................................2
1.4 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.5 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 2
2 About This Document.............................................................................................................3
2.1 General Statements................................................................................................................................................................ 3
2.2 Applicable RAT......................................................................................................................................................................... 3
2.3 Features in This Document.................................................................................................................................................. 4
3 General Principles....................................................................................................................5
4 Normal CP.................................................................................................................................7
4.1 Principles.................................................................................................................................................................................... 7
4.2 Network Analysis.....................................................................................................................................................................7
4.2.1 Benefits....................................................................................................................................................................................7
4.2.2 Impacts.................................................................................................................................................................................... 8
4.3 Requirements............................................................................................................................................................................8
4.3.1 Licenses................................................................................................................................................................................... 8
4.3.2 Software.................................................................................................................................................................................. 8
4.3.3 Hardware................................................................................................................................................................................ 8
4.3.4 Others...................................................................................................................................................................................... 9
4.4 Operation and Maintenance............................................................................................................................................... 9
4.4.1 Data Configuration..............................................................................................................................................................9
4.4.1.1 Data Preparation.............................................................................................................................................................. 9
4.4.1.2 Using MML Commands..................................................................................................................................................9
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 10
4.4.2 Activation Verification......................................................................................................................................................10
4.4.3 Network Monitoring.........................................................................................................................................................10
5 Extended CP............................................................................................................................11
5.1 Principles.................................................................................................................................................................................. 11
5.2 Network Analysis.................................................................................................................................................................. 11
5.2.1 Benefits................................................................................................................................................................................. 11
eRAN
Extended CP Feature Parameter DescriptionContents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iii

5.2.2 Impacts..................................................................................................................................................................................12
5.3 Requirements......................................................................................................................................................................... 14
5.3.1 Licenses................................................................................................................................................................................. 14
5.3.2 Software................................................................................................................................................................................14
5.3.3 Hardware..............................................................................................................................................................................19
5.3.4 Others....................................................................................................................................................................................19
5.4 Operation and Maintenance.............................................................................................................................................19
5.4.1 Data Configuration........................................................................................................................................................... 19
5.4.1.1 Data Preparation............................................................................................................................................................ 20
5.4.1.2 Using MML Commands............................................................................................................................................... 20
5.4.1.3 Using the MAE-Deployment (FDD).........................................................................................................................20
5.4.1.4 Using the MAE-Deployment (TDD).........................................................................................................................21
5.4.2 Activation Verification......................................................................................................................................................21
5.4.3 Network Monitoring.........................................................................................................................................................21
6 Parameters..............................................................................................................................22
7 Counters.................................................................................................................................. 23
8 Glossary................................................................................................................................... 24
9 Reference Documents...........................................................................................................25
eRAN
Extended CP Feature Parameter DescriptionContents
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
Added descriptions of the mutually exclusive relationship between extended CP
and downlink-only module channel calibration. For details, see 5.3.2 Software.
Revised descriptions in this document.
1.2 eRAN18.1 03 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
Extended CP Feature Parameter Description1 Change History
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.1

1.3 eRAN18.1 02 (2022-10-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 01 (2022-03-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 03 (2021-06-26).
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
Extended CP Feature Parameter Description1 Change History
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
2.2 Applicable RAT
This document applies to FDD.
eRAN
Extended CP Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.3

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-001004CP length4 Normal CP
LBFD-00100401Normal CP4 Normal CP
LOFD-001031Extended CP5 Extended CP
eRAN
Extended CP Feature Parameter Description2 About This Document
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.4

## 3 General Principles
## Principles
A cyclic prefix (CP) is a copy of the end of an orthogonal frequency division
multiplexing (OFDM) symbol inserted at the beginning. Each CP serves as a guard
interval between OFDM symbols, as shown in Figure 3-1.
Figure 3-1 Structure of an OFDM symbol in the time domain
Radio signals are transmitted between an eNodeB and a UE through multiple
propagation paths. The maximum transmission delay difference between paths is
the delay spread. In typical eNodeB deployment scenarios (for example, urban
areas), the delay spread is generally short. However, in some areas with special
channel environments (for example, valleys) or special network topologies (for
example, roads covered with several RRUs serving one cell), the delay spread is
long. In addition, the delay spread increases with the cell radius.
To mitigate intersymbol interference (ISI) and inter-carrier interference (ICI)
caused by delay spread in the OFDM system, the CP technique is introduced.
The symbol energy that can be captured by an OFDM receiver depends on the CP
length:
●  If the CP length is longer than the multipath delay spread of an OFDM
symbol, the OFDM receiver can capture all the energy of the symbol.
●  If the CP length is shorter than the multipath delay spread of an OFDM
symbol, the OFDM receiver can capture only some energy of the symbol.
If the multipath components of an OFDM symbol whose multipath delay spread is
longer than the CP are incorrectly received as a subsequent OFDM symbol,
interference is generated to the actual subsequent OFDM symbol. This causes ISI.
If the interfered OFDM symbol then mistakenly captures some multipath
components of adjacent symbols, the orthogonality between subcarriers is lost
eRAN
Extended CP Feature Parameter Description3 General Principles
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.5

after fast Fourier transform (FFT). This causes ICI. To avoid ISI and ICI, a
sufficiently long CP is required. However, an unnecessarily long CP must be
avoided because it causes high system overhead and a loss of spectral efficiency.
To balance system performance, system overhead, and data transmission
capability, normal CP and extended CP were defined in section 5.6 "SC-FDMA
baseband signal generation" and section 6.12 "OFDM baseband signal generation"
of 3GPP TS 36.211 V8.9.0 for non-RACH channels to meet different multipath
delay spread requirements.
## Related Parameters
Normal CP and extended CP are specified by Cell.
UlCyclicPrefix and
## Cell.
DlCyclicPrefix.
eRAN
Extended CP Feature Parameter Description3 General Principles
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.6

4 Normal CP
## 4.1 Principles
Normal CP is a basic feature and is enabled by default. It applies to scenarios
where the delay spread is short.
Figure 4-1 shows the structure of a timeslot in the normal CP case. The timeslot
consists of seven downlink OFDM symbols or uplink single-carrier frequency
division multiple access (SC-FDMA) symbols. The CP length of symbol 0 is
approximately 5.2 μs, and the CP lengths of the other six symbols are
approximately 4.7 μs.
Figure 4-1 Structure of a timeslot in the normal CP case (with a subcarrier
spacing of 15 kHz)
The system overhead for the normal CP case shown in Figure 4-1 is calculated
using the following formula:
## 4.2 Network Analysis
## 4.2.1 Benefits
The CP technique mitigates inter-symbol interference (ISI) and inter-carrier
interference (ICI) caused by multipath delay, ensuring network coverage in E-
UTRAN cells.
eRAN
Extended CP Feature Parameter Description4 Normal CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.7

## 4.2.2 Impacts
## Network Impacts
## None
## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDNoneNoneNoneNone

## 4.3 Requirements
## 4.3.1 Licenses
There are no license requirements for basic functions.
## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
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
No requirements
## Boards
No requirements
RF Modules
No requirements
eRAN
Extended CP Feature Parameter Description4 Normal CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.8

## Cells
## None
## 4.3.4 Others
## None
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Table 4-1 describes the parameters used for function activation. This section does
not describe parameters related to cell establishment.
## NO TICE
At the moment when the CP modification takes effect in an activated cell, services
carried by UEs are interrupted in the cell. The duration for the UEs to reacquire
synchronization with the cell depends on the synchronization performance of the
UEs.
Table 4-1 Parameters used for activation
## Parameter
## Name
Parameter IDSetting Notes
Uplink cyclic
prefix length
Cell.UlCyclicP
refix
● Set the parameters to NORMAL_CP when
multipath delay spread is shorter than 4.7
μs.
● The settings of Cell.UlCyclicPrefix and
Cell.DlCyclicPrefix of a cell can be different
or not.
● The setting of Cell.
UlCyclicPrefix or
Cell.DlCyclicPrefix of a cell must be the
same as that of the other cells established
on the same BBP.
## Downlink
cyclic prefix
length
Cell.DlCyclicP
refix

4.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
eRAN
Extended CP Feature Parameter Description4 Normal CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.9

//Activating normal CP
MOD CELL: LocalCellId=0, UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP;
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
Step 1On the MAE, run the LST CELL command and check the values of Uplink cyclic
prefix length and Downlink cyclic prefix length.
●  If the values are Normal, normal CP has been configured.
●  If the values are Extended, extended CP has been configured.
Step 2On the MAE, start Uu interface tracing, deactivate the cell, and then reactivate it.
Wait until the cell is successfully activated, and then check the value of the
information element (IE) ul-CyclicPrefixLength in the first RRC_SYS_INFO message
(a SIB2 message) over the Uu interface.
●  If its value is len1(0), normal CP is working in the uplink.
●  If its value is len2(1), extended CP is working in the uplink.
## NO TE
CP configuration in the downlink is transparent to UEs. Therefore, there are no messages to
check for the downlink.
----End
## 4.4.3 Network Monitoring
## None
eRAN
Extended CP Feature Parameter Description4 Normal CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.10

5 Extended CP
## 5.1 Principles
Extended CP applies to scenarios where the delay spread is long. When multipath
interference is severe, system performance deteriorates significantly if the
multipath delay spread is longer than a normal CP. In an OFDM system, extended
CP enhances multipath delay spread resistance in large-cell-radius scenarios and
multipath interference resistance. However, extended CP increases the system
overhead and consumes certain number of transport resources.
Figure 5-1 shows the structure of a timeslot in the extended CP case. The timeslot
consists of six downlink OFDM symbols or uplink SC-FDMA symbols. The CP
length of each symbol is approximately 16.7 μs.
Figure 5-1 Structure of a timeslot in the extended CP case (with a subcarrier
spacing of 15 kHz)
As shown in Figure 5-1, an extended CP is longer than a normal CP. The
permissible multipath delay at the receiving end increases with the CP length. The
use of extended CP, however, causes more system overhead than the use of
normal CP. The system overhead for the extended CP case is calculated using the
following formula:
## 5.2 Network Analysis
## 5.2.1 Benefits
The CP technique mitigates ISI and ICI caused by multipath delay, ensuring
network coverage in E-UTRAN cells.
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.11

The deployment suggestions of extended CP are as follows:
●  It is recommended that extended CP be activated to improve uplink and
downlink signal to interference plus noise ratios (SINRs) if the multipath delay
spread exceeds the normal CP length of 4.7 μs in the area (the time
difference is greater than the length of a normal CP, 4.7 μs), for example,
where there are high buildings or mountains in the distance that will reflect
signals. This condition can be interpreted as follows: There is at least 1.5 km
difference between the line of sight (LOS) path of a signal arriving at a UE
and the reflected path of the same signal last arriving at the UE.
●  It is difficult to obtain the actual multipath delay spread. To evaluate whether
to use extended CP, operators can estimate whether the multipath delay
spread is longer than the normal CP length based on the building distribution
and landform.
●  UEs may not support extended CP. Enabling this function may cause
exceptions of such UEs. It is not recommended that this function be enabled if
there are such UEs on the live network. The extended CP capability of UEs
depends on UEs themselves.
## NO TE
This capability cannot be identified through UE capability information. If a UE can
access a cell with extended CP enabled and the UE data rate can reach its peak value,
this indicates that the UE supports extended CP.
## 5.2.2 Impacts
## Network Impacts
The use of extended CP causes more system overhead than the use of normal CP
and therefore system capacity decreases.
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.12

## Function Impacts
RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDynamic
TDM eICIC
CellAlgoS
witch.Eicic
## Switch
being set
to
## DYNAMIC
TDM eICIC (FDD)To use enhanced
inter-cell
interference
coordination
(eICIC), operators
need to enable this
function in both
macro and micro
cells. Extended CP is
applicable only to
macro eNodeBs. If
extended CP is
enabled only in
cells served by
macro eNodeBs,
optimal
performance of
eICIC cannot be
assured.
FDDUL 64QAMPUSCHCfg
.Qam64En
abled
being set
to
## BOOLEAN
## _TRUE
Modulation SchemesIn extended CP
scenarios, UL
64QAM does not
take effect.
FDDPAMCUlPAMCS
witch
option of
the
CellAlgoS
witch.
UlSc
hExtSwitc
h
parameter
SchedulingIn extended CP
scenarios, PAMC
does not take
effect.
## FDDUL 256QAMUL_256QA
## M_SWITC
H option
of the
PUSCHCfg
## .
Ul256Qa
mAlgoSwi
tch
parameter
Modulation SchemesExtended CP takes
precedence over UL
## 256QAM.

eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.13

## 5.3 Requirements
## 5.3.1 Licenses
RATFeature IDFeature
## Name
ModelSales Unit
FDDLOFD-001031Extended CPLT1S000ECP0
## 0
per RRC
## Connected
## User

## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## RAT
## Function
## Name
## Function
## Switch
ReferenceDescription
FDDUplink joint
interference
managemen
t (FDD)
## UL_JOINT
## _INTRF_S
## UPPRESS_
SW option
of the
UlInterfSu
ppressCfg.
UlJointInt
rfManage
mentSw
parameter
## Interference
Detection and
## Suppression
## None
## FDDCPRI
compression
Cell.CPRIC
ompressio
n
CPRI CompressionNone
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.14

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDSFN cellCellAlgoS
witch.Sfn
UlSchSwit
ch
CellAlgoS
witch.
## Sfn
DlSchSwit
ch
SFNThe application
scenarios are
different. Extended
CP applies to the
extended coverage
scenario, while
single frequency
network (SFN)
applies to scenarios
such as indoor
coverage, indoor
and outdoor joint
coverage, densely
populated urban
areas with short
inter-site distances,
and high-speed
railways.
FDDIn-band
relay
InBandRel
ayDeNbS
witch and
InBandRel
ayReNbS
witch
options of
the
CellAlgoS
witch.
## Rela
ySwitch
parameter
RelayNone
FDDSuper
combined
cell
SuperCom
bCellSwit
ch option
of the
CellAlgoS
witch.
## Sfn
AlgoSwitc
h
parameter
## Super Combined Cell
## (FDD)
## None
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.15

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDL CoMP
cell
FDDHom
NetDlCom
pSwitch
and
FDDHetN
etDlComp
## Switch
options of
the
CellAlgoS
witch.
DlC
ompSwitc
h
parameter
DL CoMP (FDD)Downlink (DL)
coordinated
multipoint
transmission/
reception (CoMP)
does not support
extended cell range
scenarios because
DL CoMP UEs must
receive data from
different cells.
Extended CP is
usually deployed in
extended cell range
scenarios.
Therefore, extended
CP is not supported
when DL CoMP is
enabled.
FDDLTE in-band
deployment
Prb.Deplo
yMode
NB-IoT
Enhancements (FDD)
In the current
version, both the
NB-IoT cell and the
corresponding LTE
FDD cell do not
support extended
CP in LTE in-band
deployment.
FDDMassive
## MIMO
introduction
## Massive
## MIMO
works in
multiple
scenarios.
## Its
function
switch
varies
depending
on
scenarios.
For details,
see
## Massive
## MIMO
## (FDD)
## .
Massive MIMO
## (FDD)
## None
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.16

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDIntelligent
beam
shaping
## MM_INTE
## LLIGENT_
## BEAM_SH
## APING_S
W option
of the
SectorSpli
tGroup.
## Se
ctorSplitS
witch
parameter
Massive MIMO
## (FDD)
## None
FDDWTTx MU-
## MIMO
Tm9FourL
ayerPairS
witch
option of
the
CellAlgoE
xtSwitch.
WttxMuM
imoSwitc
h
parameter
WTTx MU-MIMO
## (FDD)
## None
FDDDynamic
## Massive
## Beam
NoneSmart 8T8R (FDD)When Dynamic
Massive Beam is
used, set
Cell.UlCyclicPrefix
and
## Cell.
DlCyclicPrefix
to NORMAL_CP.
## FDDCRS
dynamic
muting
## CRS_DYN
## AMIC_MU
## TING_SW
option of
the
SymbolPw
rSaving.
## Sy
mbolShut
downEnh
ancedSw
parameter
## Energy Conservation
and Emission
## Reduction
CRS dynamic
muting is not
supported in
extended CP
scenarios.
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.17

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDRF channel
dynamic
muting
## RF_CHN_
## DYN_MUT
## ING_SW
option of
the
CellRfChn
DynMutin
g.
RfChnD
ynMuting
AlgoSwitc
h
parameter
## Energy Conservation
and Emission
## Reduction
## None
FDDDynamic
carrier
shutdown
## CARRIER_
## DYN_SHU
## TDOWN_S
W option
of the
CellShutd
own.
## Carri
erShutdo
wnEnhanc
edSw
parameter
## Energy Conservation
and Emission
## Reduction
Dynamic carrier
shutdown is not
supported in
extended CP
scenarios.
FDDStatic
## Multiple
## Beam
SectorSpli
tGroup.Be
amTempl
ateId set
to 0,
SectorSpli
tGroup.
## Be
amDeploy
mentMod
e
set to
## MODE_3,
and
SectorSpli
tCell.
CellB
eamIndex
set to 0 or
## 1
Smart 8T8R (FDD)When Static
Multiple Beam is
used, set
Cell.UlCyclicPrefix
and
## Cell.
DlCyclicPrefix
to NORMAL_CP.
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.18

RATFunction
## Name
## Function
## Switch
ReferenceDescription
FDDDownlink-
only module
channel
calibration
RruJointC
alParaCfg.
AauPassiv
ePortCalib
## Period
MIMOIf
RruJointCalParaCf
g.AauPassivePortC
alibPeriod is set to
a value other than
## 0,
## Cell.
UlCyclicPrefix
and
## Cell.
DlCyclicPrefix
must be set to
## NORMAL_CP.

## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
3900 and 5900 series base stations (macro base stations) are compatible with this
function.
## Boards
In FDD, the following BBP models do not support extended CP:
●  UBBPex2
RF Modules
In FDD: The AAU, pRRU, and book RRU do not support extended CP.
## Cells
The cell bandwidth must be greater than 5 MHz.
## 5.3.4 Others
UEs must support extended CP.
5.4 Operation and Maintenance
## 5.4.1 Data Configuration
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.19

## 5.4.1.1 Data Preparation
Table 5-1 describes the parameters used for function activation. This section does
not describe parameters related to cell establishment.
## NO TICE
At the moment when the CP modification takes effect in an activated cell, services
carried by UEs are interrupted in the cell. The duration for the UEs to reacquire
synchronization with the cell depends on the synchronization performance of the
UEs.
Table 5-1 Parameters used for activation
## Parameter
## Name
Parameter IDSetting Notes
Uplink cyclic
prefix length
Cell.UlCyclicP
refix
● Set the parameters to EXTENDED_CP when
multipath delay spread is longer than 4.7
μs.
● The settings of Cell.UlCyclicPrefix and
## Cell.
DlCyclicPrefix of a cell can be different
or not.
● The setting of Cell.
UlCyclicPrefix or
Cell.DlCyclicPrefix of a cell must be the
same as that of the other cells established
on the same BBP.
## Downlink
cyclic prefix
length
Cell.DlCyclicP
refix

5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Activating extended CP
MOD CELL: LocalCellId=0, UlCyclicPrefix=EXTENDED_CP, DlCyclicPrefix=EXTENDED_CP;
## Deactivation Command Examples
//Deactivating extended CP
MOD CELL: LocalCellId=0, UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP;
5.4.1.3 Using the MAE-Deployment (FDD)
●  Fast batch activation
This function can be batch activated using the Feature Operation and
Maintenance function of the MAE-Deployment. For detailed operations, see
the following section in the MAE-Deployment product documentation or
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.20

online help: MAE-Deployment Operation and Maintenance > MAE-
## Deployment Guidelines > Enhanced Feature Management > Feature
Operation and Maintenance.
●  Single/Batch configuration
This function can be activated for a single base station or a batch of base
stations on the MAE-Deployment. For detailed operations, see Feature
Configuration Using the MAE-Deployment.
5.4.1.4 Using the MAE-Deployment (TDD)
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
For details, see 4.4.2 Activation Verification.
## 5.4.3 Network Monitoring
## None
eRAN
Extended CP Feature Parameter Description5 Extended CP
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.21

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
Extended CP Feature Parameter Description6 Parameters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.22

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
Extended CP Feature Parameter Description7 Counters
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.23

## 8 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
Extended CP Feature Parameter Description8 Glossary
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.24

## 9 Reference Documents
-  3GPP TS 36.211 V8.9.0, "SC-FDMA baseband signal generation"
-  3GPP TS 36.211 V8.9.0, "OFDM baseband signal generation"
## 3.
CPRI Compression
4.DL CoMP (FDD)
5.Massive MIMO (FDD)
6.WTTx MU-MIMO (FDD)
7.NB-IoT Enhancements (FDD)
8.Relay
## 9.SFN
10.Smart 8T8R (FDD)
11.Super Combined Cell (FDD)
12.Scheduling
13.Modulation Schemes
14.Interference Detection and Suppression
15.Energy Conservation and Emission Reduction
16.TDM eICIC (FDD)
17.Physical Channel Resource Management
eRAN
Extended CP Feature Parameter Description9 Reference Documents
Issue 04 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.25