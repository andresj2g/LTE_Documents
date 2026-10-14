

eRAN
## Extended Cell Range Feature
## Parameter Description
## Issue06
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
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 06 (2023-09-14)..................................................................................................................................................1
1.2 eRAN18.1 05 (2023-04-23)..................................................................................................................................................1
1.3 eRAN18.1 04 (2023-02-01)..................................................................................................................................................2
1.4 eRAN18.1 03 (2022-07-29)..................................................................................................................................................2
1.5 eRAN18.1 02 (2022-04-27)..................................................................................................................................................2
1.6 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.7 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 2
2 About This Document.............................................................................................................4
2.1 General Statements................................................................................................................................................................ 4
2.2 Applicable RAT......................................................................................................................................................................... 4
2.3 Features in This Document.................................................................................................................................................. 5
3 General Principles....................................................................................................................6
3.1 Introduction...............................................................................................................................................................................6
3.2 Random Access Preamble Format.....................................................................................................................................7
4 Cell Radius Less Than 15 km................................................................................................ 9
4.1 Principles.................................................................................................................................................................................... 9
4.2 Network Analysis.....................................................................................................................................................................9
4.2.1 Benefits....................................................................................................................................................................................9
4.2.2 Impacts.................................................................................................................................................................................... 9
4.3 Requirements......................................................................................................................................................................... 10
4.3.1 Licenses................................................................................................................................................................................. 10
4.3.2 Software................................................................................................................................................................................10
4.3.3 Hardware..............................................................................................................................................................................10
4.3.4 Networking.......................................................................................................................................................................... 10
4.4 Operation and Maintenance.............................................................................................................................................16
4.4.1 Data Configuration........................................................................................................................................................... 16
4.4.1.1 Data Preparation............................................................................................................................................................ 16
4.4.1.2 Using MML Commands............................................................................................................................................... 17
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 18
4.4.2 Activation Verification......................................................................................................................................................18
4.4.3 Network Monitoring.........................................................................................................................................................19
eRAN
Extended Cell Range Feature Parameter DescriptionContents
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iii

5 Cell Radius Greater Than 15 km........................................................................................20
5.1 Principles.................................................................................................................................................................................. 20
5.2 Network Analysis.................................................................................................................................................................. 20
5.2.1 Benefits................................................................................................................................................................................. 20
5.2.2 Impacts..................................................................................................................................................................................20
5.3 Requirements......................................................................................................................................................................... 22
5.3.1 Licenses................................................................................................................................................................................. 22
5.3.2 Software................................................................................................................................................................................22
5.3.3 Hardware..............................................................................................................................................................................24
5.3.4 Networking.......................................................................................................................................................................... 25
5.4 Operation and Maintenance.............................................................................................................................................25
5.4.1 Data Configuration........................................................................................................................................................... 25
5.4.1.1 Data Preparation............................................................................................................................................................ 25
5.4.1.2 Using MML Commands............................................................................................................................................... 25
5.4.1.3 Using the MAE-Deployment...................................................................................................................................... 26
5.4.2 Activation Verification......................................................................................................................................................26
5.4.3 Network Monitoring.........................................................................................................................................................26
6 Cell Radius Greater Than 100 km (FDD).........................................................................27
6.1 Principles.................................................................................................................................................................................. 27
6.2 Network Analysis.................................................................................................................................................................. 27
6.2.1 Benefits................................................................................................................................................................................. 27
6.2.2 Impacts..................................................................................................................................................................................27
6.3 Requirements......................................................................................................................................................................... 29
6.3.1 Licenses................................................................................................................................................................................. 29
6.3.2 Software................................................................................................................................................................................30
6.3.3 Hardware..............................................................................................................................................................................33
6.3.4 Networking.......................................................................................................................................................................... 34
6.4 Operation and Maintenance.............................................................................................................................................34
6.4.1 Data Configuration........................................................................................................................................................... 34
6.4.1.1 Data Preparation............................................................................................................................................................ 34
6.4.1.2 Using MML Commands............................................................................................................................................... 34
6.4.1.3 Using the MAE-Deployment...................................................................................................................................... 34
6.4.2 Activation Verification......................................................................................................................................................34
6.4.3 Network Monitoring.........................................................................................................................................................35
7 Parameters..............................................................................................................................36
8 Counters.................................................................................................................................. 37
9 Glossary................................................................................................................................... 38
10 Reference Documents........................................................................................................ 39
eRAN
Extended Cell Range Feature Parameter DescriptionContents
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 06 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
●  Removed descriptions of optimization command examples from 4.4.1.2 Using
MML Commands, 6.4.1.2 Using MML Commands, and 5.4.1.2 Using MML
Commands and added descriptions of deactivation command examples in
these sections.
●  Revised descriptions in this document, which do not involve changes in
meanings and therefore are not detailed.
1.2 eRAN18.1 05 (2023-04-23)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
## Extended Cell Range Feature Parameter Description1 Change History
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.1

1.3 eRAN18.1 04 (2023-02-01)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 03 (2022-07-29)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 02 (2022-04-27)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
Added MML command examples. For details, see 5.4.1.2 Using MML Commands.
Optimized suggestions for configuring the preamble format based on the cell
radius. For details, see 3.2 Random Access Preamble Format.
1.6 eRAN18.1 01 (2022-03-08)
This issue does not include any changes.
1.7 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 04 (2021-09-29).
eRAN
## Extended Cell Range Feature Parameter Description1 Change History
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.2

## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
## Extended Cell Range Feature Parameter Description1 Change History
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.3

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
## Extended Cell Range Feature Parameter Description2 About This Document
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.4

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-002012Cell Access Radius up
to 15km
4 Cell Radius Less Than 15 km
LOFD-001009Extended Cell Access
## Radius
5 Cell Radius Greater Than 15 km
LOFD-081223Extended Cell Access
## Radius Beyond 100km
6 Cell Radius Greater Than 100 km (FDD)
eRAN
## Extended Cell Range Feature Parameter Description2 About This Document
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.5

## 3 General Principles
Nowadays, mobile communications networks cover most of the inland areas, but
rural areas, remote areas such as at sea, or in the desert, or grasslands, have poor
coverage due to site acquisition problems. It is difficult to find suitable site
locations at sea. Site deployment as usual in the desert or in grasslands (where
traffic is light) requires excessively huge investment.
In addition to this, extended coverage in these areas increases access delay and
requires enhanced coverage. In this situation, Huawei eNodeBs use the extended
cell range feature.
## 3.1 Introduction
Extended cell range helps operators increase the cell radius up to 200 km
theoretically, to expand cell coverage.
## NO TE
In this document, the cell radius is the theoretical cell radius with the corresponding
extended cell range feature enabled. The actual cell radius is the farthest location that the
radio signal covers away from the site center. The actual cell radius is typically less than the
theoretical one.
Table 3-1 lists the functions included in extended cell range and their application
scenarios.
Table 3-1 Functions included in extended cell range and their application scenarios
## Function
## Application Scenario
Cell radius less than 15 kmThe cell radius is less than or equal to 15 km.
Cell radius greater than 15 kmThe cell radius is in the range of (15 km, 100 km].
Cell radius greater than 100
km
The cell radius is in the range of (100 km, 200 km].

As shown in Figure 3-1, with the cell radius greater than 100 km function
enabled, the theoretical coverage area is the ring area B.
N (0 km < N ≤ 100 km)
eRAN
## Extended Cell Range Feature Parameter Description3 General Principles
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.6

and N + 100 km denote the nearest and farthest locations of the cell coverage
away from the site center. In this scenario, UEs that are located in area A cannot
access this cell. To provide services in area A, operators need to deploy other
common cells to provide the coverage.
Figure 3-1 Example of the coverage area of a cell with the cell radius greater than
100 km
## 3.2 Random Access Preamble Format
In accordance with section 5.7 in 3GPP TS 36.211 of Release 8 (2009 Q1), FDD
supports random access preamble formats 0 to 3 and TDD supports random
access preamble formats 0 to 4. A preamble format determines the cell coverage
and the time domain resources that can be used by a physical random access
channel (PRACH).
In a random access procedure, the eNodeB detects the preamble sequences
transmitted from a UE, estimates the round-trip delay (RTD), and completes the
synchronization for the UE.
RTD between the eNodeB and the UE increases with the cell radius, denoted by
## R.
It is calculated using the following formula:
Extended cell range uses different random access preamble formats to adapt to
different RTDs. The random access preamble format and cell radius are specified
by the Cell.PreambleFmt and Cell.CellRadius parameters, respectively.
In FDD, different preamble formats correspond to different cell radii and RTDs, as
listed in Table 3-2.
Table 3-2 Mapping between FDD random access preamble formats and cell radii
## Preamble Format
Cyclic Prefix (CP)
## Length T
## CP
## (μs)
Cell Radius (R) (km)Maximum RTD (μs)
## 0103.1R ≤ 14.596.7
## 1684.4R ≤ 77.3515.6
eRAN
## Extended Cell Range Feature Parameter Description3 General Principles
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.7

Preamble FormatCyclic Prefix (CP)
## Length T
## CP
## (μs)
Cell Radius (R) (km)Maximum RTD (μs)
## 2203.1R ≤ 29.5196.8
## 3684.4R ≤ 100666.7

## NO TE
Set the random access preamble format in FDD based on the cell radius as follows:
●   If the cell radius is less than or equal to 14.5 km, the recommended preamble format
is 0.
●   If the cell radius is greater than 14.5 km and less than or equal to 29.5 km, the
recommended preamble format is 1, 2, or 3.
●   If the cell radius is greater than 29.5 km and less than or equal to 77.3 km, the
recommended preamble format is 1 or 3.
●   If the cell radius is greater than 77.3 km, the recommended preamble format is 3.
eRAN
## Extended Cell Range Feature Parameter Description3 General Principles
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.8

4 Cell Radius Less Than 15 km
## 4.1 Principles
For details, see 3 General Principles.
## 4.2 Network Analysis
## 4.2.1 Benefits
Extended cell range increases cell coverage to meet communication requirements
in rural and remote areas such as at sea, in the desert, and in grasslands,
significantly decreasing the cost to deploy sites in such areas.
Extended cell range addresses the delay and fading caused by remote coverage. To
use extended cell range, operators need to obtain the actual coverage radius of a
cell. It is recommended that this function be enabled when the maximum
coverage distance of a cell is less than or equal to 15 km. This function is a basic
function. It is enabled by default and does not need to be activated or deactivated.
In high-speed or ultra-high-speed scenarios: In addition to the parameters
described in this document, other parameters may affect the access. For details
about the definition of high and low speeds and related parameter settings and
selection, see
## High Speed Mobility.
## 4.2.2 Impacts
## Network Impacts
## None
## Function Impacts
## None
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.9

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
The following base stations are compatible with this function:
3900 and 5900 series base stations (macro base stations)
## Boards
No requirements
RF Modules
No requirements
## 4.3.4 Networking
It is recommended that the following networking planning policies be used to
ensure better service rates at the cell edge with extended cell range:
●  Deploying distributed eNodeBs
A distributed eNodeB has two types of basic modules: the baseband unit
(BBU) and remote radio unit (RRU), which are deployed in a distributed
architecture. The BBU is installed in a cabinet, while RRUs are installed close
to the antenna system. The BBU and RRUs are connected using optical fibers.
Compared with macro eNodeBs under the same site conditions, distributed
eNodeBs can reduce feeder costs and loss for the antenna system and obtain
a gain in the range of 2.5 dB to 3 dB, increasing cell coverage. Figure 4-1
shows the installation scenarios of a macro eNodeB and distributed eNodeB.
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.10

Figure 4-1 Installation scenario comparison between a macro eNodeB and a
distributed eNodeB
●  Power amplifier
A Huawei eNodeB enhances downlink coverage by supporting up to 80 W TX
power.
●  Using tower-mounted amplifiers (TMAs)
A TMA is a low noise amplifier, which reduces the RX noise factor and
increases RX sensitivity of the eNodeB. On a live network, TMAs are installed
near RX antennas to improve RX performance.
If the equipment room is far from the antenna tower, resulting in a feeder
loss greater than 2.2 dB, TMAs can be installed to eliminate the impact of
feeder loss on RX sensitivity. TMAs improve RX performance. However, TMAs
also bring an insertion loss of about 0.5 dB to the downlink.
●  Antenna altitude
A valid antenna altitude consists of two parts: mountain altitude and altitude
from the antennas to the ground, as shown in Figure 4-2. Due to limitations
on the altitude of a tower or pole where the antennas are mounted, the
maximum altitude from the antennas to the ground is 70 m.
Figure 4-2 Example of a valid antenna altitude
On a live network, the antenna's effective altitude determines the cell
coverage. Therefore, when planning the antenna altitude, ensure that the
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.11

target cell coverage is within a line of sight (LOS). Non line of sight (NLOS)
areas may experience signal attenuation and poor cell coverage due to the
Earth's curvature.
For antenna altitude planned above the sea level, Huawei provides a
segmentation model to describe radio propagation on the sea, shown in
## Figure 4-3.
Figure 4-3 Segmentation model for radio propagation on the sea
As shown in the preceding figure:
## –
Ht denotes the site altitude above sea level.
–Hr denotes the UE altitude above sea level.
## –
d1 denotes the LOS path A on the sea.
–d2 denotes the LOS path B on the sea.
## –
Re denotes the Earth radius.
–d denotes path C on the sea, which is a shadow area with poor signal
quality due to the Earth's curvature, and therefore this path can be
ignored during network planning.
According to the Huawei segmentation model for radio propagation on the
sea, the following tables list the path losses calculated based on the site
altitudes, UE altitudes, and LOS distances above sea level at a site with center
frequencies of 800 MHz and 450 MHz.
–   800 MHz: Table 4-1 and Table 4-2
–   450 MHz: Table 4-3 and Table 4-4
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.12

## NO TE
The path losses with other center frequencies can be calculated based on that of 800
MHz or 450 MHz. Take the path loss calculation of a center frequency of 1800 MHz
based on the path loss with a center frequency of 800 MHz as an example. Delta
denotes the pass loss difference against 800 MHz. Delta = 20 x [log(1800) – log(800)].
The pass loss of a center frequency of 1800 MHz is equal to the sum of delta and the
pass loss of the center frequency of 800 MHz. The path loss of a center frequency of
1800 MHz can be calculated using the same method based on that of 450 MHz. The
path losses are for reference only.
Table 4-1 Path losses calculated based on site altitudes, UE altitudes (Hr = 2 m), and LOS distances
above sea level at a site with a center frequency of 800 MHz
Ht (m)d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 5029.2128.75.835.0136.8
## 6031.9129.65.837.8137.7
## 7034.5130.55.840.3138.3
## 8036.9131.35.842.7139.0
## 9039.1131.95.844.9139.5
## 10041.2132.55.847.1140.3
## 20058.3136.45.864.1143.6
## 30071.4138.75.877.2145.8
## 40082.5140.45.888.3147.6
## 50092.2141.75.898.0148.7

Table 4-2 Path losses calculated based on site altitudes, UE altitudes (Hr = 10 m), and LOS
distances above sea level at a site with a center frequency of 800 MHz
## Ht (m)
d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 5029.2128.613.042.2138.9
## 6031.9129.613.045.0139.7
## 7034.5130.513.047.5140.1
## 8036.9131.313.049.9140.8
## 9039.1131.913.052.2141.5
## 10041.2132.513.054.3141.9
## 20058.3136.413.071.3144.8
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.13

Ht (m)d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 30071.4138.713.084.5147.2
## 40082.5140.413.095.5148.5
## 50092.2141.613.0105.2149.5

Table 4-3 Path losses calculated based on site altitudes, UE altitudes (Hr = 2 m), and LOS distances
above sea level at a site with a center frequency of 450 MHz
Ht (m)d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 5029.2123.75.835.0131.8
## 6031.9124.65.837.8132.7
## 7034.5125.55.840.3133.3
## 8036.9126.35.842.7134.0
## 9039.1126.95.844.9134.4
## 10041.2127.55.847.1135.2
## 20058.3131.55.864.1138.6
## 30071.4133.75.877.2140.7
## 40082.5135.45.888.3142.5
## 50092.2136.75.898.0143.6
## 600101137.75.8106.8144.6
## 700109.1138.65.8114.9145.5
## 800116.7139.45.8122.5146.5
## 900123.7140.05.8129.5147.0
## 1100136.8141.25.8142.6148.3
## 1300148.7142.15.8154.5149.3

Table 4-4 Path losses calculated based on site altitudes, UE altitudes (Hr = 10 m), and LOS
distances above sea level at a site with a center frequency of 450 MHz
## Ht (m)
d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 5029.2123.613.042.2133.9
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.14

Ht (m)d1 (km)Path Loss
(dB)
d2 (km)d1+d2 (km)Path Loss
(dB)
## 6031.9124.613.045.0134.7
## 7034.5125.513.047.5135.1
## 8036.9126.313.049.9135.8
## 9039.1126.913.052.2136.4
## 10041.2127.513.054.3136.8
## 20058.3131.413.071.3139.8
## 30071.4133.713.084.5142.0
## 40082.5135.413.095.5143.4
## 50092.2136.613.0105.2144.4
## 600101137.713.0114.0145.4
## 700109.1138.513.0122.1146.2
## 800116.7139.313.0129.7147.2
## 900123.7140.013.0136.7147.6
## 1100136.8141.113.0149.8148.9
## 1300148.7142.113.0161.7149.8

When deploying extended cell range at sea, calculate the antenna altitude
based on the LOS distances (d1 + d2) listed in the preceding tables. When
deploying extended cell range in deserts or on grasslands, calculate the
antenna altitude based on the LOS distance d1 as listed in the preceding
tables.
If the antenna altitude of a site is too high, the antennas may receive radio
signals from too large an area, resulting in interference at the site. Calculate
the antenna altitude at an allowable height based on the distance between
the site and the target cell coverage to meet requirements for deploying
extended cell range on seas.
●  Site acquisition
The deployment of extended cell range requires good radio environment.
Therefore, the following requirements must be met for site acquisition:
–   There are no obvious obstacles in the target area to be covered by the
eNodeB. LOS areas are preferred.
–   The site altitude is as high as possible based on coverage requirements.
–   Extended cell coverage provided by the GERAN or UTRAN is preferentially
selected as the target cell coverage for the E-UTRAN.
–   Other requirements are the same as those for macro networks.
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.15

●  Channel power allocation
Channel power is allocated according to the configuration baseline of channel
power for macro networks.
●  Antenna selection
–   In most cases, it is recommended that 18 dBi antennas with a half-power
beamwidth of 65° be used.
–   When deployed at sea, the antennas are mounted as high as possible, in
order to resist the effect of the Earth's curvature. However, this may also
create coverage holes for areas near the antennas. In this scenario,
suitable antennas must be selected to avoid coverage holes. In addition,
antennas with smaller surface areas are recommended, to resist the
ocean wind, which also reduces the wind resistance on the tower or pole
where the antennas are mounted.
–   In open areas, vertically polarized antennas have better performance than
other types of polarized antennas. If wide cell coverage is required,
vertically polarized antennas are recommended.
–   Non-RET antennas can be used for scenarios that do not require tilt
adjustment. At a site with an extremely high altitude, antenna tilts can be
adjusted electronically or mechanically to ensure cell coverage for both
remote and local areas. RET is short for remote electrical tilt.
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Low-Speed Cell with Extended Cell Range
Table 4-5 describes the parameters used for function activation.
Table 4-5 Parameters used for activation
## Parameter
## Name
Parameter IDSetting Notes
Preamble formatCell.PreambleFmtSet this parameter to its recommended value.
Cell radiusCell.CellRadiusSet the parameter to a value greater than or
equal to the actual cell radius.
If the cell radius is greater than 100 km, take
the Cell.CellRadiusStartLocation parameter
setting into consideration when setting this
parameter. It is recommended that the value of
this parameter be equal to the sum of 100 km
and the value of the Cell.
CellRadiusStartLoca-
tion
parameter.
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.16

## Parameter
## Name
Parameter IDSetting Notes
## Cell Radius Start
## Location
Cell.CellRadiusStartLoca-
tion
This parameter value must be less than the
Cell.CellRadius parameter value. The value
difference between the Cell.CellRadius
parameter and this parameter must be less
than or equal to 100000. Set this parameter to
a value greater than 0 only when the cell radius
is greater than 100 km.
Standard RatioBBP.SRTThis parameter specifies the resource ratio for
LTE. Currently, only UBBP boards support this
parameter. If other baseband processing boards
are used, this parameter is invalid. If the cell
radius is in the range of 160 km to 200 km, set
this parameter based on the RAT planning
when adding a BBP.

High-Speed or Ultra-High-Speed Cell with Extended Cell Range
Table 4-6 describes the parameters used for function activation.
Table 4-6 Parameters used for activation
## Parameter
## Name
Parameter IDSetting Notes
Preamble formatCell.PreambleFmtSet this parameter to its recommended value.
Cell radiusCell.CellRadiusSet the parameter to a value greater than or
equal to the actual cell radius. The maximum
values for cells supporting high speed mobility
and ultra high speed mobility are 32800 and
17200, respectively.

For details about definitions of and parameters related to high-speed and ultra-
high-speed cells, see
## High Speed Mobility.
4.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Setting the preamble format to 0 as recommended if the cell radius is less than or equal to 14.5 km
MOD CELL: LocalCellId=0, PreambleFmt=0, CellRadius=10000;
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.17

## Deactivation Command Examples
MML commands are not required for deactivating this function. You can
determine whether to restore the settings of other parameters based on actual
network conditions.
4.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 4.4.2 Activation Verification
Step 1Check that the cell has been successfully activated, and then start tracing over the
Uu interface on the MAE-Access.
Step 2Run the MOD CELL command to configure a preamble format for the cell. The
cell will be automatically deactivated and then reactivated. Wait until the cell is
set up, and then check the decimal value of the IE prach-ConfigIndex in the first
RRC_SYS_INFO (SIB2) message over the Uu interface. For example, in the
following figure, the value of this IE is 3.
●  If the value of this IE is from 0 to 15, the Preamble format parameter has
been set to 0.
●  If the value of this IE is from 16 to 31, the Preamble format parameter has
been set to 1.
●  If the value of this IE is from 32 to 47, the Preamble format parameter has
been set to 2.
●  If the value of this IE is from 48 to 63, the Preamble format parameter has
been set to 3.
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.18

Figure 4-4 Example of querying the value of the IE prach-ConfigIndex
----End
## 4.4.3 Network Monitoring
Create signaling tracing tasks to monitor the performance. For details, see 4.4.2
## Activation Verification.
eRAN
Extended Cell Range Feature Parameter Description4 Cell Radius Less Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.19

5 Cell Radius Greater Than 15 km
## 5.1 Principles
For details, see 3 General Principles.
## 5.2 Network Analysis
## 5.2.1 Benefits
Extended cell range increases cell coverage to meet communication requirements
in rural and remote areas such as at sea, in the desert, and in grasslands,
significantly decreasing the cost to deploy sites in such areas.
Extended cell range addresses the delay and fading caused by remote coverage. To
use extended cell range, operators need to obtain the actual coverage radius of a
cell. It is recommended that this function be enabled when the maximum
coverage distance of a cell is in the interval of (15 km, 100 km]. Set the cell radius
based on the actual coverage radius (the cell radius can be greater than the actual
coverage radius) and configure the preamble format based on the cell radius.
In high-speed or ultra-high-speed scenarios: In addition to the parameters
described in this document, other parameters may affect the access. For details
about the definition of high and low speeds and related parameter settings and
selection, see
## High Speed Mobility.
## 5.2.2 Impacts
## Network Impacts
## ●  Coverage
The cell radius can be extended to up to 100 km.
●  Impact on network KPIs
The random access success rate increases in the coverage area.
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.20

## Function Impacts
RATFunction
## Name
Function SwitchReferenceDescription
FDDTTI bundlingTtiBundlingSwitch option
of the
CellAlgoSwitch.UlSchSwit
ch parameter
VoLTEExtended cell range leads
to the coverage limitation
in the uplink. TTI bundling
enhances PUSCH coverage
and increases the MCS
indexes in uplink weak
coverage areas, enhancing
uplink coverage and
improving coverage quality.
FDDUplink 2-
antenna
receive
diversity
NoneMIMOExtended cell range leads
to the coverage limitation
in the uplink. Uplink multi-
antenna technologies
enhance uplink coverage
and improve coverage
quality.
FDDUplink 4-
antenna
receive
diversity
NoneMIMOExtended cell range leads
to the coverage limitation
in the uplink. Uplink multi-
antenna technologies
enhance uplink coverage
and improve coverage
quality.
FDDPUSCH IRCCellAlgoSwitch.PuschIrcAl
goSwitch
MRC and
## IRC
## Receivers
Extended cell range leads
to the coverage limitation
in the uplink. Receiver
technologies are usually
used with uplink multi-
antenna technologies to
achieve a higher signal to
interference plus noise ratio
(SINR), enhancing uplink
coverage and improving
coverage quality.
FDDDownlink
## MU-MIMO
in TM9
4TxTM9MuMimoSwitch
option of the
CellAlgoSwitch.EmimoSwi
tch parameter
eMIMO
## (FDD)
In extended cell range
scenarios, TM9 is generally
not used.
In such scenarios, the
capacity is not high, the
user number is small, and
the traffic volume is low.
Therefore, the pairing rate
is low and the MU-MIMO
benefits are not apparent.
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.21

RATFunction
## Name
Function SwitchReferenceDescription
FDDWTTx MU-
## MIMO
Tm9FourLayerPairSwitch
option of the
CellAlgoExtSwitch.WttxM
uMimoSwitch parameter
WTTx MU-
## MIMO
## (FDD)
In extended cell range
scenarios, TM9 is generally
not used.
In such scenarios, the
capacity is not high, the
user number is small, and
the traffic volume is low.
Therefore, the pairing rate
is low and the MU-MIMO
benefits are not apparent.
FDDIntra-
eNodeB
## CSPC
CellCspcPara.IntraEnbCspc
## Sw
CSPCIntra-eNodeB CSPC is
suitable for densely
populated urban areas. It is
not recommended for cells
with radius greater than 15
km.

## 5.3 Requirements
## 5.3.1 Licenses
## RAT
Feature IDFeature NameModelSales Unit
FDDLOFD-001009Extended Cell
## Access Radius
LT1S00ECAR00per Cell

## 5.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.22

## Mutually Exclusive Functions
RATFunction
## Name
Function SwitchReferenceDescription
FDDCSPCCellCspcPara.CellCspcSwit
ch
CSPCThe larger the cell radius,
the lower the inter-cell
interference. Coordinated
scheduling-based power
control (CSPC) does not
apply to low-interference
scenarios.
FDDeCSPCCellCspcPara.CelleCspcSwi
tch
CSPCeCSPC requires that the
radius of each cell involved
should not exceed 15 km. If
the radius exceeds 15 km,
eCSPC does not take effect.
## FDDUL CRAUL_COORD_RES_ALLOC_S
WITCH option of the
UlCsAlgoPara.UlCsSw
parameter
## Uplink
## Coordinated
## Scheduling
When the cell radius is in
the interval of (15 km, 100
km], the traffic volume and
the interference are weak,
which is not a gain-yielding
scenario of uplink
coordinated scheduling.
## FDDUL CPCUL_COORD_PC_SWITCH
option of the
UlCsAlgoPara.UlCsSw
parameter
## Uplink
## Coordinated
## Scheduling
When the cell radius is in
the interval of (15 km, 100
km], the traffic volume and
the interference are weak,
which is not a gain-yielding
scenario of uplink
coordinated scheduling.
FDDStatic
## Multiple
## Beam
NoneMassive
## MIMO
## (FDD)
Massive MIMO does not
support a cell radius
greater than 15 km.
FDDDynamic
## Massive
## Beam
NoneMassive
## MIMO
## (FDD)
Massive MIMO does not
support a cell radius
greater than 15 km.
FDDIntelligent
beam
shaping
## MM_INTELLIGENT_BEAM_
SHAPING_SW option of
the
SectorSplitGroup.SectorSp
litSwitch
parameter
## Massive
## MIMO
## (FDD)
Massive MIMO does not
support a cell radius
greater than 15 km.
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.23

RATFunction
## Name
Function SwitchReferenceDescription
FDDDL CoMP
with TM10
HomNet:
FDDHomNetDlCompS-
witch option of the
CellAlgoSwitch.DlCompSw
itch parameter
HetNet:
FDDHetNetDlCompSwitch
option of the
CellAlgoSwitch.
DlCompSw
itch
parameter
DL CoMP
## (FDD)
In DL CoMP, UEs need to
receive data from different
cells simultaneously.
Therefore, DL CoMP does
not apply to extended
coverage scenarios.
FDDUplink joint
interference
managemen
t
## UL_JOINT_INTRF_SUPPRES
S_SW option of the
UlInterfSuppressCfg.UlJoi
ntIntrfManagementSw
parameter
## Interference
## Detection
and
## Suppression
Uplink joint interference
management requires that
the radius of each cell
involved should not exceed
15 km. If the radius exceeds
15 km, uplink joint
interference management
does not take effect.
FDDStatic
## Multiple
## Beam
None3D
## Beamformin
g (FDD)
The cell radius greater than
15 km function does not
work at passive ports on
AAUs.
FDDDynamic
## Massive
## Beam
None3D
## Beamformin
g (FDD)
## None
FDDStatic
## Multiple
## Beam
NoneSmart 8T8R
## (FDD)
## None
FDDDynamic
## Massive
## Beam
NoneSmart 8T8R
## (FDD)
## None

## 5.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in
## 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
The following base stations are compatible with this function:
3900 and 5900 series base stations (macro base stations)
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.24

## Boards
No requirements
RF Modules
No requirements
## 5.3.4 Networking
For details, see 4.3.4 Networking.
5.4 Operation and Maintenance
## 5.4.1 Data Configuration
## 5.4.1.1 Data Preparation
For details, see 4.4.1.1 Data Preparation.
5.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
Before using MML commands, refer to 5.3.2 Software and 5.2.2 Impacts and
complete the parameter configurations for related functions based on the impact,
dependency, and mutually exclusive relationships between the functions, as well
as the actual network scenario.
●  Setting the preamble format to 1, 2, or 3 as recommended if the cell radius is
greater than 14.5 km and less than or equal to 29.5 km.
MOD CELL: LocalCellId=0, PreambleFmt=2, CellRadius=17000;
●  Setting the preamble format to 1 or 3 as recommended if the cell radius is
greater than 29.5 km and less than or equal to 77.3 km.
MOD CELL: LocalCellId=0, PreambleFmt=1, CellRadius=30000;
●  Setting the preamble format to 3 as recommended if the cell radius is greater
than 77.3 km.
MOD CELL: LocalCellId=0, PreambleFmt=3, CellRadius=90000;
## Deactivation Command Examples
MML commands are not required for deactivating this function. You can
determine whether to restore the settings of other parameters based on actual
network conditions.
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.25

5.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 5.4.2 Activation Verification
## Verifying Preamble Format Configuration
For details, see 4.4.2 Activation Verification.
Observing the Extended Cell Access Radius Feature
Step 1On the MAE-Access, run the LST CELL command and check the value of Cell
radius. If it is not greater than 15000, the Extended Cell Access Radius feature has
not taken effect. If it is greater than 15000, write it down and proceed to the next
step.
Step 2On the MAE-Access, run the DSP LICINFO command and check the Actual Used
value corresponding to Extended Cell Access Radius(per Cell)(FDD). If the value is
0, the feature has not taken effect. If the value is greater than 0, write it down
and proceed to the next step.
Step 3On the MAE-Access, run the MOD CELL command with the Cell radius parameter
set to 10000. If necessary, change the value of the Preamble format parameter.
Step 4Run the DSP CELL command and verify that the cell has been successfully
activated. Run the DSP LICINFO command and check the value of Actual Used
corresponding to Extended Cell Access Radius(per Cell)(FDD).
●  If this value equals that obtained in Step 2, the feature had not been
activated before you modified Cell radius.
●  If this value equals that obtained in Step 2 minus 1, the feature had been
activated before you modified Cell radius. Write down this value and proceed
to the next step.
Step 5On the MAE-Access, run the MOD CELL command with Cell radius set to the
value obtained in Step 1.
Step 6Run the DSP CELL command and verify that the cell has been successfully
activated. Run the DSP LICINFO command and check the value of Actual Used
corresponding to Extended Cell Access Radius(per Cell)(FDD). If this value equals
that obtained in Step 4 plus 1, the feature has already been activated.
----End
## 5.4.3 Network Monitoring
Create signaling tracing tasks to monitor the performance. For details, see 5.4.2
## Activation Verification.
eRAN
Extended Cell Range Feature Parameter Description5 Cell Radius Greater Than 15 km
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.26

6 Cell Radius Greater Than 100 km (FDD)
## 6.1 Principles
For details, see 3 General Principles.
## 6.2 Network Analysis
## 6.2.1 Benefits
Extended cell range increases cell coverage to meet communication requirements
in rural and remote areas such as at sea, in the desert, and in grasslands,
significantly decreasing the cost to deploy sites in such areas.
Extended cell range addresses the delay and fading caused by remote coverage. To
use extended cell range, operators need to obtain the actual coverage radius of a
cell. It is recommended that this function be enabled when the maximum
coverage distance of a cell is greater than 100 km.
In high-speed or ultra-high-speed scenarios: In addition to the parameters
described in this document, other parameters may affect the access. For details
about the definition of high and low speeds and related parameter settings and
selection, see
## High Speed Mobility.
## 6.2.2 Impacts
## Network Impacts
The cell radius can be extended to up to 200 km.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.27

## Function Impacts
## Function
## Name
Function SwitchReferenceDescription
TTI bundlingTtiBundlingSwitch option of
the
CellAlgoSwitch.UlSchSwitch
parameter
VoLTEExtended cell range leads to
the coverage limitation in the
uplink. TTI bundling enhances
PUSCH coverage and increases
the MCS indexes in uplink
weak coverage areas,
enhancing uplink coverage and
improving coverage quality.
## Uplink 2-
antenna
receive
diversity
NoneMIMOExtended cell range leads to
the coverage limitation in the
uplink. Uplink multi-antenna
technologies enhance uplink
coverage and improve
coverage quality.
## Uplink 4-
antenna
receive
diversity
NoneMIMOExtended cell range leads to
the coverage limitation in the
uplink. Uplink multi-antenna
technologies enhance uplink
coverage and improve
coverage quality.
PUSCH IRCCellAlgoSwitch.PuschIrcAlgoS
witch
MRC and IRC
## Receivers
Extended cell range leads to
the coverage limitation in the
uplink. Receiver technologies
are usually used with uplink
multi-antenna technologies to
achieve a higher signal to
interference plus noise ratio
(SINR), enhancing uplink
coverage and improving
coverage quality.
## Downlink 4x2
## MIMO
NoneMIMOCell radius greater than 100
km does not support channel
calibration. Therefore, cell
radius greater than 100 km
and closed-loop 4x2 MIMO
cannot be activated at the
same time. Otherwise, the
downlink performance
deteriorates. However, the cell
radius greater than 100 km
and open-loop 4x2 MIMO can
be activated at the same time.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.28

## Function
## Name
Function SwitchReferenceDescription
## Downlink 4x4
## MIMO
NoneMIMOCell radius greater than 100
km does not support channel
calibration. Therefore, cell
radius greater than 100 km
and closed-loop 4x4 MIMO
cannot be activated at the
same time. Otherwise, the
downlink performance
deteriorates. However, the cell
radius greater than 100 km
and open-loop 4x4 MIMO can
be activated at the same time.
WTTx MU-
## MIMO
Tm9FourLayerPairSwitch
option of the
CellAlgoExtSwitch.WttxMuMi
moSwitch parameter
WTTx MU-
## MIMO (FDD)
In extended cell range
scenarios, TM9 is generally not
used.
In such scenarios, the capacity
is not high, the user number is
small, and the traffic volume is
low. Therefore, the pairing rate
is low and the MU-MIMO
benefits are not apparent.
Smart carrier
selection
based on
virtual grids
## SMART_CARRIER_SELECTION
_SW option of the
MultiCarrUnifiedSch.MultiCar
rierUnifiedSchSw parameter
## Multi-carrier
## Unified
## Scheduling
Virtual grid models cannot be
built for cells whose radius is
greater than 100 km.
Intra-eNodeB
## CSPC
CellCspcPara.IntraEnbCspcSwCSPCIntra-eNodeB CSPC is suitable
for densely populated urban
areas. It is not recommended
for cells with radius greater
than 100 km.

## 6.3 Requirements
## 6.3.1 Licenses
Feature ID
Feature NameModelSales Unit
LOFD-081223Extended Cell Access
## Radius Beyond 100km
LT1S0ECARB00Per Cell

eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.29

## 6.3.2 Software
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## Function
## Name
Function SwitchReferenceDescription
UL CoMP cellUlJointReceptionSwitch
option of the
CellAlgoSwitch.UplinkCompS
witch parameter
UL CoMPIt is recommended that the
inter-site distance for uplink
coordinated multipoint
reception (UL CoMP) be less
than or equal to 1 km. In
extended cell range scenarios,
UL CoMP is not supported
because the inter-site distance
is much greater than 1 km.
PSIC receiverMumimoPuschPsicSwitch
option of the
CellAlgoSwitch.PsicSwitch
parameter
PSIC ReceiverThis function is not applicable
when the cell radius exceeds
100 km, and therefore it is not
supported.
## Static
## Multiple
## Beam
None3D
## Beamforming
## (FDD)
This function is not supported
because downlink 4x4 MIMO is
not supported when the cell
radius exceeds 100 km.
## Dynamic
## Massive Beam
None3D
## Beamforming
## (FDD)
This function is not supported
because downlink 4x4 MIMO is
not supported when the cell
radius exceeds 100 km.
## Static
## Multiple
## Beam
NoneMassive
## MIMO (FDD)
In massive MIMO scenarios,
the Cell.CellRadius parameter
cannot be set to a value
greater than 15 km.
## Dynamic
## Massive Beam
NoneMassive
## MIMO (FDD)
In massive MIMO scenarios,
the Cell.CellRadius parameter
cannot be set to a value
greater than 15 km.
## Intelligent
beam shaping
## MM_INTELLIGENT_BEAM_SH
APING_SW option of the
SectorSplitGroup.SectorSplitS
witch
parameter
## Massive
## MIMO (FDD)
In massive MIMO scenarios,
the Cell.CellRadius parameter
cannot be set to a value
greater than 15 km.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.30

## Function
## Name
Function SwitchReferenceDescription
High speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
In accordance with 3GPP
specifications, high speed
mobility is not supported when
the cell radius exceeds 100 km.
Ultra high
speed
mobility
Cell.HighSpeedFlagHigh Speed
## Mobility
In accordance with 3GPP
specifications, ultra high speed
mobility is not supported when
the cell radius exceeds 100 km.
CSPCCellCspcPara.CellCspcSwitchCSPCThis function is not applicable
when the cell radius exceeds
100 km, and therefore it is not
supported.
eCSPCCellCspcPara.CelleCspcSwitchCSPCeCSPC requires that the radius
of each cell involved should
not exceed 15 km. If the radius
exceeds 15 km, eCSPC does
not take effect.
SFN cellCell.MultiRruCellModeSFNMulti-RRU combination cells
are not supported when the
cell radius exceeds 100 km.
## Super
combined cell
SuperCombCellSwitch option
of the
CellAlgoSwitch.SfnAlgoSwitc
h parameter
## Super
## Combined Cell
## (FDD)
Multi-RRU combination cells
are not supported when the
cell radius exceeds 100 km.
## Carrier
aggregation
NoneCarrier
## Aggregation
CA-related features are not
supported when the cell radius
exceeds 100 km.
## UL CRAUL_COORD_RES_ALLOC_SWIT
CH option of the
UlCsAlgoPara.UlCsSw
parameter
## Uplink
## Coordinated
## Scheduling
When the cell radius exceeds
100 km, the traffic volume and
the interference are small,
which is not a gain-yielding
scenario of uplink coordinated
scheduling.
## UL CPCUL_COORD_PC_SWITCH
option of the
UlCsAlgoPara.UlCsSw
parameter
## Uplink
## Coordinated
## Scheduling
When the cell radius exceeds
100 km, the traffic volume and
the interference are small,
which is not a gain-yielding
scenario of uplink coordinated
scheduling.
eMTC
introduction
EMTC_SWITCH option of the
CellEmtcAlgo.EmtcAlgoSwitc
h parameter
eMTCCell radius greater than 100
km is mutually exclusive with
eMTC introduction.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.31

## Function
## Name
Function SwitchReferenceDescription
Inter-eNodeB
VoLTE CoMP
UlVoiceJROverRelaxedBHSw
option of the
ENodeBAlgoSwitch.OverBBUs
Switch parameter
UL CoMPCell radius greater than 100
km is mutually exclusive with
inter-eNodeB VoLTE CoMP.
NB-IoT
network
deployment
Prb.DeployModeNB-IoT Basics
## (FDD)
An NB-IoT network can be
deployed in standalone, LTE
guard band, or LTE in-band
mode. When an NB-IoT and an
LTE FDD cell are served by the
same RRU, the FDD cell radius
cannot exceed 100 km.
Turbo receiverCellAlgoSwitch.TurboReceive
rSwitch
## Turbo
## Receiver
When the cell radius exceeds
100 km, the processing by the
turbo receiver is affected by
delay and therefore the turbo
receiver cannot work in this
scenario.
## Superior
uplink
coverage
CellAlgoExtSwitch.UlCoverag
eEnhancementSw
## Superior
## Uplink
## Coverage
## (FDD)
Cell radius greater than 100
km is mutually exclusive with
superior uplink coverage.
LTE FDD and
NR Flash
## Dynamic
## Spectrum
## Sharing
SpectrumCloud.SpectrumClo
udSwitch set to
## LTE_NR_SPECTRUM_SHR
LTE FDD and
NR Spectrum
## Sharing
Cell radius greater than 100
km is mutually exclusive with
LTE FDD and NR Flash
## Dynamic Spectrum Sharing.
Hybrid DSS
Based on
## Asymmetric
## Bandwidth
SpectrumCloud.SpectrumClo
udSwitch set to
LTE_NR_SPECTRUM_SHR and
## LNR_SPECTRUM_SHR_ASYM_
SW option of the
SpectrumCloud.
SpectrumClo
udEnhSwitch parameter
selected
LTE FDD and
NR Spectrum
## Sharing
Cell radius greater than 100
km is mutually exclusive with
Hybrid DSS Based on
## Asymmetric Bandwidth.
## Static
## Multiple
## Beam
NoneSmart 8T8R
## (FDD)
## None
## Dynamic
## Massive Beam
NoneSmart 8T8R
## (FDD)
## None

eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.32

## 6.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
The following base stations are compatible with this function:
3900 and 5900 series base stations (macro base stations)
## Boards
LTE-only UBBPd, LTE-only UBBPe, LTE-only UBBPei, and LTE-only UBBPg boards
support this function. Table 6-1 lists the configuration specifications specific to
LTE-only UBBPd, LTE-only UBBPe, and LTE-only UBBPg boards.
Table 6-1 Board configuration specifications
ItemLTE-only UBBPd BoardsLTE-only UBBPg or LTE-
only UBBPe Boards
Maximum value of
Cell.CellRadiusStartLocation
## 60000100000
Maximum value of
Cell.CellRadius
## 160000200000
Maximum length of the optical
fiber connecting the BBP and RF
unit
40 km20 km

## NO TE
●  One BBP can be configured with only one cell with a cell radius greater than 100 km.
●  If the cell radius is in the range of 160 km to 200 km, set the BBP.
SRT parameter to
FDD_ENHANCE when adding a BBP.
RF Modules
RF modules except the following models support this function:
## ●  RRU: RRU3201/RRU3203/RRU3220/RRU3220E/RRU3222/RRU3908/RRU3808/
RRU3230E/RRU3930E/RRU5301 (1.4 GHz)/RRU3821E/RRU5935E/RRU5336E
●  RFU: LRFU and MRFU
●  AAU: none
## NO TE
The Cell.CellRadiusStartLocation parameter must be set to the same value for cells served
by an RRU.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.33

## 6.3.4 Networking
For details, see 4.3.4 Networking.
6.4 Operation and Maintenance
## 6.4.1 Data Configuration
## 6.4.1.1 Data Preparation
For details, see 4.4.1.1 Data Preparation.
6.4.1.2 Using MML Commands
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
//Setting the preamble format to 3 as recommended if the cell radius is greater than 100 km
MOD CELL: LocalCellId=0, PreambleFmt=3, CellRadius=120000, CellRadiusStartLocation=20000;
//Setting the resource ratio for an RAT based on the planning
## MOD BBP: CN=0, SRN=0, SN=4, TYPE=UBBP, WM=FDD, SRT=FDD_ENHANCE;
## Deactivation Command Examples
MML commands are not required for deactivating this function. You can
determine whether to restore the settings of other parameters based on actual
network conditions.
6.4.1.3 Using the MAE-Deployment
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
## 6.4.2 Activation Verification
## Verifying Preamble Format Configuration
For details, see 4.4.2 Activation Verification.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.34

Observing the Extended Cell Access Radius Beyond 100km Feature
Step 1On the MAE-Access, run the LST CELL command and check the values of Cell
radius and Cell Radius Start Location. If Cell radius is not greater than 100000
and Cell Radius Start Location is 0, the feature has not taken effect. If Cell
radius is greater than 100000 and Cell Radius Start Location is greater than 0,
write them down and proceed to the next step.
Step 2On the MAE-Access, run the DSP LICINFO command and check the Actual Used
value corresponding to Extended Cell Access Radius Beyond 100 km (per Cell)
(FDD). If the value is 0, the feature has not taken effect. If the value is greater
than 0, write it down and proceed to the next step.
Step 3On the MAE-Access, run the MOD CELL command with Cell radius and Cell
Radius Start Location set to 10000 and 0, respectively. If necessary, change the
value of Preamble format.
Step 4Run the DSP CELL command and verify that the cell has been successfully
activated. Run the DSP LICINFO command and check the value of Actual Used
corresponding to Extended Cell Access Radius Beyond 100 km (per Cell)(FDD).
●  If this value equals that obtained in Step 2, the feature had not been
activated before you modified Cell radius and Cell Radius Start Location.
●  If this value equals that obtained in Step 2 minus 1, the feature had been
activated before you modified Cell radius and Cell Radius Start Location.
Write down these values and proceed to the next step.
Step 5On the MAE-Access, run the MOD CELL command with Cell radius and Cell
Radius Start Location set to the values obtained in Step 1.
Step 6Run the DSP CELL command and verify that the cell has been successfully
activated. Run the DSP LICINFO command and check the value of Actual Used
corresponding to Extended Cell Access Radius Beyond 100 km (per Cell)(FDD).
If this value equals that obtained in Step 4 plus 1, the feature has already been
activated.
----End
## 6.4.3 Network Monitoring
Create signaling tracing tasks to monitor the performance. For details, see 6.4.2
## Activation Verification.
eRAN
Extended Cell Range Feature Parameter Description6 Cell Radius Greater Than 100 km (FDD)
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.35

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
## Extended Cell Range Feature Parameter Description7 Parameters
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.36

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
## Extended Cell Range Feature Parameter Description8 Counters
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.37

## 9 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
## Extended Cell Range Feature Parameter Description9 Glossary
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.38

## 10 Reference Documents
-  3GPP TS 36.211: "Physical channels and modulation"
## 2.
## High Speed Mobility
3.Extended CP
## 4.SFN
5.UL CoMP
6.PSIC Receiver
7.3D Beamforming (FDD)
8.High Speed Mobility
## 9.CSPC
10.Super Combined Cell (FDD)
11.Carrier Aggregation
12.Uplink Coordinated Scheduling
13.eMTC
14.NB-IoT Basics (FDD)
15.VoLTE
## 16.MIMO
17.MRC and IRC Receivers
18.Massive MIMO (FDD)
19.DL CoMP (FDD)
20.eMIMO (FDD)
21.Turbo Receiver
22.LTE FDD and NR Spectrum Sharing
23.WTTx MU-MIMO (FDD)
24.Smart 8T8R (FDD)
25.Multi-carrier Unified Scheduling
26.Interference Detection and Suppression
27.Superior Uplink Coverage (FDD)
eRAN
## Extended Cell Range Feature Parameter Description10 Reference Documents
Issue 06 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.39