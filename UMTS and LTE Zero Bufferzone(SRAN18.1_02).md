

SingleRAN
UMTS and LTE Zero Bufferzone
## Feature Parameter Description
## Issue02
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
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 SRAN18.1 02 (2024-06-21)..................................................................................................................................................1
1.2 SRAN18.1 01 (2022-03-08)..................................................................................................................................................1
1.3 SRAN18.1 Draft B (2022-02-08)........................................................................................................................................ 1
1.4 SRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 2
2 About This Document.............................................................................................................3
2.1 General Statements................................................................................................................................................................ 3
2.2 Applicable RAT......................................................................................................................................................................... 3
2.3 Features in This Document.................................................................................................................................................. 4
3 Overview....................................................................................................................................5
3.1 Background................................................................................................................................................................................5
3.2 Definition....................................................................................................................................................................................5
3.3 Introduction...............................................................................................................................................................................7
3.4 Typical Configuration............................................................................................................................................................. 9
4 UMTS and LTE Zero Bufferzone (UMTS)..........................................................................16
4.1 Principles.................................................................................................................................................................................. 16
4.2 Network Analysis.................................................................................................................................................................. 17
4.2.1 Benefits................................................................................................................................................................................. 18
4.2.2 Impacts..................................................................................................................................................................................19
4.3 Requirements......................................................................................................................................................................... 27
4.3.1 Licenses................................................................................................................................................................................. 28
4.3.2 Software................................................................................................................................................................................28
4.3.3 Hardware..............................................................................................................................................................................30
4.3.4 Networking.......................................................................................................................................................................... 32
4.3.5 Others....................................................................................................................................................................................32
4.4 Operation and Maintenance.............................................................................................................................................32
4.4.1 When to Use....................................................................................................................................................................... 32
4.4.2 Precautions.......................................................................................................................................................................... 33
4.4.3 Data Configuration........................................................................................................................................................... 34
4.4.3.1 Data Preparation............................................................................................................................................................ 34
4.4.3.2 Using MML Commands............................................................................................................................................... 34
4.4.3.3 Using the MAE-Deployment...................................................................................................................................... 35
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
DescriptionContents
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iii

4.4.4 Activation Verification......................................................................................................................................................35
4.4.5 Network Monitoring.........................................................................................................................................................35
5 UMTS and LTE Zero Bufferzone (LTE FDD)......................................................................37
5.1 Principles.................................................................................................................................................................................. 37
5.2 Network Analysis.................................................................................................................................................................. 40
5.2.1 Benefits................................................................................................................................................................................. 40
5.2.2 Impacts..................................................................................................................................................................................42
5.3 Requirements......................................................................................................................................................................... 50
5.3.1 Licenses................................................................................................................................................................................. 50
5.3.2 Software................................................................................................................................................................................50
5.3.3 Hardware..............................................................................................................................................................................52
5.3.4 Networking.......................................................................................................................................................................... 53
5.3.5 Others....................................................................................................................................................................................53
5.4 Operation and Maintenance.............................................................................................................................................53
5.4.1 When to Use....................................................................................................................................................................... 53
5.4.2 Precautions.......................................................................................................................................................................... 53
5.4.3 Data Configuration........................................................................................................................................................... 53
5.4.3.1 Data Preparation............................................................................................................................................................ 53
5.4.3.2 Using MML Commands............................................................................................................................................... 56
5.4.3.3 Using the MAE-Deployment...................................................................................................................................... 56
5.4.4 Activation Verification......................................................................................................................................................57
5.4.5 Network Monitoring.........................................................................................................................................................57
6 Parameters..............................................................................................................................59
7 Counters.................................................................................................................................. 60
8 Glossary................................................................................................................................... 61
9 Reference Documents...........................................................................................................62
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
DescriptionContents
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
## 1.1 SRAN18.1 02 (2024-06-21)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in the document.
## 1.2 SRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.3 SRAN18.1 Draft B (2022-02-08)
This issue includes the following changes.
## Technical Changes
## None
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description1 Change History
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.1

## Editorial Changes
Added the impact relationship with Physical Resource Slicing. For details, see 5.2.2
## Impacts.
1.4 SRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to SRAN17.1 04 (2021-11-27).
## Technical Changes
Change DescriptionParameter
## Change
## Base Station
## Model
Added the mutually exclusive
relationship between UMTS and LTE
Zero Bufferzone (UMTS) and UMTS
Smart 8T Beam. For details, see 4.3.2
## Software.
None3900 and 5900
series base
stations
Deleted the LMPT from this document
because the LMPT has reached its end
of service (EOS) phase.
None3900 and 5900
series base
stations

## Editorial Changes
Revised descriptions in the document.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description1 Change History
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.2

## 2 About This Document
## 2.1 General Statements
## Purpose
Feature Parameter Description documents are intended to acquaint readers with:
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
Any parameters, alarms, counters, or managed objects (MOs) described in Feature
Parameter Description documents apply only to the corresponding software
release. For future software releases, refer to the corresponding updated product
documentation.
2.2 Applicable RAT
This document applies to UMTS and LTE FDD.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description2 About This Document
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.3

2.3 Features in This Document
This document describes the following features.
RATFeature IDFeature NameChapter/Section
UMTSMRFD-150211UMTS and LTE Zero
Bufferzone (UMTS)
4 UMTS and LTE Zero
Bufferzone (UMTS)
## LTE
## FDD
MRFD-150221UMTS and LTE Zero
Bufferzone (LTE FDD)
5 UMTS and LTE Zero
Bufferzone (LTE
## FDD)
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description2 About This Document
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.4

## 3 Overview
## 3.1 Background
Operators have growing demands for faster deployment or more capacity for LTE
networks because data services are growing more popular and the penetration
rate of smart terminals is increasing. The UMTS spectrum is released and refarmed
for LTE deployment.
After UMTS spectrum is refarmed for LTE deployment, co-channel interference
exists between UMTS and LTE networks operating on the same frequency band.
Severe interference may decrease the throughput, increase the service drop rate,
and cause service initiation failures. Therefore, a buffer zone is required to
geographically isolate refarming areas and non-refarming areas to avoid impact of
co-channel interference on UMTS and LTE network performance. However, the
spectrum in the buffer zone cannot be used for UMTS or LTE network deployment,
resulting in a waste of spectrum resources.
## 3.2 Definition
This feature allows for the deployment of UMTS and LTE networks on the same
frequency in adjacent areas in the buffer zone. It helps make full use of spectrum
resources in the buffer zone. As shown in Figure 3-1, the spectrum in the buffer
zone can be used by UMTS and LTE networks. Compared with the performance of
standard bandwidths of a single UMTS or LTE mode, performance in the buffer
zone deteriorates to a certain extent due to interference.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.5

Figure 3-1 Principles of UMTS and LTE zero buffer zone
The spectrum in the buffer zone is classified into different types. Figure 3-2 shows
the classification.
●  UMTS-dedicated spectrum: UMTS-dedicated spectrum in available spectrum
resources for UMTS does not overlap LTE spectrum.
●  LTE-dedicated spectrum: LTE-dedicated spectrum in available spectrum
resources for LTE does not overlap UMTS spectrum.
●  UMTS and LTE shared spectrum (UL shared spectrum for short): UL shared
spectrum is the spectrum in the UMTS and LTE spectrum overlapping area.
The PRB range of UL shared spectrum can be determined by setting the
ULSpectrumShrConfig.
PrbRsvType parameter to
UMTS_LTE_SHARED_SPECTRUM and setting the
ULSpectrumShrConfig.
LtePrbStartIndex and
ULSpectrumShrConfig.LtePrbEndIndex parameters in an LTE cell. The
downlink spectrum in UL shared spectrum can be used by both UMTS and LTE
networks. The uplink spectrum is classified into UMTS preferential spectrum
and UMTS non-preferential spectrum.
–   UMTS preferential spectrum: The spectrum bandwidth used for
measuring the received total wideband power (RTWP) of a UMTS cell
within the UL shared spectrum range is termed as UMTS preferential
spectrum. Only cell center users (CCUs) in an LTE cell can use this
spectrum. The reason is to ensure the uplink capacity of UMTS cells.
Users can set the ULSpectrumShrConfig.
PrbRsvType parameter to
## UMTS_CORE_SPECTRUM_1, UMTS_CORE_SPECTRUM_2,
UMTS_CORE_SPECTRUM_3, or UMTS_CORE_SPECTRUM_4 to specify the
PRB reserving type of UMTS and LTE spectrum sharing. Then, users set
the ULSpectrumShrConfig.
LtePrbStartIndex and
ULSpectrumShrConfig.
LtePrbEndIndex parameters to specify the PRB
range of the UMTS preferential spectrum for UMTS carrier 1, UMTS
carrier 2, UMTS carrier 3, or UMTS carrier 4.
–   UMTS non-preferential spectrum: The UL shared spectrum except the
UMTS preferential spectrum is termed as non-preferential spectrum,
which can be used by both CCUs and cell edge users (CEUs) in an LTE
cell. The ULOCELL.
ULLEFTSHAREDBANDWIDTH and
ULOCELL.ULRIGHTSHAREDBANDWIDTH parameters specify the range
of PRBs on the left and right of UMTS non-preferential spectrum,
respectively.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.6

Figure 3-2 Uplink spectrum classification in the buffer zone (using one UMTS
carrier as an example)
## 3.3 Introduction
This feature mitigates the interference of UMTS and LTE networks when they are
deployed on the same frequency in adjacent areas. By fully utilizing spectrum
resources in the buffer zone, this feature improves the capacity of UMTS and LTE
cells and accelerates network evolution to a higher RAT. When UMTS and LTE cells
are deployed adjacent to each other on the same frequency, UMTS and LTE cells
and UEs experiences interferences from four directions, as shown in Figure 3-3.
Table 3-1 describes the impact of interference in each direction.
Figure 3-3 Interference among UMTS and LTE cells and UEs
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.7

Table 3-1 Interference impact analysis
DirectionInterference
## Description
ImpactIs Interference
## Processing
## Required?
aUplink
transmit of
LTE UE to
uplink receive
of NodeB
A UMTS network is a self-
interference system. Therefore,
the uplink transmit power of
UEs must be strictly controlled
to ensure the uplink cell
capacity and network
performance. When UMTS
intra-frequency cells are
adjacent, the interference of
neighboring cells can be
controlled by power control in
UMTS cells. When UMTS and
LTE intra-frequency cells are
adjacent and LTE CEUs are
close to the UMTS cell, these
UEs cause strong interference
to the UMTS cell because the
uplink transmit power of these
UEs is not controlled by the
UMTS cell.
## Yes
bDownlink
transmit (DL
TX) of NodeB
to downlink
receive (DL
RX) of LTE UE
The impact of interference in
this direction is similar to that
of DL TX signals of
neighboring LTE cells to DL RX
signals of LTE UEs. In addition,
when the power spectral
density (PSD) of the UMTS
cell is the same as that of the
LTE cell, the interference of
direction b can be ignored.
## No
cDL TX of
eNodeB to DL
RX of UMTS
## UE
The interference impact is the
same as that of direction b.
## No
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.8

DirectionInterference
## Description
ImpactIs Interference
## Processing
## Required?
dUplink
transmit of
UMTS UE to
uplink receive
of eNodeB
The uplink transmit power of
UMTS UEs is lower than that
of LTE UEs because uplink
transmit power of UMTS UEs
is strictly controlled. Therefore,
the impact of UMTS UEs on
the uplink receive signals of
the eNodeB is lower than that
brought by UEs in neighboring
LTE cells. Therefore,
interference of direction d can
be ignored.
## No

This feature provides the following solutions for interference in direction a:
●  Interference control on the UMTS side:
–   The uplink adaptive filtering automatically identifies the strength and
location of LTE uplink interference, adaptively filters out UMTS signals
affected by strong LTE interference, and improves the UMTS uplink anti-
interference capability.
–   The uplink narrowband filtering filters out the edge bandwidth on both
sides of the UMTS network, filters out UMTS signals affected by strong
LTE interference, and improves the UMTS uplink anti-interference
capability.
Either the uplink adaptive filtering or uplink narrowband filtering can be used
on the UMTS side based on the network planning. Unless otherwise specified,
both filters are applicable.
●  Uplink physical channel resource management and scheduling optimization
on the LTE side: This feature differentiates CCUs and CEUs in LTE cells. CCUs
can use UMTS preferential spectrum and non-preferential spectrum, and CEUs
can use only UMTS non-preferential spectrum. This reduces interference from
CEUs to UMTS cells.
## NO TE
This feature has no special requirements on frequency bands. This feature is supported by
850 MHz, 900 MHz, 1900 MHz, AWS, and 2100 MHz frequency bands.
## 3.4 Typical Configuration
The following spectrum resources need to be configured in the buffer zone: UMTS
left shared spectrum, UMTS right shared spectrum, UL shared spectrum, and
UMTS preferential spectrum. The scheduling priorities of resources corresponding
to different spectrum types are also different. Therefore, the configuration range
of each type of spectrum needs to be properly planned to achieve the optimal
scheduling effect. The typical configurations vary with the functions used on the
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.9

UMTS side. Unless otherwise specified, the LTE physical channel configurations
comply with those described in Physical Channel Resource Management in eRAN
## Feature Documentation.
## When Uplink Adaptive Filtering Is Used
During spectrum planning, adhere to the following principles:
●  If there is no dedicated PRB on the LTE network, to prevent interference
between the LTE PRACH/PUCCH and UMTS preferential spectrum, the UMTS
preferential spectrum must be set to 2.34 MHz to maximize the UMTS uplink
capacity gain. If there is dedicated PRB on the LTE network, the UMTS
preferential spectrum can be set to a value greater than 2.34 MHz.
●  The UMTS preferential spectrum should be configured at the center of the
UMTS bandwidth to maximize the UMTS uplink capacity gains. In addition,
sufficient number of PRBs used for configuring the LTE PRACH and PUCCH are
required for the shared spectrum on the left and the shared spectrum on the
right.
The following provides the typical configurations of each type of spectrum in the
buffer zone in different LTE bandwidth scenarios.
●  LTE bandwidth: 5 MHz (one carrier shared by UMTS)
The shared bandwidth A on the left side of the UMTS network is 1.33 MHz,
and the shared bandwidth B on the right side of the UMTS network is 1.33
MHz. The UMTS preferential spectrum range is PRB 6 to PRB 18.
Figure 3-4 5 MHz LTE bandwidth (one carrier shared by UMTS)
●  LTE bandwidth: 10 MHz (two carriers shared by UMTS)
–   The shared bandwidth A on the left side of the UMTS network 1 is 1.4
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 1.26 MHz. The UMTS 1 preferential spectrum range is PRB 5 to PRB
## 17.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1.26
MHz, and the shared bandwidth D on the right side of the UMTS network
2 is 1.4 MHz. The UMTS 2 preferential spectrum range is PRB 32 to PRB
## 44.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.10

Figure 3-5 10 MHz LTE bandwidth (two carriers shared by UMTS)
●  LTE bandwidth: 15 MHz (three carriers shared by UMTS)
–   The shared bandwidth A on the left side of the UMTS network 1 is 1.83
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 0.83 MHz. The UMTS 1 preferential spectrum range is PRB 4 to PRB
## 16.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1.33
MHz, and the shared bandwidth D on the right side of the UMTS network
2 is 1.33 MHz. The UMTS 2 preferential spectrum range is PRB 31 to PRB
## 43.
–   The shared bandwidth E on the left side of the UMTS network 3 is 0.83
MHz, and the shared bandwidth F on the right side of the UMTS network
3 is 1.83 MHz. The UMTS 3 preferential spectrum range is PRB 58 to PRB
## 70.
Figure 3-6 15 MHz LTE bandwidth (three carriers shared by UMTS)
●  LTE bandwidth: 20 MHz (four carriers shared by UMTS)
–   The shared bandwidth A on the left side of the UMTS network 1 is 2.26
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 0.4 MHz. The UMTS 1 preferential spectrum range is PRB 7 to PRB
## 19.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1.4
MHz, and the shared bandwidth D on the right side of the UMTS network
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.11

2 is 1.26 MHz. The UMTS 2 preferential spectrum range is PRB 30 to PRB
## 42.
–   The shared bandwidth E on the left side of the UMTS network 3 is 1.26
MHz, and the shared bandwidth F on the right side of the UMTS network
3 is 1.4 MHz. The UMTS 3 preferential spectrum range is PRB 57 to PRB
## 69.
–   The shared bandwidth G on the left side of the UMTS network 4 is 0.4
MHz, and the shared bandwidth H on the right side of the UMTS
network 4 is 2.26 MHz. The UMTS 4 preferential spectrum range is PRB
81 to PRB 93.
Figure 3-7 20 MHz LTE bandwidth (four carriers shared by UMTS)
## When Uplink Narrowband Filtering Is Used
The following provides the typical configurations of each type of spectrum in the
buffer zone in different LTE bandwidth scenarios.
●  LTE bandwidth: 5 MHz (one carrier shared by UMTS)
The shared bandwidth A on the left side of the UMTS network is 1.2 MHz,
and the shared bandwidth B on the right side of the UMTS network is 1.2
MHz. The UMTS preferential spectrum range is PRB 5 to PRB 19.
Figure 3-8 5 MHz LTE bandwidth (one carrier shared by UMTS)
●  LTE bandwidth: 10 MHz (two carriers shared by UMTS)
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.12

–   The shared bandwidth A on the left side of the UMTS network 1 is 0.8
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 0.8 MHz. The UMTS 1 preferential spectrum range is PRB 1 to PRB
## 20.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1.2
MHz, and the shared bandwidth D on the right side of the UMTS network
2 is 1.2 MHz. The UMTS 2 preferential spectrum range is PRB 31 to PRB
## 46.
Figure 3-9 10 MHz LTE bandwidth (two carriers shared by UMTS)
In this scenario, the PUCCH and PRACH in the LTE network must be shifted to
the center to avoid interference to the UMTS preferential spectrum. The
PUCCH range is PRB 21 to PRB 24 and PRB 25 to PRB 28. The PRACH range is
PRB 29 to PRB 34.
●  LTE bandwidth: 15 MHz (three carriers shared by UMTS)
–   The shared bandwidth A on the left side of the UMTS network 1 is 1
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 1 MHz. The UMTS 1 preferential spectrum range is PRB 1 to PRB 18.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1
MHz, and the shared bandwidth D on the right side of the UMTS network
2 is 1 MHz. The UMTS 2 preferential spectrum range is PRB 29 to PRB 45.
–   The shared bandwidth E on the left side of the UMTS network 3 is 1
MHz, and the shared bandwidth F on the right side of the UMTS network
3 is 1 MHz. The UMTS 3 preferential spectrum range is PRB 56 to PRB 73.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.13

Figure 3-10 15 MHz LTE bandwidth (three carriers shared by UMTS)
In this scenario, the PUCCH and PRACH in the LTE network must be shifted to
the center to avoid interference to the UMTS preferential spectrum. The
PUCCH range is PRB 24 to PRB 28 and PRB 46 to PRB 50. The PRACH range is
PRB 51 to PRB 56.
●  LTE bandwidth: 20 MHz (four carriers shared by UMTS)
–   The shared bandwidth A on the left side of the UMTS network 1 is 0.8
MHz, and the shared bandwidth B on the right side of the UMTS network
1 is 0.8 MHz. The UMTS 1 preferential spectrum range is PRB 0 to PRB
## 17.
–   The shared bandwidth C on the left side of the UMTS network 2 is 1.2
MHz, and the shared bandwidth D on the right side of the UMTS network
2 is 1.2 MHz. The UMTS 2 preferential spectrum range is PRB 28 to PRB
## 43.
–   The shared bandwidth E on the left side of the UMTS network 3 is 1.2
MHz, and the shared bandwidth F on the right side of the UMTS network
3 is 1.2 MHz. The UMTS 3 preferential spectrum range is PRB 56 to PRB
## 71.
–   The shared bandwidth G on the left side of the UMTS network 4 is 0.8
MHz, and the shared bandwidth H on the right side of the UMTS
network 4 is 0.8 MHz. The UMTS 4 preferential spectrum range is PRB 82
to PRB 99.
In this scenario, the PUCCH and PRACH in the LTE network must be shifted to
the center to avoid interference to the UMTS preferential spectrum. The
PUCCH range is PRB 22 to PRB 27 and PRB 72 to PRB 77. The PRACH range is
PRB 78 to PRB 83.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.14

Figure 3-11 20 MHz LTE bandwidth (four carriers shared by UMTS)
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description3 Overview
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.15

4 UMTS and LTE Zero Bufferzone (UMTS)
## 4.1 Principles
This feature is enabled when ULOCELL.
UL0BUFFERZONE is set to TRUE. The
uplink adaptive filtering or uplink narrowband filtering can be used to suppress
the interference from the LTE network to the UMTS network. Use either of the
functions based on the network planning.
## Uplink Adaptive Filtering
Uplink adaptive filtering is enabled when ULOCELL.
UL0BUFFERZONEFILTER is set
to ULADAPTIVEFILTER.
Uplink adaptive filtering dynamically detects the LTE interference strength within
the UL shared spectrum in real time and identifies the interference frequency
location and bandwidth. Then, uplink adaptive filtering adaptively adjusts the
UMTS uplink receive bandwidth to reduce the uplink interference of LTE UEs to
the UMTS cell. Figure 4-1 shows the interference processing on the UMTS side.
The principles are as follows:
-  The NodeB performs spectrum scanning within the 5 MHz UMTS bandwidth
and uses the uplink receive signals within the UMTS preferential bandwidth as
the reference signals. The start frequency of the UMTS preferential spectrum
is calculated using the following formula: Cell center frequency – 2.5 MHz +
## ULOCELL.
ULLEFTSHAREDBANDWIDTH parameter value. The end frequency
of the UMTS preferential spectrum is calculated using the following formula:
Cell center frequency + 2.5 MHz – ULOCELL.ULRIGHTSHAREDBANDWIDTH
parameter value.
-  The NodeB compares the uplink receive signal strength within the UMTS non-
preferential spectrum and UMTS preferential spectrum within the UL shared
spectrum to identify the strong LTE interference and the PRB position and
range corresponding to the interference.
-  The NodeB automatically filters the UE signals and interference signals of LTE
in the position with strong interference.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.16

Figure 4-1 Uplink adaptive filtering
## Uplink Narrowband Filtering
Uplink narrowband filtering is enabled when ULOCELL.
UL0BUFFERZONEFILTER is
set to ULNARROWBANDFILTER.
Uplink narrowband filtering always filters out the interference from UMTS non-
preferential spectrum on both sides of the UMTS network. The
## ULOCELL.
ULLEFTSHAREDBANDWIDTH and
ULOCELL.ULRIGHTSHAREDBANDWIDTH parameters specify the non-preferential
spectrum bandwidth to be filtered out on both sides of the UMTS network. The
values of ULOCELL.
ULLEFTSHAREDBANDWIDTH and
## ULOCELL.
ULRIGHTSHAREDBANDWIDTH must be the same. They must be set to
80, 100, 120, or 140.
Assume that ULOCELL.ULLEFTSHAREDBANDWIDTH and
## ULOCELL.
ULRIGHTSHAREDBANDWIDTH are set to 100. In this case, 1 MHz
bandwidth is filtered out on both the left and right sides of the UMTS network, as
shown in Figure 4-2.
Figure 4-2 Uplink narrowband filtering
## 4.2 Network Analysis
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.17

## 4.2.1 Benefits
## Gains
After this feature is enabled, intra-frequency UMTS cells can be deployed in the UL
buffer zone. This means that UMTS cells can use more spectrum resources,
improving the uplink and downlink capacity of UMTS cells.
●  When uplink adaptive filtering is used, the average uplink throughput or
uplink load of UMTS cells in the buffer zone is 60% or higher of that in
common 5 MHz UMTS cells, and the average downlink throughput is 90% or
higher of that in common 5 MHz UMTS cells.
●  When uplink narrowband filtering is used, the average uplink throughput or
uplink load of UMTS cells in the buffer zone is 30% to 70% that of common 5
MHz UMTS cells, and the average downlink throughput is 90% or higher of
that in common 5 MHz UMTS cells.
The following describes calculation formulas for gain-related KPIs:
●  Number of UEs in CELL_DCH State for Cell
VS.CellDCHUEs
●  Number of Total Bytes Sent in Downlink of HSDPA MAC-d Flow for Cell
VS.HSDPA.MeanChThroughput.TotalBytes
●  Number of Total Bytes Received in Uplink of HSUPA MAC-d Flow for Cell
VS.HSUPA.MeanChThroughput.TotalBytes
●  Average uplink throughput in UMTS cells (kbit/s)
[VS.HSUPA.MeanChThroughput.TotalBytes x 8 + VS.PS.Bkg.UL.8.Traffic +
VS.PS.Bkg.UL.16.Traffic + VS.PS.Bkg.UL.32.Traffic + VS.PS.Bkg.UL.64.Traffic
+ VS.PS.Bkg.UL.128.Traffic + VS.PS.Bkg.UL.144.Traffic +
VS.PS.Bkg.UL.256.Traffic + VS.PS.Bkg.UL.384.Traffic + VS.PS.Int.UL.8.Traffic
+ VS.PS.Int.UL.16.Traffic + VS.PS.Int.UL.32.Traffic + VS.PS.Int.UL.64.Traffic +
VS.PS.Int.UL.128.Traffic + VS.PS.Int.UL.144.Traffic + VS.PS.Int.UL.256.Traffic
+ VS.PS.Int.UL.384.Traffic + VS.PS.Str.UL.8.Traffic + VS.PS.Str.UL.16.Traffic +
VS.PS.Str.UL.32.Traffic + VS.PS.Str.UL.64.Traffic + VS.PS.Str.UL.128.Traffic +
VS.PS.Conv.UL.Traffic]/Traffic statistical period
●  Uplink load percentage (%)
1–10^(– (VS.MeanRTWP – Background noise)/10). The background noise can
be queried by running the LST UCELLCAC command on the RNC.
●  Average downlink throughput in UMTS cells (kbit/s)
[VS.HSDPA.MeanChThroughput.TotalBytes x 8 + VS.PS.Bkg.DL.8.Traffic +
VS.PS.Bkg.DL.16.Traffic + VS.PS.Bkg.DL.32.Traffic + VS.PS.Bkg.DL.64.Traffic
+ VS.PS.Bkg.DL.128.Traffic + VS.PS.Bkg.DL.144.Traffic +
VS.PS.Bkg.DL.256.Traffic + VS.PS.Bkg.DL.384.Traffic + VS.PS.Int.DL.8.Traffic
+ VS.PS.Int.DL.16.Traffic + VS.PS.Int.DL.32.Traffic + VS.PS.Int.DL.64.Traffic +
VS.PS.Int.DL.128.Traffic + VS.PS.Int.DL.144.Traffic + VS.PS.Int.DL.256.Traffic
+ VS.PS.Int.DL.384.Traffic + VS.PS.Str.DL.8.Traffic + VS.PS.Str.DL.16.Traffic +
VS.PS.Str.DL.32.Traffic + VS.PS.Str.DL.64.Traffic + VS.PS.Str.DL.128.Traffic +
VS.PS.Str.DL.144.Traffic + VS.PS.Str.DL.256.Traffic + VS.PS.Str.DL.384.Traffic
+ VS.PS.Conv.DL.Traffic]/Traffic statistical period
●  HSDPA downlink single-user throughput (kbit/s)
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.18

VS.HSDPA.DataOutput.Traffic/VS.HSDPA.DataTtiNum.User/2
●  HSUPA uplink single-user throughput (kbit/s)
(VS.HSUPA.2msTTI.Traffic + VS.HSUPA.10msTTI.Traffic)/
(VS.HSUPA.2msPDU.TTI.Num x 0.002 + VS.HSUPA.10msPDU.TTI.Num x
## 0.01)
## Factors Affecting Gains
The uplink throughput gains of UMTS cells in the buffer zone are affected by the
following factors:
●  The larger the UMTS preferential spectrum, the more available UMTS
spectrum resources, and the higher the average uplink throughput of UMTS
cells.
●  The larger the distance between UMTS and LTE intra-frequency cells, the
smaller the uplink interference of LTE UEs to UMTS cells and the higher the
average uplink throughput of UMTS cells.
●  The smaller the number of CEUs, the smaller the uplink interference of LTE
UEs to UMTS cells and the higher the average uplink throughput of UMTS
cells.
●  It is recommended that the PSD of UMTS cells be equal to that of LTE cells.
The difference between UMTS cell PSD and LTE cell PSD is calculated using
the following formula: 10lg(UMTS power/5 MHz) – 10lg(LTE power/LTE
standard bandwidth). In this formula, the UMTS and LTE power refers to the
sum of the power of multiple antennas. If the 1:1 ratio requirement cannot be
met, the interference between UMTS and LTE cells increases, and the average
downlink throughput of UMTS and LTE cells decreases.
## 4.2.2 Impacts
## Network Impacts
After function deployment:
●  The uplink receive bandwidth of UMTS cells is narrowed. As a result, the
average received total bandwidth power (represented by VS.MeanRTWP) of
the cells decreases by about 1 dB to 3 dB.
●  The RRC connection setup success rate of UMTS cells may decrease and the
service drop rate may increase because UMTS cells are interfered by intra-
frequency neighboring LTE cells. The following describes calculation formulas
for related KPIs:
–   RRC connection setup success rate (service) (%)
[(RRC.SuccConnEstab.OrgConvCall + RRC.SuccConnEstab.OrgStrCall +
RRC.SuccConnEstab.OrgInterCall + RRC.SuccConnEstab.OrgBkgCall +
RRC.SuccConnEstab.OrgSubCall + RRC.SuccConnEstab.TmConvCall +
RRC.SuccConnEstab.TmStrCall + RRC.SuccConnEstab.TmItrCall +
RRC.SuccConnEstab.TmBkgCall + RRC.SuccConnEstab.EmgCall +
RRC.SuccConnEstab.Unkown + RRC.SuccConnEstab.OrgHhPrSig +
RRC.SuccConnEstab.OrgLwPrSig + RRC.SuccConnEstab.CallReEst +
RRC.SuccConnEstab.TmHhPrSig + RRC.SuccConnEstab.TmLwPrSig)/
(RRC.AttConnEstab.OrgConvCall + RRC.AttConnEstab.OrgStrCall +
RRC.AttConnEstab.OrgInterCall + RRC.AttConnEstab.OrgBkgCall +
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.19

RRC.AttConnEstab.OrgSubCall + RRC.AttConnEstab.TmConvCall +
RRC.AttConnEstab.TmStrCall + RRC.AttConnEstab.TmInterCall +
RRC.AttConnEstab.TmBkgCall + RRC.AttConnEstab.EmgCall +
RRC.AttConnEstab.Unknown + RRC.AttConnEstab.OrgHhPrSig +
RRC.AttConnEstab.OrgLwPrSig + RRC.AttConnEstab.CallReEst +
RRC.AttConnEstab.TmHhPrSig + RRC.AttConnEstab.TmLwPrSig)] x
## 100%
–   RRC connection setup success rate (process) (%)
[(RRC.SuccConnEstab.IRATCelRes + RRC.SuccConnEstab.IRATCCO +
RRC.SuccConnEstab.Reg + RRC.SuccConnEstab.Detach)/
(RRC.AttConnEstab.IRATCelRes + RRC.AttConnEstab.IRATCCO +
RRC.AttConnEstab.Reg + RRC.AttConnEstab.Detach)] x 100%
–   CS call drop rate (%)
[VS.RAB.AbnormRel.AMR/(VS.RAB.AbnormRel.AMR +
VS.RAB.NormRel.AMR)] x 100%
–   PS service drop rate (%)
(VS.RAB.AbnormRel.PS - VS.RAB.AbnormRel.PS.PCH -
VS.RAB.AbnormRel.PS.D2P - VS.RAB.AbnormRel.PS.F2P)/
(VS.RAB.AbnormRel.PS + VS.RAB.NormRel.PS -
VS.RAB.AbnormRel.PS.PCH - VS.RAB.NormRel.PS.PCH +
VS.DCCC.D2P.Succ + VS.DCCC.Succ.F2P + VS.DCCC.Succ.D2U +
VS.DCCC.Succ.F2U) x 100%
–   HSDPA call drop rate excluding the call drop rate of UEs in the CELL_PCH
and URA_PCH states (%)
((VS.HSDPA.RAB.AbnormRel - VS.HSDPA.RAB.AbnormRel.H2P)/
(VS.HSDPA.RAB.AbnormRel + VS.HSDPA.RAB.NormRel +
VS.HSDPA.HHO.H2D.SuccOutIntraFreq +
VS.HSDPA.HHO.H2D.SuccOutInterFreq + VS.HSDPA.H2D.Succ +
VS.HSDPA.H2F.Succ + VS.HSDPA.H2P.Succ)) x 100%
–   HSUPA call drop rate excluding the call drop rate of UEs in the CELL_PCH
and URA_PCH states (%)
((VS.HSUPA.RAB.AbnormRel - VS.HSUPA.RAB.AbnormRel.E2P)/
(VS.HSUPA.RAB.AbnormRel + VS.HSUPA.RAB.NormRel +
VS.HSUPA.HHO.E2D.SuccOutIntraFreq +
VS.HSUPA.HHO.E2D.SuccOutInterFreq + VS.HSUPA.E2F.Succ +
VS.HSUPA.E2D.Succ + VS.HSUPA.E2P.Succ)) x 100%
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.20

## Function Impacts
Table 4-1 Impact of the uplink adaptive filtering
## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
## Interference
## Rejection
## Combining
ULOCELL.IRCSWInterference
## Rejection
## Combining
If this function works
with interference
rejection combining
(IRC), uplink signal
correlation is
weakened by filters.
As a result, the
number of effective
UEs with IRC enabled
will reduce and the
feature gains
decrease.
## Adaptive
## Interference
## Rejection
ULOCELL.AIRAdaptive
## Interference
## Rejection
After this function is
enabled, the uplink
receive bandwidth for
interference detection
in Adaptive
## Interference Rejection
is changed to 5 MHz.
As a result, the
effective proportion of
this feature may
change, but the
interference
suppression
performance is not
impaired.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.21

## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
## Flexible
frequency
bandwidth of
UMTS carrier
NoneGU 900 MHz
## Non-standard
## Frequency
## Spacing
After this function is
enabled, the UMTS
cell processes uplink
signals based on the 5
MHz bandwidth.
When the UMTS
flexible carrier
bandwidth is set to a
value other than 5
MHz, the NodeB
sends downlink
signals to the UE
based on the non-5
MHz bandwidth
configuration, and the
NodeB receives uplink
signals from the UE in
the uplink at a
bandwidth of 5 MHz,
decreasing the cell
uplink throughput.
That is, when UMTS
and LTE Zero
Bufferzone is enabled
and either Flexible
frequency bandwidth
of UMTS carrier or
2.0MHz Central
Frequency point
separation between
GSM and UMTS mode
is enabled at the
same time, the uplink
functions of Flexible
frequency bandwidth
of UMTS carrier or
2.0MHz Central
Frequency point
separation between
GSM and UMTS mode
do not take effect.
2.0MHz
## Central
## Frequency
point
separation
between GSM
and UMTS
mode(UMTS)
NoneGU 900 MHz
## Non-standard
## Frequency
## Spacing
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.22

## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
GU@5 MHz
## Phase 2
## ULADAPTIVEBPFI
LTER and
## DLADAPTIVEBPFI
## LTERPERFEOPT
options of the
## ULOCELL.
## GU5MH
## ZPERFOPT
parameter
GU@5 MHzAfter this function and
the Uplink Super
## Narrowband Filter
feature in GU@5 MHz
Phase 2 are enabled,
this feature filters out
the strong
interference in the
received signals of the
UMTS cell. As a result,
the gains of the
## Uplink Super
## Narrowband Filter
feature in GU@5 MHz
Phase 2 may be
reduced, but the
interference
suppression
performance is not
impaired.
HSUPA 2ms
## TTI
## MAP_HSUPA_TTI
## _2MS_SWITCH
option of the
## UCORRMALGOS
WITCH.MapSwitc
h
parameter
HSUPAAfter this function is
enabled, the uplink
bandwidth of UMTS
cells is narrowed and
demodulation
performance
deteriorates. As a
result, the throughput
of HSUPA 2ms TTI
UEs decreases.

SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.23

Table 4-2 Impact of the uplink narrowband filtering
## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
## Interference
## Rejection
## Combining
ULOCELL.IRCSWInterference
## Rejection
## Combining
If this function works
with IRC, uplink signal
correlation is
weakened by filters.
As a result, the
number of effective
UEs with IRC enabled
will reduce and the
feature gains
decrease.
## Adaptive
## Interference
## Rejection
ULOCELL.AIRAdaptive
## Interference
## Rejection
If this function works
with adaptive
interference rejection,
uplink signal
correlation is
weakened by filters.
As a result, the
number of effective
UEs with adaptive
interference rejection
enabled will reduce
and the feature gains
decrease.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.24

## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
## Flexible
frequency
bandwidth of
UMTS carrier
NoneGU 900 MHz
## Non-standard
## Frequency
## Spacing
After this function is
enabled, the UMTS
cell processes uplink
signals based on the 5
MHz bandwidth.
When the UMTS
flexible carrier
bandwidth is set to a
value other than 5
MHz, the NodeB
sends downlink
signals to the UE
based on the non-5
MHz bandwidth
configuration, and the
NodeB receives uplink
signals from UEs in
the uplink at the
configured fixed
bandwidth, decreasing
the cell throughput.
That is, when UMTS
and LTE Zero
Bufferzone is enabled
and either Flexible
frequency bandwidth
of UMTS carrier or
2.0MHz Central
Frequency point
separation between
GSM and UMTS mode
is enabled at the
same time, the uplink
functions of Flexible
frequency bandwidth
of UMTS carrier or
2.0MHz Central
Frequency point
separation between
GSM and UMTS mode
do not take effect.
2.0MHz
## Central
## Frequency
point
separation
between GSM
and UMTS
mode(UMTS)
NoneGU 900 MHz
## Non-standard
## Frequency
## Spacing
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.25

## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
HSUPA 2ms
## TTI
## MAP_HSUPA_TTI
## _2MS_SWITCH
option of the
## UCORRMALGOS
WITCH.MapSwitc
h
parameter
HSUPAAfter this function is
enabled, the uplink
receive bandwidth of
UMTS cells is
narrowed and
demodulation
performance
deteriorates. As a
result, the throughput
of HSUPA 2ms TTI
UEs decreases.
## HSUPA UL
## Interference
## Cancellation
## ULOCELL.ICMOD
## E
HSUPA Data
## Channel
## Interference
## Cancellation
When the uplink
baseband processing
unit is WBBPf or
WBBPd, the burst
service does not take
effect if both this
function and HSUPA
UL Interference
Cancellation are
enabled.
## Narrowband
## Interference
## Suppression
ULOCELL.NBISNarrowband
## Interference
## Suppression
After this function is
enabled, the uplink
receive bandwidth of
UMTS cells is
narrowed and the
measured noise floor
is low. When both this
function and
## Narrowband
## Interference
Suppression are
enabled, the
interference decision
is inaccurate.
Therefore, it is
recommended that
the two functions do
not work together.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.26

## Function
## Name
Function SwitchReference (RAN
## Feature
## Parameter
## Description
## Document)
## Description
## Moving
## Speed-based
## Adaptive
## Demodulation
## ULOCELL.SPEEDB
## ASEDDEMODSW
## Moving Speed-
based Adaptive
## Demodulation
After this function is
enabled, the
narrowband filter
expands signals in the
time domain and
affects the accuracy of
radio channel
parameter estimation.
Therefore, the
demodulation
performance gains
brought by Moving
## Speed-based Adaptive
## Demodulation
decrease.
## Voice
## Coverage
## Improvement
by Advanced
## Demodulation
## ULOCELLALGPAR
## A.COVERIMPBAS
## EDONADVDEM
## Voice Coverage
Improvement by
## Advanced
## Demodulation
After this function is
enabled, wanted
signals, which are
required by Voice
## Coverage
Improvement by
## Advanced
Demodulation to
enhance channel
estimation, may be
weakened. Therefore,
gains brought by
## Voice Coverage
Improvement by
## Advanced
## Demodulation
decrease.

## 4.3 Requirements
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.27

## 4.3.1 Licenses
## Featur
e ID
## Feature
## Name
ModelLicense Control
## Item
NESales
## Unit
## MRFD-
## 150211
UMTS and
LTE Zero
## Bufferzone
## (UMTS)
## LQW9UL0
## BUF01
UMTS and LTE
## Zero Bufferzone
(UMTS) (Per
## Cell)
NodeBPer Cell

## 4.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
Table 4-3 Mutually exclusive functions of uplink adaptive filtering
## Function Name
Function SwitchReference (RAN
## Feature Parameter
## Description Document)
## Independent
Demodulation of Signals
from Multiple Small Cell
RRUs in One Cell
NoneIndependent
Demodulation of Signals
from Multiple Small Cell
RRUs in One Cell
0.5/0.5 configuration
mode
ULOCELL.LOCELLTYPEMultiple RRUs in One
## Cell
## Extended Cell Coverage
up to 200km
NoneExtended Range
4-Antenna Receive
## Diversity
NoneTX Diversity and RX
## Diversity
## Independent
Demodulation of Signals
from Multiple RRUs in
## One Cell
NoneMultiple RRUs in One
## Cell
UMTS 4T Beam
## Optimization
ULOCELL.BFMODEUMTS Beamforming
Inter-Dependence of BBU
## Uplink Resource
NoneInter-Dependence of BBU
## Uplink Resource
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.28

Function NameFunction SwitchReference (RAN
## Feature Parameter
## Description Document)
HSUPA FDEULOCELL.FDEMODEFrequency Domain
## Equalization
Dual Carriers over
## Narrowband
## ULOCELL.DLASYMFILTE
## R
Dual Carriers over
## Narrowband
DC-HSDPA Shared with
## GSM
## ULOCELL.DCHSDPASHA
## REDWITHGSM
DC-HSDPA Shared with
## GSM
UMTS and LTE Spectrum
Sharing Based on DC-
## HSDPA
## ULOCELL.DCHSDPASHA
## REDWITHLTE
UMTS and LTE Spectrum
Sharing Based on DC-
## HSDPA
UMTS Smart 8T BeamULOCELL.BFMODEUMTS Beamforming

Table 4-4 Mutually exclusive functions of uplink narrowband filtering
Function NameFunction SwitchReference (RAN
## Feature Parameter
## Description Document)
## Independent
Demodulation of Signals
from Multiple Small Cell
RRUs in One Cell
NoneIndependent
Demodulation of Signals
from Multiple Small Cell
RRUs in One Cell
## Independent
Demodulation of Signals
from Multiple RRUs in
## One Cell
NoneMultiple RRUs in One
## Cell
0.5/0.5 configuration
mode
ULOCELL.LOCELLTYPEMultiple RRUs in One
## Cell
Inter-Dependence of BBU
## Uplink Resource
NoneInter-Dependence of BBU
## Uplink Resource
## Uplink Super
## Narrowband Filter
## ULOCELL.ULSUPERNAR
## ROWBANDFILTER
GU@5 MHz
UMTS and LTE Spectrum
## Sharing
## ULOCELL.ULSPECTRUM
## SHARINGSWITCH
UMTS and LTE Spectrum
## Sharing
DC-HSDPA Shared with
## GSM
## ULOCELL.DCHSDPASHA
## REDWITHGSM
DC-HSDPA Shared with
## GSM
UMTS and LTE Spectrum
Sharing Based on DC-
## HSDPA
## ULOCELL.DCHSDPASHA
## REDWITHLTE
UMTS and LTE Spectrum
Sharing Based on DC-
## HSDPA

SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.29

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
3900 and 5900 series base stations
## Boards
●  When uplink adaptive filtering is used:
–   The following table lists the function support of each board.
BoardSupported
UMPTYes
UBBPYes
WBBPNo
BBU3910AYes
BBU3910CNo

–   When this function is enabled, the slots that can house a BBP board
providing optical connections must house a UBBP board containing the
UMTS mode, and the BBP board that provides optical connections must
be a UBBP board. If multiple BBP boards provide optical connections, one
of them must be a UBBP board containing the UMTS mode. If the RF
module serving the cell uses the inter-board cold backup ring topology,
the BBP boards connected to the RF module via optical fibers must be
UBBP boards containing the UMTS mode.
–   Interference processing in this function consumes uplink CE resources in
baseband resources. Therefore, the number of available CEs in the uplink
resource group for UMTS cells decreases.
## ▪
If this function is enabled on one to three cells in the uplink resource
group, the number of available CEs in the uplink resource group
decreases by 128.
▪If this function is enabled on four to six cells in the uplink resource
group, the number of available CEs in the uplink resource group
decreases by 256.
–   The cells with this function enabled must be set up on the UBBP/
BBU3910A. The uplink resource group to which the cells belong can
contain UBBP and other types of BBPs. The downlink resource group can
be set up only on the UBBP/BBU3910A.
–   This function is not supported when any of the following conditions are
met:
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.30

▪The BBPs are configured to work in GSM&UMTS&LTE mode.
▪The UBBPd1, UBBPd2, UBBPd3, or UBBPd4 board is configured to
work in GSM&UMTS mode.
▪The BBU3910A model is BBU3910A1, and it is configured to work in
GSM&UMTS or UMTS&LTE mode.
–   After this function is enabled on the preceding BBPs or BBUs supporting
this function, the number of supported UMTS and LTE Zero Bufferzone
cells is half of the number of supported common UMTS cells. For
example, a BBP supports a maximum of six common UMTS cells, among
which a maximum of three UMTS and LTE Zero Bufferzone cells can be
supported and the other three are common UMTS cells.
–   When an uplink resource group serves more than nine cells, enabling this
function triggers reallocation of the baseband resources in the resource
group. The reallocation then possibly causes reestablishment of cells not
enabled with this function in the resource group.
–   When this function is used together with GU@5 MHz Phase 2 and UMTS
and LTE Spectrum Sharing functions, these functions share the resources
of the interface baseband board. Consequently, the number of UMTS and
LTE zero bufferzone (UMTS) cells supported by the interface baseband
board is affected. The interface baseband processing unit supports 24 UL
spectrum sharing cells or 24 GU@5 MHz Phase 2 cells. The maximum
number of UMTS and LTE zero bufferzone (UMTS) cells supported by the
interface baseband board is equal to {24 – Number of GU@5 MHz Phase
2 cells – Number of UL spectrum sharing cells}.
●  When uplink narrowband filtering is used:
The following table lists the function support of each board.
## Board
## Supported
UMPTYes
UBBPYes
WBBPaNo
WBBPbYes. Only the downlink resource
group of the cell with this function
enabled can be set up on the board.
The uplink resource group cannot be
set up on this board.
WBBPdYes, and this function must be
enabled for all cells in the uplink
resource group.
WBBPfYes
BBU3910AYes
BBU3910CYes

SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.31

RF Modules
●  When uplink adaptive filtering is used:
–   RRUs: UMTS-capable RF modules, excluding the MRFU V1, MRRU V1,
## RRU3203RRU3808, WRFU
–   AAUs: AAU3910, AAU3911, AAU3920, AAU3940, AAU5940, and AAU5942
–   Optical module and CPRI bandwidths: The uplink CPRI bandwidth
consumed by a cell running this function is three times that of a common
UMTS cell. Therefore, before enabling this function, evaluate whether
optical modules and CPRI bandwidths meet requirements.
●  When uplink narrowband filtering is used:
–   RRUs: UMTS-capable RF modules, excluding the MRFU V1, MRFU V2,
MRFU V2a, RRU3203RRU3808, RRU3908 V2, WRFU
–   AAUs: AAU3910, AAU3911, AAU3920, AAU3940, AAU5940, and AAU5942
## Cells
TX/RX mode: 1T1R, 1T2R, or 2T2R
## 4.3.4 Networking
●  UMTS and LTE networks belong to the same operator and use Huawei
devices.
●  UMTS and LTE cells are deployed on different base stations.
●  The coverage of base stations in areas with this function deployed is
contiguous.
## 4.3.5 Others
●  When this function is enabled, MRFD-150221 UMTS and LTE Zero Bufferzone
(LTE FDD) must be activated for intra-frequency neighboring LTE cells.
●  After this function is enabled, function derating may occur due to intermittent
disconnections of baseband and RF resources. The function of immediate
reestablishment in the event of function derating must be enabled to address
this issue. Immediate reestablishment in the event of feature derating triggers
reestablishment of all cells under the base station, which interrupts services
for less than 1 minute. This function is controlled by the
SPECTRUMFEAORFUNCTION option of the
## NODEBRESALLOCRULE.
CELLDEGRADEREBUILDSW parameter.
4.4 Operation and Maintenance
4.4.1 When to Use
It is recommended that this feature be enabled in the following scenarios: After
the UMTS spectrum is refarmed to the LTE network, the buffer zone exists for a
long time and the operator expects to improve the capacity of the UMTS and LTE
networks in the buffer zone.
This function is not recommended in the following scenarios:
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.32

●  Hot spots and indoor distribution scenarios: If the inter-site distance (ISD) is
too small, for example, less than 300 m, all UEs need to perform UL
interference processing.
●  High-speed or ultra-high-speed scenarios: Interference cannot be accurately
determined in these scenarios.
●  Scenarios with high LTE uplink PRB usage (greater than 50%): After this
function is enabled, the LTE uplink capacity is easily limited.
●  Scenarios where the buffer zone exists in the short term: Frequent enabling or
disabling of the function brings high maintenance costs.
## 4.4.2 Precautions
●  Pay attention to the following when using the uplink adaptive filtering:
–   It is recommended that this function be activated when traffic is light, for
example, in the early morning. Reconfigurations are required during
function activation, which causes UMTS cells to reset.
–   After this function is enabled, the CPRI bandwidth consumption of UMTS
cells increases. If CPRI bandwidth resources are insufficient, the base
station preferentially allocates resources to the cell with this function
enabled when the local cell is reestablished due to base station reset or
upgrade. As a result, other cells may become unavailable. Each UMTS
carrier, however, requires a continuous CPRI bandwidth. After this
function is enabled, CPRI bandwidth fragments may exist, causing the
UMTS cell capability to decline or making UMTS cells unavailable. To
avoid such problems, all the UMTS cells of the base station must be
deactivated and then reactivated to ensure optimum CPRI bandwidth
allocation.
–   After this function is enabled, the NodeB preferentially allocates the cell
with this function enabled to the UBBP. When cell resources of the board
are insufficient, cells with WRFD-010696 DC-HSDPA and WRFD-160209
192 HSPA Users per Cell enabled report ALM-28206 Local Cell Capability
## Decline.
–   If other cells already occupy the UBBP board resources before this
function is enabled, run the STR REALLOCLOCELL command to
reestablish all local cells and to re-allocate the board resources. If UBBP
board resources are not occupied, skip this operation. Run the LST
ULOCELL command. In the command output, check the values of UL
Baseband Equipment ID and DL Baseband Equipment ID to determine
whether UBBP resources are occupied by other cells.
## NO TICE
After the STR REALLOCLOCELL command is executed, services on local
cells are interrupted for less than 1 minute.
–   If this function is enabled in an uplink resource group consisting of UBBP
boards that support UMTS and LTE, baseband resources in a resource
group will be replanned, and cells in the resource group will be
reestablished.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.33

●  Pay attention to the following when using the uplink narrowband filtering:
–   If the uplink resource group does not contain the UBBP or WBBPf board
and there are common cells in the uplink resource group, you are advised
not to enable uplink narrowband filtering in existing common cells or
new common cells. Otherwise, ALM-28206 Local Cell Capability Decline is
reported when uplink narrowband filtering is enabled. That is, uplink
narrowband filtering does not take effect. If this occurs, the UBBP or
WBBPf board can be added to the uplink resource group. After uplink
narrowband filtering is enabled, the common cell changes from the
derating state to the available state. In this case, service drops occur in
the cell. After UEs access the network again, the fault is rectified.
–   If the uplink resource group does not contain the UBBP or WBBPf board
and uplink narrowband filtering has been enabled for all cells in the
uplink resource group, you are advised not to add common cells.
Otherwise, ALM-28203 Local Cell Unusable is reported. That is, common
cells are unavailable. If this occurs, the UBBP or WBBPf board can be
added to the uplink resource group and all cells are reorganized to
recover common cells.
## 4.4.3 Data Configuration
## 4.4.3.1 Data Preparation
Table 4-5 describes the parameters used for function activation.
Table 4-5 Parameters used for activation
## Parameter Name
Parameter IDSetting Notes
UMTS and LTE Zero
## Bufferzone
## ULOCELL.UL0BUFFERZ
## ONE
Set this parameter to TRUE.
UMTS and LTE Zero
## Bufferzone Filter
## ULOCELL.UL0BUFFERZ
## ONEFILTER
Set this parameter to
ULADAPTIVEFILTER or
## ULNARROWBANDFILTER
based on the network plan.
## Uplink Left Shared
## Bandwidth
## ULOCELL.ULLEFTSHARE
## DBANDWIDTH
Set this parameter based on
the network plan.
## Uplink Right Shared
## Bandwidth
## ULOCELL.ULRIGHTSHA
## REDBANDWIDTH
Set this parameter based on
the network plan.

4.4.3.2 Using MML Commands
## Activation Command Examples
//Enabling uplink adaptive filtering in UMTS and LTE Zero Bufferzone and configuring the UMTS non-
preferential spectrum range
## MOD ULOCELL: ULOCELLID=0, LOCELLTYPE=NORMAL_CELL, UL0BUFFERZONE=TRUE,
## UL0BUFFERZONEFILTER=ULADAPTIVEFILTER, ULLEFTSHAREDBANDWIDTH=133,
## ULRIGHTSHAREDBANDWIDTH=133;
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.34

//Enabling uplink narrowband filtering in UMTS and LTE Zero Bufferzone and configuring the UMTS non-
preferential spectrum range
## MOD ULOCELL: ULOCELLID=0, LOCELLTYPE=NORMAL_CELL, UL0BUFFERZONE=TRUE,
## UL0BUFFERZONEFILTER=ULNARROWBANDFILTER, ULLEFTSHAREDBANDWIDTH=100,
## ULRIGHTSHAREDBANDWIDTH=100;
//(Optional) Running this command only when UBBP resources are occupied by other cells before this
feature is enabled
## STR REALLOCLOCELL:;
## Deactivation Command Examples
//Turning off the UMTS and LTE Zero Bufferzone (UMTS) switch and removing the configuration of the
UMTS non-preferential spectrum range
## MOD ULOCELL: ULOCELLID=0, LOCELLTYPE=NORMAL_CELL, UL0BUFFERZONE=FALSE,
## ULLEFTSHAREDBANDWIDTH=0, ULRIGHTSHAREDBANDWIDTH=0;
4.4.3.3 Using the MAE-Deployment
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
## 4.4.4 Activation Verification
## ●  Method 1
On the NodeB, run the DSP ULOCELL command. If the value of UMTS and
LTE Zero Bufferzone Capability is AVAILABLE, uplink adaptive filtering or
uplink narrowband filtering has been enabled.
## ●  Method 2
–   Check the value of VS.BasebandNBIS.Bandwidth.Mean on the NodeB. If
the value of this counter is greater than 0, uplink adaptive filtering has
been enabled.
–   Start the UMTS FFT frequency scanning function on the LMT with the
Scan Mode parameter set to High-resolution Online Frequency, and
observe the occupied bandwidth. If the bandwidth is the same as that
configured for uplink narrowband filtering of the cell, uplink narrowband
filtering has been enabled. For details about UMTS FFT frequency
scanning, see "FFT Frequency Scanning" in
## 3900 & 5900 Series Base
Station LMT User Guide
in 3900 & 5900 Series Base Station Product
## Documentation
## .
## 4.4.5 Network Monitoring
After this function is enabled, check the network capacity before and after the
function is enabled based on the KPIs related to gains in 4.2.1 Benefits.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.35

If ALM-28206 Local Cell Capability Decline is reported due to insufficient
configuration capability, software capability, or hardware capability, rectify the
fault according to the alarm handling procedure.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description4 UMTS and LTE Zero Bufferzone (UMTS)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.36

5 UMTS and LTE Zero Bufferzone (LTE
## FDD)
## 5.1 Principles
The UMTS_LTE_ZERO_BUFFER_ZONE_SW option of the
ULZeroBufferZone.
ZeroBufZoneSwitch parameter specifies whether to enable
this function.
This function reduces interference from LTE UEs to UMTS cells by allocating and
scheduling uplink physical channel resources. This function optimizes the
allocation and scheduling of PUCCH, SRS, PRACH, and PUSCH resources. For
details about resource allocation and scheduling of other physical channels, see
Physical Channel Resource Management in eRAN Feature Documentation.
## PUCCH
PUCCH PRBs are configured on the LTE-dedicated spectrum and UMTS non-
preferential spectrum to reduce uplink interference from the PUCCH to UMTS
cells.
SRS and PRACH
The SRS and PRACH PRBs are configured on the LTE-dedicated spectrum and
UMTS non-preferential spectrum. The SRS and PRACH can reuse the same PRB
resources to reduce the uplink interference from the SRS and PRACH to the UMTS
cell.
## PUSCH
As shown in Figure 5-1, the PUSCH uses different scheduling policies based on the
location of the UE in the LTE cell.
●  For LTE CEUs, only the PRBs on the LTE-dedicated spectrum or UMTS non-
preferential spectrum can be scheduled for the PUSCH because the path loss
between these UEs and intra-frequency neighboring UMTS cells is relatively
small.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.37

●  For LTE CCUs, all spectrum can be scheduled for the PUSCH because the path
loss between these UEs and intra-frequency neighboring UMTS cells is
relatively large. The spectrum includes PRB resources of LTE-dedicated
spectrum, UMTS preferential spectrum, and UMTS non-preferential spectrum.
The UtranNFreq.ULSharedFreqInd parameter must be set to BOOLEAN_TRUE to
determine the location of an LTE UE.
Figure 5-1 PUSCH resource scheduling policy
Figure 5-2 shows the scheduling procedure for PUSCH resources.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.38

Figure 5-2 PUSCH resource scheduling procedure
-  Check the uplink PRB usage in an LTE cell.
–   If the eNodeB determines that the uplink PRB usage of the LTE cell is low,
only the LTE-dedicated spectrum and the PRB resources on the UMTS
non-preferential spectrum are used in the uplink.
–   If the eNodeB determines that the uplink PRB usage of the LTE cell is
high, go to 2.
-  Determine the location of an LTE UE.
–   The eNodeB triggers the LTE UE to periodically perform intra-frequency
measurements on all neighboring UMTS cells whose
UtranNFreq.
ULSharedFreqInd is set to BOOLEAN_TRUE based on the
UE-level timer ULZeroBufferZone.
ULZeroBufZoInterRatB1Timer if the
following condition is true: ULZeroBufferZone.ULZeroBufZoneRsrpThd –
ULZeroBufferZone.
ULZeroBufZoneRsrpOffset –
ULZeroBufferZone.
ULZeroBufZoneB1RmvOffset ≤ Downlink RSRP of
the LTE UE < ULZeroBufferZone.
ULZeroBufZoneRsrpThd +
ULZeroBufferZone.ULZeroBufZoneB1RmvOffset. Then, the eNodeB
classifies LTE UE positions based on the RSCP of the neighboring UMTS
cells:
▪If the measured neighboring UMTS cell RSCP is smaller than the
ULZeroBufferZone.
ULZeroBufZoneUtranRscpThd parameter value,
the eNodeB determines that the LTE UE is a CCU.
▪If the measured neighboring UMTS cell RSCP is greater than or equal
to the ULZeroBufferZone.
ULZeroBufZoneUtranRscpThd parameter
value, the eNodeB determines that the LTE UE is a CEU.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.39

–   If the downlink RSRP of an LTE UE is beyond the preceding range, the
eNodeB does not trigger the measurement of intra-frequency
neighboring UMTS cells of the LTE UE. The eNodeB directly performs
location classification based on the RSRP of the LTE UE.
▪The eNodeB determines that the UE is a CCU if the following
condition is true: Downlink RSRP of the LTE UE ≥
ULZeroBufferZone.ULZeroBufZoneRsrpThd +
ULZeroBufferZone.
ULZeroBufZoneB1RmvOffset parameter values.
▪The eNodeB determines that the UE is a CEU if the following
condition is true: Downlink RSRP of the LTE UE <
ULZeroBufferZone.
ULZeroBufZoneRsrpThd –
ULZeroBufferZone.ULZeroBufZoneRsrpOffset –
ULZeroBufferZone.
ULZeroBufZoneB1RmvOffset parameter values.
-  PRB scheduling based on LTE UE position
–   If the UE is a CCU, the eNodeB can use all spectrum when scheduling the
PUSCH of the LTE UE. The spectrum includes PRB resources of LTE-
dedicated spectrum, UMTS preferential spectrum, and UMTS non-
preferential spectrum.
–   If the UE is a CEU, the eNodeB can use PRB resources corresponding to
the LTE-dedicated spectrum and UMTS non-preferential spectrum when
scheduling the PUSCH of the LTE UE.
## NO TE
●  The downlink RSRP of LTE UEs is calculated based on the uplink path loss, which may be
slightly different from the actual downlink RSRP of LTE UEs.
●  If the LTE UE does not support UMTS, the intra-frequency neighboring UMTS cell
measurement is not triggered and the UE is regarded as a CEU.
●  If the LTE cell and UMTS cell have spectrum overlapping but the UMTS cell is not
configured as an inter-RAT neighboring cell of the LTE cell, configure the external
UTRAN cell of the LTE cell and the inter-RAT neighboring UMTS cell of the LTE cell in
the UtranExternalCell and UtranNCell MOs. This ensures that LTE UEs can measure
neighboring UMTS cells.
## 5.2 Network Analysis
## 5.2.1 Benefits
After this function is enabled, LTE cells in the UMTS and LTE buffer zone can use a
larger standard bandwidth. However, some LTE UEs may cause strong interference
to the UMTS network, and these UEs cannot schedule PRB resources in the UMTS
preferential spectrum. Therefore, the uplink capacity of LTE cells in the buffer zone
is 20% to 70% that of common LTE cells and the downlink capacity of LTE cells is
70% to 90% that of common LTE cells. The formula for calculating the uplink
capacity and downlink capacity of an LTE cell is as follows:
●  LTE cell downlink capacity = Number of available PRBs in an LTE cell x
Spectral efficiency = L.ChMeas.PRB.DL.Avail x
((L.Traffic.DL.SCH.QPSK.TB.bits + L.Traffic.DL.SCH.16QAM.TB.bits +
L.Traffic.DL.SCH.64QAM.TB.bits + L.Traffic.DL.SCH.256QAM.TB.bits)/
L.ChMeas.PRB.DL.Used.Avg/Statistical period/10^6)
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.40

●  LTE cell uplink capacity = Number of available PRBs in a cell x Spectrum
efficiency = L.ChMeas.PRB.UL.Avail x ((L.Traffic.UL.SCH.QPSK.TB.bits +
L.Traffic.UL.SCH.16QAM.TB.bits + L.Traffic.UL.SCH.64QAM.TB.bits)/
L.ChMeas.PRB.UL.Used.Avg/Statistical period/10^6)
Table 5-1 lists the lower limit of the uplink capacity of different LTE standard
bandwidths and the number of uplink shared carriers compared with the uplink
capacity of common LTE cells.
Table 5-1 Uplink capacity of UMTS and LTE zero buffer zone cells
LTE Standard
## Bandwidth
Number of UMTS
Carriers in the UL
## Shared Spectrum
Lower Limit of the
Proportion of Uplink
Capacity to Common
LTE Cells
5 MHz120%
10 MHz159%
10 MHz225%
15 MHz165%
15 MHz252%
15 MHz334%
20 MHz166%
20 MHz260%
20 MHz348%
20 MHz439%

In new LTE deployment, the capacity baseline of common LTE cells cannot be
obtained directly. In this case, the capacity baseline can be calculated using the
following formula: LTE common cell capacity baseline = (Single-user peak rate test
value/Number of actually invoked PRBs) x Number of available PRBs outside the
UMTS preferential spectrum.
## NO TE
●  The uplink capacity of an LTE cell depends on the distance between the UMTS cell and
the LTE cell and the UE location. The larger the inter-site distance and the larger the
number of CCUs, the larger the uplink capacity of an LTE cell.
●  It is recommended that the PSD of UMTS cells be equal to that of LTE cells. The
difference between UMTS cell PSD and LTE cell PSD is calculated using the following
formula: 10lg(UMTS power/5 MHz) – 10lg(LTE power/LTE standard bandwidth). In this
formula, the UMTS and LTE power refers to the sum of the power of multiple antennas.
If the 1:1 ratio requirement cannot be met, the interference between UMTS and LTE
cells increases, and the average downlink throughput of UMTS and LTE cells decreases.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.41

## 5.2.2 Impacts
## Network Impacts
●  Inter-RAT interference avoidance between UMTS and LTE requires LTE UEs to
start inter-RAT measurements. The gap-assisted measurement results in a
decrease in the uplink and downlink peak rates of a single LTE UE. LTE UEs
with strong interference in neighboring UMTS cells cannot use the UMTS
preferential spectrum. As a result, the uplink peak rate of a single LTE UE
decreases.
●  In UMTS and LTE intra-frequency neighboring networking, the impacts of
UMTS interference on the LTE network are as follows. The impact of each
impact item is within 5%.
–   The RRC connection or E-RAB setup success rate decreases.
–   The bearer service drop rate increases.
–   The number of RRC connection reestablishments increases.
–   The average number of UEs in a cell decreases.
–   The uplink and downlink BLERs of cells increase.
–   The outgoing intra-frequency handover success rate decreases.
●  When LTE-dedicated carriers exist, the LTE bandwidth is different from the
center frequency. Therefore, the inter-frequency handover between LTE cells
increases, and the inter-frequency outgoing handover success rate decreases.
Table 5-2 lists the KPIs related to network impact on the LTE side.
Table 5-2 KPIs related to network impact on the LTE side
## KPI
FormulaImpact
## RRC
connection
setup success
rate
L.RRC.ConnReq.Succ/L.RRC.ConnReq.AttDecreased
E-RAB setup
success rate
L.E-RAB.SuccEst/L.E-RAB.AttEstDecreased
Bearer call
drop rate
L.E-RAB.AbnormRel/(L.E-RAB.AbnormRel
+L.E-RAB.NormRel)
## Increased
Number of
## RRC
connection
reestablishme
nt times
L.RRC.ReEst.AttIncreased
## Average
number of
UEs in a cell
L.Traffic.User.AvgDecreased
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.42

KPIFormulaImpact
Cell uplink
## BLER
(L.Traffic.UL.SCH.QPSK.ErrTB.Rbler +
L.Traffic.UL.SCH.16QAM.ErrTB.Rbler +
L.Traffic.UL.SCH.64QAM.ErrTB.Rbler)/
(L.Traffic.UL.SCH.QPSK.TB +
L.Traffic.UL.SCH.16QAM.TB +
L.Traffic.UL.SCH.64QAM.TB)
## Increased
Cell downlink
## BLER
(L.Traffic.DL.SCH.QPSK.ErrTB.Rbler +
L.Traffic.DL.SCH.16QAM.ErrTB.Rbler +
L.Traffic.DL.SCH.64QAM.ErrTB.Rbler)/
(L.Traffic.DL.SCH.QPSK.TB +
L.Traffic.DL.SCH.16QAM.TB +
L.Traffic.DL.SCH.64QAM.TB)
## Increased
## Outgoing
intra-
frequency
handover
success rate
(L.HHO.IntraeNB.IntraFreq.ExecSuccOut
## +
L.HHO.IntereNB.IntraFreq.ExecSuccOut)/
(L.HHO.IntraeNB.IntraFreq.ExecAttOut +
L.HHO.IntereNB.IntraFreq.ExecAttOut)
## Decreased
## Outgoing
inter-
frequency
handover
success rate
(L.HHO.IntraeNB.InterFreq.ExecSuccOut
## +
L.HHO.IntereNB.InterFreq.ExecSuccOut)/
(L.HHO.IntraeNB.InterFreq.ExecAttOut +
L.HHO.IntereNB.InterFreq.ExecAttOut)
## Decreased

## Function Impacts
## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
UMTS and
LTE Spectrum
Sharing (LTE
## FDD)
SpectrumCloud.S
pectrumCloudSw
itch
UMTS and LTE
## Spectrum Sharing
When the two
functions are enabled
at the same time, the
LTE uplink capacity
gains of the two
functions decrease.
## Compact
bandwidth
Cell.CustomizedB
andWidthCfgInd
## Compact
Bandwidth (FDD)
When the two
functions are enabled
at the same time, the
LTE uplink capacity
gains of the two
functions decrease.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.43

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
SRS resource
management
SRSCfg.SrsCfgIndPhysical Channel
## Resource
## Management
The SRS can use only
the PRB resources of
the UMTS preferential
spectrum. Therefore,
the resources that can
be allocated to the
SRS are reduced. As a
result, the SRS does
not support the
frequency hopping
function.
SFN cellCell.MultiRruCell
## Mode
SFNThe SRS can use only
the PRB resources of
the UMTS preferential
spectrum. Therefore,
the resources that can
be allocated to the
SRS are reduced. As a
result, the SFN cell
performance
deteriorates.
Intra-eNodeB
and inter-
eNodeB
uplink
interference
cancellation
UlIntraSiteIcSwit
ch and
UlInterSiteIcSwit
ch options of the
CellAlgoSwitch.U
plinkIcSwitch
parameter
## Uplink
## Interference
## Cancellation
## (FDD)
This function cannot
process inter-RAT
interference from the
UMTS network. As a
result, the gain
decreases.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.44

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
UL CoMP cellUlJointReception
Switch option of
the
CellAlgoSwitch.U
plinkCompSwitch
parameter
UL CoMP● The SRS can use
only the PRB
resources of the
UMTS preferential
spectrum.
Therefore, the
resources that can
be allocated to the
SRS are reduced. As
a result, the UL
CoMP cell
performance
deteriorates.
● If UL CoMP is
enabled in both
the buffer zone
and non-buffer-
zone areas, the
uplink capacity of
UL CoMP may be
negatively affected.
LTE in-band
deployment
Prb.DeployModeNB-IoT Basics
## (FDD)
LTE in-band
deployment must
avoid UMTS
preferential spectrum
to avoid inter-RAT
interference. It is
recommended that
LTE in-band
deployment be
enabled on the LTE-
dedicated spectrum.
eMTC
introduction
## EMTC_SWITCH
option of the
CellEmtcAlgo.Em
tcAlgoSwitch
parameter
eMTCeMTC deployment
must avoid UMTS
preferential spectrum
to avoid inter-RAT
interference. It is
recommended that
eMTC deployment be
enabled on the LTE-
dedicated spectrum.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.45

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
Uplink SU-
## MIMO
ULSUMIMO2Laye
rsSwitch option
of the
CellAlgoSwitch.U
lSuMimoAlgoSwi
tch
parameter
MIMOThe SRS can use only
the PRB resources of
the UMTS preferential
spectrum. Therefore,
the resources that can
be allocated to the
SRS are reduced. As a
result, the uplink SU-
MIMO performance
deteriorates.
## Uplink 2x2
## MU-MIMO
UlVmimoSwitch
option of the
CellAlgoSwitch.U
lSchSwitch
parameter
MIMOThe SRS can use only
the PRB resources of
the UMTS preferential
spectrum. Therefore,
the resources that can
be allocated to the
SRS are reduced. As a
result, the uplink 2x2
## MU-MIMO
performance
deteriorates.
Virtual 4T4RVirtual4T4RSwitc
h option of the
CellAlgoSwitch.E
mimoSwitch
parameter
Virtual 4T4R
## (FDD)
The SRS can use only
the PRB resources of
the UMTS preferential
spectrum. Therefore,
the resources that can
be allocated to the
SRS are reduced. As a
result, the virtual
4T4R performance
deteriorates.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.46

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
Inter-eNodeB
CA based on
relaxed
backhaul
RelaxedBHCaEnh
anceSwitch
option of the
ENodeBAlgoSwit
ch.CaAlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
## Carrier
## Aggregation
for Downlink
3CC in 40MHz
CaDl3CCSwitch
option of the
CaMgtCfg.CellCa
AlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
## Carrier
## Aggregation
for Downlink
3CC in 60MHz
CaDl3CCSwitch
option of the
CaMgtCfg.CellCa
AlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.47

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
## Carrier
## Aggregation
for Downlink
4CC and 5CC
CaDl4CCSwitch
and
CaDl5CCSwitch
options of the
CaMgtCfg.CellCa
AlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
## Carrier
## Aggregation
for Uplink
## 2CC
CaUl2CCSwitch
option of the
CaMgtCfg.CellCa
AlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.48

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
## Downlink
Massive CA
●CaDl5CCSwitc
h option of the
CaMgtCfg.Cell
CaAlgoSwitch
parameter
●UeBandComb
ReducedR13S
w option of
the
ENodeBAlgoS
witch.
CaAlgoE
xtSwitch
parameter
●DlMassiveCaS
witch option
of the
CaMgtCfg.
## Cell
CaAlgoSwitch
parameter
## Carrier
## Aggregation
The PUSCH and SRS
resources of a cell in
the buffer zone are
less than those of a
common cell.
Therefore, when the
LTE bandwidth is 5
MHz or 10 MHz, it is
not recommended
that the cell in the
buffer zone be used
as the primary cell for
CA. Otherwise, the
performance of CA
deteriorates.
Inter-RAT
## ANR
## INTER_RAT_ANR_
SW option of the
CellAlgoSwitch.A
nrFunctionSwitc
h parameter
## ANR
## Management
A UMTS cell must be
added as a
neighboring cell of an
LTE cell in the buffer
zone. When the inter-
RAT ANR function is
enabled, the
neighboring UMTS
cells in the buffer
zone may be deleted
if the number of
neighboring UMTS
cells of the LTE cell
reaches the
maximum. Therefore,
UtranNCell.
NoRmvFl
ag
must be set to
## FORBID_RMV_ENUM
for neighboring UMTS
cells with close
interference.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.49

## Function
## Name
Function SwitchReference (eRAN
## Feature
## Parameter
## Description
## Document)
## Description
## Uplink
interference
randomizatio
n
CellUlschAlgo.Ul
RbAllocationStra
tegy set to
## FS_INRANDOM_
## ADAPTIVE
ICICAfter UMTS and LTE
Zero Bufferzone is
enabled, the PRB
resources far away
from the UMTS
preferential spectrum
are preferentially
scheduled. As a result,
the uplink interference
randomization
function becomes
invalid.
UMTS and
LTE Spectrum
## Sharing Based
on DC-HSDPA
SpectrumCloud.S
pectrumCloudSw
itch
UMTS and LTE
## Spectrum Sharing
Based on DC-
## HSDPA
When the two
functions are enabled
at the same time, the
LTE uplink capacity
gains of the two
functions decrease.

## 5.3 Requirements
## 5.3.1 Licenses
## Featur
e ID
## Feature
## Name
ModelLicense Control
## Item
NESales
## Unit
## MRFD-
## 150221
UMTS and
LTE Zero
## Bufferzone
## (LTE FDD)
## LT1S0ULZ
## BS00
UMTS and LTE
## Zero Bufferzone
(LTE FDD) (Per
## Cell)
eNodeBPer Cell

## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.50

## Mutually Exclusive Functions
## Function
## Name
Function SwitchReference (eRAN
## Feature Parameter
## Description
## Document)
LTE FDD and
NR Uplink
## Spectrum
## Sharing
SpectrumCloud.SpectrumCloudSwitc
h
LTE FDD and NR
## Uplink Spectrum
## Sharing
LTE FDD and
NR Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.SpectrumCloudSwitc
h
LTE FDD and NR
## Spectrum Sharing
GSM and LTE
## Spectrum
## Concurrency
SpectrumCloud.SpectrumCloudSwitc
h
GSM and LTE
## Spectrum Concurrency
GSM and LTE
## Dynamic
## Spectrum
## Sharing
GLDynSpectrumShareSwitch option
of the
CellAlgoSwitch.DynSpectrumShareS-
witch parameter
## None
GSM and LTE
## Zero
## Bufferzone
GLZeroBufferZoneSwitch option of
the
CellAlgoSwitch.DynSpectrumShareS-
witch parameter
## None
GSM and LTE
## Buffer Zone
## Optimization
AvoidGeranInterfSwitch option of the
CellAlgoSwitch.AvoidInterfSwitch
parameter
GSM and LTE Buffer
## Zone Optimization
CDMA and
LTE Zero
## Bufferzone
AvoidCDMAInterfSwitch option of
the
CellAlgoSwitch.AvoidInterfSwitch
parameter
CDMA and LTE Zero
## Bufferzone
UL Refarming
## Zero
## Bufferzone
AvoidUtranInterfSwitch option of the
CellAlgoSwitch.AvoidInterfSwitch
parameter
UL Refarming Zero
## Bufferzone
## Flexible
bandwidth
based on
overlapping
carriers
DdCellGroup.DdBandwidthFlexible Bandwidth
based on Overlap
Carriers (FDD)
## Adaptive
inter-cell
interference
coordination
NoneAdaptive ICIC
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.51

## Function
## Name
Function SwitchReference (eRAN
## Feature Parameter
## Description
## Document)
High speed
mobility
Cell.HighSpeedFlagHigh Speed Mobility
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh Speed Mobility
## Super
combined cell
SuperCombCellSwitch option of the
CellAlgoSwitch.SfnAlgoSwitch
parameter
## Super Combined Cell
## (FDD)
## Zero Guard
## Band
## Between
## Contiguous
Intra-Band
## Carriers
## CONTIG_INTRA_BAND_CARR_SW
option of the ContigIntraBand-
Carr.ContigIntraBandCarrSw
parameter
Seamless Intra-Band
Carrier Joining (FDD)

## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
3900 and 5900 series base stations
## Boards
## Board
## Supported
UMPTYes
LBBPcNo
LBBPdYes
UBBPYes
BBU3910AYes

RF Modules
No requirements
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.52

## Cells
TX/RX mode: no requirements
Cell bandwidth: 5 MHz, 10 MHz, 15 MHz, and 20 MHz
## 5.3.4 Networking
For details, see 4.3.4 Networking.
## 5.3.5 Others
When this function is enabled, MRFD-150211 UMTS and LTE Zero Bufferzone
(UMTS) must be activated for intra-frequency neighboring UMTS cells.
5.4 Operation and Maintenance
5.4.1 When to Use
For details, see 4.4.1 When to Use.
## 5.4.2 Precautions
To ensure the UMTS performance, the UMTS preferential spectrum must be
configured in the center of the UMTS bandwidth and avoid the PUCCH. If the
PUCCH and the UMTS preferential spectrum overlap, the UMTS cell has extra 5%
performance loss.
## 5.4.3 Data Configuration
It is recommended that this function be activated when traffic is light, for
example, in the early morning. Reconfigurations are required during function
activation, which causes LTE and UMTS cells to reset.
## 5.4.3.1 Data Preparation
Table 5-3 and Table 5-4 describe the parameters used for function activation and
optimization, respectively. Parameters related to LTE cell setup and inter-RAT
neighboring UMTS cell configuration are not described in the tables.
## NO TE
Before enabling this function, ensure that neighboring UTRAN cells are set up between the
LTE and UMTS networks in the buffer zone. Otherwise, interference measurement and
resource allocation may be inaccurate, resulting in poor UMTS network performance.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.53

Table 5-3 Parameters used for activation
Parameter NameParameter IDSetting Notes
## Zero Buffer Zone
## Switch
ULZeroBufferZone.Ze
roBufZoneSwitch
Select the
## UMTS_LTE_ZERO_BUFFER_ZO
NE_SW option.
UMTS and LTE
## Spectrum Sharing
Config ID
ULZeroBufferZone.U
LSpectrumSharing-
ConfigId
Set this parameter based on
the network plan.
UMTS and LTE
## Spectrum Sharing
Config ID
ULSpectrumShrCon-
fig.ULSpectrumShari
ngConfigId
Set this parameter based on
the network plan.
PRB Reserve TypeULSpectrumShrCon-
fig.PrbRsvType
When the UMTS preferential
spectrum is configured, set
this parameter to
## UMTS_CORE_SPECTRUM
When the UL shared spectrum
is configured, set this
parameter to
## UMTS_LTE_SHARED_SPECTR
## UM.
LTE PRB Start IndexULSpectrumShrCon-
fig.LtePrbStartIndex
Set this parameter based on
the network plan.
LTE PRB End IndexULSpectrumShrCon-
fig.LtePrbEndIndex
Set this parameter based on
the network plan.
UMTS/LTE Shared
## Frequency Indicator
UtranNFreq.ULShare
dFreqInd
Set this parameter based on
the network plan.
PRACH Frequency
## Offset Strategy
RACHCfg.PrachFreqOf
fsetStrategy
Set this parameter based on
the network plan.
## SRS ACK/NACK
simultaneous
transmission
SRSCfg.AnSrsSimuTr
ans
Set this parameter to
## BOOLEAN_TRUE.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.54

Parameter NameParameter IDSetting Notes
PUCCH algorithm
switch
CellAlgoSwitch.Pucc
hAlgoSwitch
If RACHCfg.PrachFreqOffset-
Strategy is set to MANUAL:
● If six or more RBs are
reserved only on the
PUCCH side, it is
recommended that both
the PucchSwitch and
PucchFlexCfgSwitch
options be selected and
PUCCHCfg.
PucchExtended
RBNum
be set based on
the network plan.
● If fewer than six RBs are
reserved only for the
PUCCH, deselect the
PucchSwitch option and
select the
PucchFlexCfgSwitch
option. Otherwise, cell
activation may fail.
If RACHCfg.
PrachFreqOffset-
Strategy is not set to
MANUAL, select the
PucchSwitch option.
No remove indicator
UtranNCell.NoRmvFl
ag
Set this parameter to
## FORBID_RMV_ENUM.

Table 5-4 Parameters used for optimization
## Parameter Name
Parameter IDSetting Notes
UL Zero Buffer Zone
Downlink RSRP
## Threshold
ULZeroBufferZone.UL
ZeroBufZoneRsrpThd
The default value is
recommended.
UL Zero Buffer Zone
Downlink RSRP Offset
ULZeroBufferZone.UL
ZeroBufZoneRsrpOff-
set
The default value is
recommended.
UL Zero Buffer Zone
## B1 Remove Offset
ULZeroBufferZone.UL
ZeroBufZoneB1RmvOf
fset
The default value is
recommended.
UTRAN RSCP Report
## Threshold
ULZeroBufferZone.UL
ZeroBufZoneUtranRs
cpThd
The default value is
recommended.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.55

Parameter NameParameter IDSetting Notes
UL Zero Buffer Zone
## Inter Rat B1 Timer
ULZeroBufferZone.UL
ZeroBufZoInterRatB1
## Timer
The default value is
recommended.

5.4.3.2 Using MML Commands
Deactivate LTE cells, and perform the following operations to configure related
parameters before reactivating these cells.
## Activation Command Examples
//(Optional) Reconfiguring the LTE center E-UTRA absolute radio frequency channel number (EARFCN) and
bandwidths if necessary
MOD CELL: LocalCellId=0, DlEarfcn=307, DlBandWidth=CELL_BW_N50, UlBandWidth=CELL_BW_N50;
//Configuring the UL shared frequency indicator of the UMTS frequency with overlapping spectrum
MOD UTRANNFREQ: LocalCellId=0, UtranDlArfcn=10715, ULSharedFreqInd=BOOLEAN_TRUE;
//(Optional) Adding neighbor UTRAN relationship if no neighboring UTRAN cell is configured for the LTE
cell in the overlapping area of the UL spectrum
ADD UTRANNFREQ: LocalCellId=0, UtranDlArfcn=10715, UtranFddTddType=UTRAN_FDD,
UtranUlArfcnCfgInd=NOT_CFG, CellReselPriorityCfgInd=NOT_CFG, ULSharedFreqInd=BOOLEAN_TRUE;
ADD UTRANEXTERNALCELL: Mcc="460", Mnc="00", RncId=123, CellId=2, UtranDlArfcn=10715,
UtranUlArfcnCfgInd=NOT_CFG, UtranFddTddType=UTRAN_FDD, RacCfgInd=CFG, Rac=130,
PScrambCode=100, Lac=120;
ADD UTRANNCELL: LocalCellId=0, Mcc="460", Mnc="00", RncId=123, CellId=2;
//Setting the No remove indicator of the neighboring UMTS cell to FORBID_RMV_ENUM
MOD UTRANNCELL: LocalCellId=0, Mcc="460", Mnc="00", RncId=123, CellId=2,
NoRmvFlag=FORBID_RMV_ENUM;
//Configuring the range of UMTS preferential spectrum and UL shared spectrum
ADD ULSPECTRUMSHRCONFIG: ULSpectrumSharingConfigId=6, PrbRsvType=UMTS_CORE_SPECTRUM_1,
LtePrbStartIndex=6, LtePrbEndIndex=18;
ADD ULSPECTRUMSHRCONFIG: ULSpectrumSharingConfigId=6, PrbRsvType=UMTS_CORE_SPECTRUM_2,
LtePrbStartIndex=31, LtePrbEndIndex=43;
ADD ULSPECTRUMSHRCONFIG: ULSpectrumSharingConfigId=6,
PrbRsvType=UMTS_LTE_SHARED_SPECTRUM, LtePrbStartIndex=0, LtePrbEndIndex=49;
//Enabling the UMTS and LTE Zero Bufferzone function
MOD ULZEROBUFFERZONE: LocalCellId=0, ZeroBufZoneSwitch=UMTS_LTE_ZERO_BUFFER_ZONE_SW-1,
ULZeroBufZoneUtranRscpThd=-103, ULZeroBufZoneRsrpOffset=60, ULZeroBufZoneRsrpThd=-60,
ULZeroBufZoInterRatB1Timer=30, ULZeroBufZoneB1RmvOffset=3, ULSpectrumSharingConfigId=6;
//Configuring the PRACH frequency offset policy
MOD RACHCFG: LocalCellId=0, PrachFreqOffsetStrategy=FULLY_AUTOMATIC;
//Configuring the SRS ACK/NACK simultaneous transmission policy
MOD SRSCFG: LocalCellId=0, AnSrsSimuTrans=BOOLEAN_TRUE;
//Setting the PUCCH resource adjustment switch
MOD CELLALGOSWITCH: LocalCellId=0, PucchAlgoSwitch=PucchSwitch-1;
## Deactivation Command Examples
//Disabling the UMTS and LTE Zero Bufferzone (LTE)
MOD ULZEROBUFFERZONE: LocalCellId=0, ZeroBufZoneSwitch=UMTS_LTE_ZERO_BUFFER_ZONE_SW-0;
5.4.3.3 Using the MAE-Deployment
●  Fast batch activation
This function can be batch activated using the Feature Operation and
Maintenance function of the MAE-Deployment. For detailed operations, see
the following section in the MAE-Deployment product documentation or
online help: MAE-Deployment Operation and Maintenance > MAE-
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.56

## Deployment Guidelines > Enhanced Feature Management > Feature
Operation and Maintenance.
●  Single/Batch configuration
This function can be activated for a single base station or a batch of base
stations on the MAE-Deployment. For detailed operations, see Feature
Configuration Using the MAE-Deployment.
## 5.4.4 Activation Verification
## Using Counters
If the counters listed in Table 5-5 all produce non-zero values, this function has
been activated.
Table 5-5 Counters for activation verification
Counter IDCounter Name
1526737760L.Traffic.ULShared.USER.Avg
1526748659L.Traffic.UmtsCore.USER.Avg

## Tracing Signaling Messages
Step 1Log in to the MAE-Access. Choose Monitor > Signaling Trace > Signaling Trace
Task Statistics. In the navigation tree of the displayed window, choose LTE >
## Application Layer > Uu Interface Trace.
Step 2Trace the RRC_MEAS_RPRT message on the Uu interface to check whether the UE
can report the RSCP of the UMTS cell periodically. The period is specified by the
ULZeroBufferZone.
ULZeroBufZoInterRatB1Timer parameter. If the RSCP of a
UMTS cell can be observed periodically, this function has been activated.
----End
## 5.4.5 Network Monitoring
This section describes how to monitor the network performance after this function
is enabled based on the uplink and downlink throughput of LTE cells, RTWP of
intra-frequency neighboring UMTS cells, and usage of UL shared spectrum.
●  Uplink and downlink throughput
–   Downlink throughput = L.Thrp.bits.DL/L.Thrp.Time.DL
–   Uplink throughput = L.Thrp.bits.UL/L.Thrp.Time.UL
●  RTWP of an intra-frequency neighboring UMTS cell
Observe the value of the VS.MeanRTWP counter.
●  Usage of the UL shared spectrum
–   Proportion of UEs in the UMTS preferential spectrum =
L.Traffic.UmtsCore.USER.Avg/L.Traffic.User.Avg
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.57

–   PRB usage of UMTS preferential spectrum =
L.ChMeas.PRB.UL.UmtsCore.Used.Avg/L.ChMeas.PRB.UL.Used.Avg
–   Proportion of UEs in the UL shared spectrum =
L.Traffic.ULShared.USER.Avg/L.Traffic.User.Avg
–   PRB usage of the UL shared spectrum =
L.ChMeas.PRB.UL.ULShared.Used.Avg/L.ChMeas.PRB.UL.Used.Avg
–   CCU throughput proportion = L.Thrp.bits.UL.CCU/L.Thrp.Time.UL.CCU
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
Description5 UMTS and LTE Zero Bufferzone (LTE FDD)
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.58

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
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description6 Parameters
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.59

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
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description7 Counters
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.60

## 8 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description8 Glossary
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.61

## 9 Reference Documents
●  Feature parameter description documents in RAN Feature Documentation
–Interference Rejection Combining
–Adaptive Interference Rejection
–GU 900 MHz Non-standard Frequency Spacing
–GU@5 MHz
## –HSUPA
–HSUPA Data Channel Interference Cancellation
–Independent Demodulation of Signals from Multiple Small Cell RRUs in
## One Cell
–Narrowband Interference Suppression
–Moving Speed-based Adaptive Demodulation
–Voice Coverage Improvement by Advanced Demodulation
–Extended Range
–TX Diversity and RX Diversity
–Multiple RRUs in One Cell
–UMTS Beamforming
–Inter-Dependence of BBU Uplink Resource
–Frequency Domain Equalization
–Dual Carriers over Narrowband
–UMTS and LTE Spectrum Sharing
–DC-HSDPA Shared with GSM
–UMTS and LTE Spectrum Sharing Based on DC-HSDPA
●  Feature parameter description documents in eRAN Feature Documentation
–UMTS and LTE Spectrum Sharing
–Compact Bandwidth (FDD)
–Physical Channel Resource Management
## –SFN
–Uplink Interference Cancellation (FDD)
–UL CoMP
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description9 Reference Documents
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.62

–NB-IoT Basics (FDD)
–eMTC
## –MIMO
–Virtual 4T4R (FDD)
–Carrier Aggregation
–ANR Management
## –ICIC
–LTE FDD and NR Uplink Spectrum Sharing
–GSM and LTE Spectrum Concurrency
–GSM and LTE Buffer Zone Optimization
–CDMA and LTE Zero Bufferzone
–UL Refarming Zero Bufferzone
–Flexible Bandwidth based on Overlap Carriers (FDD)
–Adaptive ICIC
–High Speed Mobility
–Super Combined Cell (FDD)
–LTE FDD and NR Spectrum Sharing
–Seamless Intra-Band Carrier Joining (FDD)
●3900 & 5900 Series Base Station LMT User Guide in 3900 & 5900 Series Base
## Station Product Documentation
SingleRAN
UMTS and LTE Zero Bufferzone Feature Parameter
## Description9 Reference Documents
Issue 02 (2024-06-21)Copyright © Huawei Technologies Co., Ltd.63