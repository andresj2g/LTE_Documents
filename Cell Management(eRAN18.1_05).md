

eRAN
## Cell Management Feature
## Parameter Description
## Issue05
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
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN18.1 05 (2023-09-14)..................................................................................................................................................1
1.2 eRAN18.1 04 (2022-11-15)..................................................................................................................................................1
1.3 eRAN18.1 03 (2022-08-25)..................................................................................................................................................2
1.4 eRAN18.1 02 (2022-04-27)..................................................................................................................................................2
1.5 eRAN18.1 01 (2022-03-08)..................................................................................................................................................2
1.6 eRAN18.1 Draft A (2021-12-30)........................................................................................................................................ 3
2 About This Document.............................................................................................................4
2.1 General Statements................................................................................................................................................................ 4
2.2 Applicable RAT......................................................................................................................................................................... 4
2.3 Features in This Document.................................................................................................................................................. 5
3 Cell Management....................................................................................................................6
3.1 Principles.................................................................................................................................................................................... 6
3.1.1 Definitions.............................................................................................................................................................................. 6
3.1.2 Related Concepts................................................................................................................................................................. 6
3.1.2.1 Cell.........................................................................................................................................................................................7
3.1.2.2 Sector....................................................................................................................................................................................7
3.1.2.3 Sector Equipment............................................................................................................................................................. 8
3.1.2.4 RF Equipment.................................................................................................................................................................... 8
3.1.2.5 Baseband Equipment...................................................................................................................................................... 9
3.1.2.6 Cell-specific Sector Equipment and Cell-specific Sector Equipment Group.................................................9
3.1.3 Typical Scenarios................................................................................................................................................................10
3.1.3.1 Common Cell................................................................................................................................................................... 10
3.1.3.2 Split-RRU/RFU-Sector Cell.......................................................................................................................................... 10
3.1.3.3 Combined-RRU/RFU-Sector Cell............................................................................................................................... 11
3.1.3.4 Multi-Sector Cell.............................................................................................................................................................11
3.1.3.5 Cells in a Multi-Carrier Sector................................................................................................................................... 13
3.1.3.6 Downlink-only Cell (FDD)........................................................................................................................................... 14
3.1.4 Cell-related Parameters...................................................................................................................................................14
3.1.4.1 Frequency Band.............................................................................................................................................................. 14
3.1.4.2 Cell Bandwidth................................................................................................................................................................17
3.1.4.3 Maximum Transmit Power of a Cell........................................................................................................................17
eRAN
Cell Management Feature Parameter DescriptionContents
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iii

3.2 Network Analysis.................................................................................................................................................................. 21
3.2.1 Benefits................................................................................................................................................................................. 21
3.2.2 Impacts..................................................................................................................................................................................21
3.3 Requirements......................................................................................................................................................................... 22
3.3.1 Licenses................................................................................................................................................................................. 22
3.3.2 Software................................................................................................................................................................................22
3.3.3 Hardware..............................................................................................................................................................................23
3.3.4 Others (FDD)...................................................................................................................................................................... 25
3.4 Operation and Maintenance.............................................................................................................................................26
3.4.1 Data Configuration (FDD)..............................................................................................................................................26
3.4.1.1 Data Preparation............................................................................................................................................................ 26
3.4.1.2 Using MML Commands............................................................................................................................................... 35
3.4.1.3 Using the MAE-Deployment...................................................................................................................................... 39
3.4.2 Activation Observation.................................................................................................................................................... 39
3.4.3 Possible Issues.................................................................................................................................................................... 40
4 Parameters..............................................................................................................................41
5 Counters.................................................................................................................................. 42
6 Glossary................................................................................................................................... 43
7 Reference Documents...........................................................................................................44
eRAN
Cell Management Feature Parameter DescriptionContents
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN18.1 05 (2023-09-14)
This issue includes the following changes.
## Technical Changes
## Change Description
Parameter ChangeBase Station Model
Added support for splitting by
the RRU5862 and RRU5865.
For details, see 3.1.3.2 Split-
RRU/RFU-Sector Cell.
None3900 and 5900
series base stations
(macro base
stations)

## Editorial Changes
Revised descriptions in this document.
1.2 eRAN18.1 04 (2022-11-15)
This issue includes the following changes.
eRAN
## Cell Management Feature Parameter Description1 Change History
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.1

## Technical Changes
Change DescriptionParameter ChangeBase Station Model
NoneNoneNone

## Editorial Changes
Revised descriptions in this document.
1.3 eRAN18.1 03 (2022-08-25)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.4 eRAN18.1 02 (2022-04-27)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
1.5 eRAN18.1 01 (2022-03-08)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
## Cell Management Feature Parameter Description1 Change History
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.2

1.6 eRAN18.1 Draft A (2021-12-30)
This issue introduces the following changes to eRAN17.1 02 (2021-04-30).
## Technical Changes
## None
## Editorial Changes
Revised descriptions in this document.
eRAN
## Cell Management Feature Parameter Description1 Change History
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.3

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
## Cell Management Feature Parameter Description2 About This Document
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.4

2.3 Features in This Document
This document describes the following FDD features.
Feature IDFeature NameChapter/Section
LBFD-001003Scalable Bandwidth3 Cell Management
LBFD-131106Multi Carrier3 Cell Management
eRAN
## Cell Management Feature Parameter Description2 About This Document
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.5

## 3 Cell Management
## 3.1 Principles
## 3.1.1 Definitions
Cell management refers to management of wireless communications resources by
establishing cells and configuring related parameters.
## 3.1.2 Related Concepts
The concepts related to a cell include the cell itself, sector, sector equipment, RF
equipment, baseband equipment, and cell-specific sector equipment. Figure 3-1
shows a mapping example.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.6

Figure 3-1 Concepts related to a cell
## 3.1.2.1 Cell
A cell is an area where radio communications services are provided. It is the
fundamental unit of a radio network. A cell is added by running the ADD CELL
command. Coverage of the entire radio network is provided by cells.
## 3.1.2.2 Sector
A sector is a coverage area of an antenna. It is added using the ADD SECTOR
command. Each sector uses one or more radio carriers to provide coverage.
## NO TE
●  For a co-MPT base station, if services of different RATs are carried on the same transmit
channel (that is, multi-standard radio), it is recommended that all the RATs use the
same SECTOR MO.
●  For a LampSite base station, it is recommended that a sector be planned for each pRRU/
hRRU.
A sector can be omnidirectional or directional, depending on the antenna type.
## Sector Type
DefinitionBenefit
## Omnidirectio
nal
An omnidirectional sector uses
an omnidirectional antenna to
provide a 360° circular coverage
area with the antenna as the
coverage center.
In light-traffic areas, the
deployment of
omnidirectional sectors
reduces the cost of antenna
equipment.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.7

Sector TypeDefinitionBenefit
DirectionalA directional sector uses a
directional antenna for coverage.
● If three sectors are configured
for an eNodeB, each
directional antenna covers a
120° sector.
● If six sectors are configured
for an eNodeB, each
directional antenna covers a
60° sector.
The actual azimuth of each
antenna is slightly greater than
the theoretical value so that
adjacent sectors overlap each
other and provide seamless
coverage.
● In heavy-traffic areas, the
deployment of directional
sectors supports large
traffic volume.
● Directional sectors
support more flexible
area and sector planning.

## 3.1.2.3 Sector Equipment
Sector equipment is a set of antennas used for the same sector. A sector is linked
to a set of antennas comprising a specific piece of sector equipment by running
the ADD SECTOR or ADD SECTOREQM command.
## NO TE
For a co-MPT base station, if services of different RATs are carried on the same transmit
channel, configure the SECTOREQM MO by mode.
3.1.2.4 RF Equipment
For a macro or LampSite eNodeB, radio frequency (RF) equipment is a set of RF
processing units, including RRUs, RFUs, pRRUs, hRRUs, and AAUs. RF equipment is
added and associated with CPRI ports on baseband processing units (BBPs) by
running the ADD RRU and ADD RRUCHAIN commands, respectively.
For a micro eNodeB, RF equipment refers to its RF processing units. RRUs need to
be added only when they need to be remotely deployed.
In FDD, if the Description field contains V3 in the output of the DSP
BRDMFRINFO command, the following requirements must be met for the
corresponding RRU:
●  For a 1T1R, 1T2R, or 2T2R sector served by a 2T4R or 4T4R RRU, antennas in
the same group must be used. (Antennas A and C are assigned as one group,
and antennas B and D are assigned as the other group.)
●  For a 2T4R sector, transmit antennas must be in two different groups.
xTyR means x transmit channels and y receive channels.
When the channels of RF units are faulty and disabled, the number of antennas in
use decreases and the cells are reestablished. You can run the DSP TXBRANCH
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.8

command to query the faulty RF channels. The number of antennas serving FDD
cells decreases in the sequence of 4 > 2 > 1.
## 3.1.2.5 Baseband Equipment
A piece of baseband equipment consists of one or more BBPs.
For a macro or LampSite eNodeB, a BBP is added by running the ADD BRD
command. It can be added to a piece of baseband equipment by running the ADD
BASEBANDEQM command.
For a micro eNodeB, there is no need to add BBPs or baseband equipment.
In LTE eNodeBs, the baseband equipment is used for both uplink and downlink
transmissions.
3.1.2.6 Cell-specific Sector Equipment and Cell-specific Sector Equipment
## Group
When binding sector equipment to a cell, you can specify the sector equipment
and the baseband equipment for the cell at the same time.
●  For a macro eNodeB, the sector equipment and serving BBPs specific to a cell
are added by running the ADD EUCELLSECTOREQM command. If no
baseband equipment is specified for a cell, the BBP directly connected to the
RF equipment serving the cell is used by default.
●  For a LampSite eNodeB, the sector equipment group of a cell is added by
running the ADD EUSECTOREQMGROUP command. Then, sector equipment
is added to the sector equipment group by running the ADD
EUSECTOREQMID2GROUP command.
●  In scenarios without macro-micro co-siting: The cell-specific sector equipment
does not need to be bound to BBPs. The eNodeB will select an appropriate
BBP for the sector equipment. If the cell-specific sector equipment needs to be
bound to the BBP in a specified slot, you need to add a piece of baseband
equipment for the sector equipment. Ensure that each piece of baseband
equipment is bound to one BBP and that a BBP is bound only to one piece of
baseband equipment.
●  In macro-micro co-siting scenarios: LampSite and macro cells cannot be
established on the same BBP. When both a LampSite cell and a macro cell are
to be established on the same eNodeB, different baseband resources need to
be configured for the two types of cells if baseband resources are configured
manually. Relevant MML commands are as follows:
–ADD BASEBANDEQM: This command is used to configure a piece of
baseband equipment. One piece of baseband equipment includes one or
more BBPs.
–ADD EUCELLSECTOREQM: This command is used to bind a macro cell to
a piece of baseband equipment.
–ADD EUSECTOREQMGROUP: This command is used to bind a LampSite
cell to a piece of baseband equipment.
## NO TE
Macro-micro co-siting scenarios refer to scenarios where both macro cells (RRU/RFU-
serving cells) and LampSite cells (MPRU aggregation cells) exist on the live network.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.9

## 3.1.3 Typical Scenarios
Typical scenarios are as follows:
●  Common cell
●  Split-RRU/RFU-sector cell
●  Combined-RRU/RFU-sector cell
●  Multi-sector cell
●  Cells in a multi-carrier sector
●  Cell in a sector with RRU/RFU channel cross-connection under MIMO (FDD)
●  Downlink-only cell (FDD)
## NO TE
●  Cell setup in a sector with RRU/RFU channel cross-connection under MIMO is supported
only by FDD. For details, see Base Station Equipment Reliability.
●  RFUs are supported only by FDD.
## 3.1.3.1 Common Cell
A common cell refers to a cell that is established in a common sector served by a
single RF processing module.
## NO TE
For FDD, if the transmit/receive mode of a cell is 4T4R, you can run the MOD RXBRANCH
command to disable two receive channels. Then, the cell will work in 4T2R mode. This
mode is used only to temporarily prevent intermodulation interference. It is not
recommended for normal use because uplink coverage in this mode may shrink compared
with that in 4T4R mode. For TDD, there are no requirements.
Figure 3-2 Common sectors
3.1.3.2 Split-RRU/RFU-Sector Cell
In RRU/RFU splitting scenarios, one RRU/RFU connects to different antennas to
cover different areas.
The RRU/RFU can be split to serve two independent sectors, each of which uses
half of the RRU/RFU's antenna channels for transmitting and receiving signals.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.10

Figure 3-3 Establishing cells in two sectors with 4T4R RRU splitting (example)
## NO TE
In LTE FDD, the 8T8R RRUs that can be split to serve two 4T4R sectors include RRU5862
and RRU5865.
3.1.3.3 Combined-RRU/RFU-Sector Cell
In RRU/RFU combination scenarios, two RRUs/RFUs connect to the same antenna
to cover the same area.
For FDD, macro eNodeBs support combination of 1T2R, 2T2R, 2T4R, or 4T4R RRUs
or RFUs. Micro/LampSite eNodeBs do not support RRU/RFU combination.
Figure 3-4 Combined-RRU/RFU-sector cell (using 2T2R RRUs as an example)
3.1.3.4 Multi-Sector Cell
A multi-sector cell is served by multiple sectors, each of which has separate RF
channels, antenna mode, and transmit power, implementing precise control of
services. If the Cell.
MultiRruCellFlag parameter is set to BOOLEAN_TRUE for a
cell, this cell is a multi-sector cell. The Cell.MultiRruCellMode parameter specifies
the type of such a cell.
Among all FDD micro eNodeB models, only the BTS3911E supports multi-sector
cells.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.11

Figure 3-5 Multi-sector cell
Table 3-1 lists the types of multi-sector cells.
Table 3-1 Types of multi-sector cells
RATCell TypeDescriptionApplicable
eNodeB
FDDSingle
frequency
network
(SFN) cell
Multiple RF modules (such as RRUs)
are combined to serve an SFN cell
where the same physical cell identifier
(PCI) and cell ID are used in all the RF
module coverage areas. This expands
the cell center area and reduces
interference at the cell edge.
SFN cells apply in densely populated
outdoor scenarios and in indoor
scenarios where the distributed
antenna system (DAS) is used. For
details about SFN cells, see
## SFN.
## Macro
eNodeBs
## FDDMPRU
aggregation
cell
An MPRU aggregation cell is the basic
service area for providing indoor
coverage in the LampSite solution.
For details about MPRU aggregation
cells, see SFN.
For details about how to deploy MPRU
aggregation cells, see
eRAN
## Reconfiguration Guide.
LampSite
eNodeBs
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.12

RATCell TypeDescriptionApplicable
eNodeB
## FDD2-RRU-
combination
cell
A 2-RRU-combination cell is set up
using two RRUs of the same model.
The RRUs serve different sectors. In the
downlink, the two RRUs transmit the
same data. In the uplink, the BBP
combines the signals received by the
two RRUs.
2-RRU-combination cells mainly cover
high-speed railways and highways.
They are not recommended because of
unstable performance.
## Macro
eNodeBs
FDDDigital
combination
cell
A digital combination cell is served by
multiple RRUs. The RRUs serve
different sectors but use the same PCI.
In the downlink, the RRUs transmit the
same data. In the uplink, the BBP
combines the signals received by the
RRUs.
Digital combination cells mainly cover
subways and underground business
areas.
## Macro
eNodeBs

3.1.3.5 Cells in a Multi-Carrier Sector
In this scenario, multiple cells working on different frequencies are set up in a
single sector, as shown in Figure 3-6. This helps expand system capacity without
additional base stations.
Figure 3-6 Cells in a multi-carrier sector
Multi-carrier networking applies to densely populated urban areas where traffic
increases rapidly, such as exhibition centers, airport waiting halls, shopping malls,
central business districts, and superior residential buildings.
For details about carrier specifications, see RRU technical descriptions in
## 3900 &
## 5900 Series Base Station Product Documentation
## .
For details about how to reconfigure a single-carrier sector as a dual-carrier sector,
see
eRAN Reconfiguration Guide.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.13

## NO TE
In LTE FDD, cells in a multi-carrier sector must have the same frame offset and uplink and
downlink CP lengths.
3.1.3.6 Downlink-only Cell (FDD)
A downlink-only cell refers to a cell where services are available only in the
downlink. As defined by 3GPP specifications, it is a cell that operates in downlink-
only bands, or it is a cell that provides only downlink services because passive
intermodulation cannot be eliminated in the uplink or there are special
networking requirements. A downlink-only cell generally functions as a secondary
cell for carrier aggregation (CA) UEs.
In downlink-only cells, the parameter settings must meet the following
requirements:
●  For a 1T/2T/4T cell that operates in downlink-only bands, the Cell.WorkMode
parameter must be set to DL_ONLY.
●  For a 1T/2T/4T cell that operates in uplink and downlink bands, the
## Cell.
WorkMode parameter must be set to UL_DL or DL_ONLY. The value
UL_DL is recommended. If the Cell.WorkMode parameter is set to UL_DL, the
ForbidCellSiSwitch option of the CellSiMap.
SiSwitch parameter must be
selected. In this case, the cell is in the access barred state and provides no
uplink services. UEs in other cells cannot be handed over to this cell.
●  For a massive MIMO cell that operates in uplink and downlink bands, the
## Cell.
WorkMode parameter must be set to UL_DL for channel calibration, and
the ForbidCellSiSwitch option of the CellSiMap.
SiSwitch parameter must be
selected. In this case, the cell is in the access barred state and provides no
uplink services. UEs in other cells cannot be handed over to this cell.
This function applies only to macro eNodeBs, BTS3911E, and LampSite eNodeBs.
When an LBBPc is configured and serves at least one downlink-only cell, all RF
modules serving the cells on the LBBPc must directly connect to this board.
## 3.1.4 Cell-related Parameters
This section describes three parameters: frequency band, cell bandwidth, and
reference signal (RS) power.
For other parameters of a cell, such as CPRI compression, CP, preamble format,
and cell radius, see
CPRI Compression, Extended CP, and Extended Cell Range.
For the steps of reconfiguring these parameters, see
eRAN Reconfiguration Guide.
## 3.1.4.1 Frequency Band
The cell frequency bands are described in section 5.5 "Operating bands" in 3GPP
TS 36.104 R11 (2013-07). The frequency band is specified by the Cell.FreqBand
parameter.
If the operating frequencies of a cell belong to multiple frequency bands, the
frequency band specified by the Cell.FreqBand parameter has the highest priority.
For details about multi-band technologies, see
Multi-Band Compatibility
## Enhancement
## .
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.14

Table 3-2 Mapping between the frequency band and frequency range for FDD
macro cells
## Frequency
## Band
(FreqBand)
## Uplink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Uplink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## 11920198021102170
## 21850191019301990
## 31710178518051880
## 41710175521102155
## 5824849869894
## 6830840875885
## 72500257026202690
## 8880915925960
## 91749.91784.91844.91879.9
## 101710177021102170
## 111427.91447.91475.91495.9
## 12699716729746
## 13777787746756
## 14788798758768
15ReservedReservedReservedReserved
16ReservedReservedReservedReserved
## 17704716734746
## 18815830860875
## 19830845875890
## 20832862791821
## 211447.91462.91495.91510.9
## 223410349035103590
## 232000202021802200
## 241626.51660.515251559
## 251850191519301995
## 26814849859894
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.15

## Frequency
## Band
(FreqBand)
## Uplink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Uplink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## 27807824852869
## 28703748758803
29NoneNone717728
## 661710178021102200
## 71663698617652

## NO TE
●  Band 6 is unavailable.
●  Band 29 applies only to carrier aggregation scenarios. For details, see
## Carrier
## Aggregation.
Table 3-3 Mapping between the frequency band and frequency range for FDD
micro cells
## Frequency
## Band
(FreqBand)
## Uplink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Uplink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Highest
## Frequency)
(MHz)
## Downlink
## Frequency
## Range
(Lowest
## Frequency)
(MHz)
## 11920198021102170
## 21850191019301990
## 31710178518051880
## 41710175521102155
## 72500256026202680
## 72500257026202690

eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.16

## 3.1.4.2 Cell Bandwidth
Table 3-4 Cell bandwidth
RATBase Station
## Model
Supported Cell Bandwidth (MHz)
FDDMacro eNodeB1.4, 3, 5, 10, 15, and 20
FDDLampSite
eNodeB
5, 10, 15, and 20
FDDMicro eNodeB3, 5, 10, 15, and 20
Among micro eNodeB models, only the
BTS3911E operating in the 1800 MHz band
supports the 3 MHz bandwidth.

FDD cells support non-standardized bandwidths, while TDD cells do not. For
details about non-standard bandwidths, see
Compact Bandwidth (FDD).
The cell bandwidth is specified by the Cell.
UlBandWidth and Cell.DlBandWidth
parameters.
3.1.4.3 Maximum Transmit Power of a Cell
This section describes the method of configuring the maximum transmit power of
a cell (P
max_out
## ).
## NO TE
For FDD, the method of calculating the maximum cell transmit power described in this
section applies only to a non-massive MIMO cell. In a massive MIMO cell, each physical
channel carries signals transmitted from multiple logical ports of multiple sector split cells,
achieving power gains. To ensure that the power of each physical channel does not exceed
the rated power of a single AAU channel, the maximum CRS power is subject to the
maximum power allowed by the carrier, the number of split cells on the carrier, the number
of CRS ports, the scheme for setting the weight of TM4, and the PA and PB values. For
details, contact Huawei technical support.
## P
max_out
## Configuration Principle
The value of P
max_out
must be less than or equal to the maximum transmit power
of the RRU or RFU that provides the cell coverage.
## NO TE
●  If multiple cells are served by the same RRU or RFU, the sum of the P
max_out
values of
these cells must be less than or equal to the maximum transmit power of the RRU or
## RFU.
●  For details about the maximum transmit power of RRUs or RFUs in various carrier
configuration scenarios, see
## 3900 & 5900 Series Base Station Technical Description.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.17

## P
max_out
## Configuration Parameters
## P
max_out
is not specified by any parameter. It depends on the bandwidth, transmit/
receive mode, CellDlpcPdschPa.PaPcOff, PDSCHCfg.Pb, and reference signal
power. The following table lists parameters that affect P
max_out
for a cell with a
fixed bandwidth and transmit/receive mode.
## Table 3-5 P
max_out
configuration parameters
ParameterSetting Notes
ReferenceSignalPwrIts value must be calculated. For details, see
## Pmax_out Calculation Example.
CellDlpcPdschPa.PaPcOffDual-antenna or four-antenna scenarios:
DB_3_P_A(-3 dB)
Single-antenna scenarios: DB0_P_A(0 dB)
PDSCHCfg.PbSingle-antenna scenarios: 0
Dual-antenna scenarios: 1

## NO TE
The value of ReferenceSignalPwr is determined by one of the following parameters:
●eUCellSectorEqm.ReferenceSignalPwr (or EuSectorEqmGroup.ReferenceSignalPwr
for LampSite eNodeBs)
●PDSCHCfg.ReferenceSignalPwr
The value of the eUCellSectorEqm.ReferenceSignalPwr or
EuSectorEqmGroup.
ReferenceSignalPwr parameter takes effect only when the
## Cell.
MultiRruCellFlag parameter is set to BOOLEAN_TRUE.
The value of the PDSCHCfg.
ReferenceSignalPwr parameter takes effect only when the
## Cell.
MultiRruCellFlag parameter is set to BOOLEAN_FALSE.
## P
max_out
## Query Method
To query P
max_out
of a cell, perform the following steps:
Step 1Run the DSP CELL command to query the value of Maximum transmit
power(0.1dBm). This parameter indicates the maximum transmit power of a
single antenna channel of a cell.
Step 2Multiply the value of Maximum transmit power(0.1dBm) by the number of
transmit channels of a cell to obtain the value of P
max_out
## .
----End
## P
max_out
## Calculation Formula
●  If the TxBranch.
TXMAXPWR parameter is configured, P
max_out
equals the
value of the TxBranch.
TXMAXPWR parameter.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.18

●  In other cases:
## P
max_out
= MAX {TypeA(P
max_out
), TypeB(P
max_out
## )}
where
–   TypeA(P
max_out
) is the maximum transmit power configured for one type
A symbol. The calculation formula is as follows:
–   TypeB(P
max_out
) is the maximum transmit power configured for one type
B symbol. The calculation formula is as follows:
Table 3-6 describes the variables. For details about the preceding formulas, see
section 5.2 in 3GPP TS 36.213 Release 10 (2012-03).
Table 3-6 Variables in the formulas
VariableDescription
ReferenceSi
gnalPwr
RS power of the physical downlink shared channel (PDSCH)
For details, see Pmax_out Configuration Parameters.
## For
TypeA(P
max_
out
) in FDD:
PowerFactor
## Ratio
Power factor ratio of the energy per resource element (EPRE) on
the PDSCH
For TypeA(P
max_out
), the calculation formula is as follows:
PowerFactorRatio = 10
PaPcOff/10
## .
PaPcOff is determined by the CellDlpcPdschPa.
PaPcOff
parameter.
For example, if the CellDlpcPdschPa.PaPcOff parameter is set to
DB_3_P_A(-3 dB), the value of PowerFactorRatio is 10
## –3/10
, that
is, about 0.5.
## For
TypeB(P
max_
out
) in FDD:
PowerFactor
## Ratio
Power factor ratio of the EPRE on the PDSCH
For TypeB(P
max_out
), the calculation formula is as follows:
PowerFactorRatio = 10
PaPcOff/10
x ρ
## B
## /ρ
## A
## .
●PaPcOff is determined by the CellDlpcPdschPa.PaPcOff
parameter.
● ρ
## B
## /ρ
## A
is related to the PDSCHCfg.
Pb parameter. Table 3-7 lists
the mapping between ρ
## B
## /ρ
## A
and the PDSCHCfg.Pb parameter.
For example, if the CellDlpcPdschPa.PaPcOff and PDSCHCfg.Pb
parameters are set to DB_3_P_A(-3 dB) and 1, respectively, then
ρ
## B
## /ρ
## A
is 1. In this case, the value of PowerFactorRatio is 0.5.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.19

VariableDescription
TypeA(N
## RE
## )
Number of non-RS resource elements (REs) in one type A symbol
period. The calculation formula is as follows: TypeA(N
## RE
## ) =
Number of REs per RB x Number of RBs x Number of antennas.
Table 3-8 lists the mapping between the cell bandwidth and
number of RBs.
TypeB(N
## RS
)Number of RSs in one type B symbol period. The calculation
formula is as follows: TypeB(N
## RS
) = Number of RSs per RB x
Number of RBs x Number of antennas.
TypeB(N
## RE
)Number of non-RS REs in one type B symbol period. The
calculation formula is as follows: TypeB(N
## RE
) = Number of REs
per RB x Number of RBs x Number of antennas.

Table 3-7 Mapping between PDSCHCfg.
Pb and ρ
## B
## /ρ
## A
PDSCHCfg.Pbρ
## B
## /ρ
## A
(One Antenna
## Port)
ρ
## B
## /ρ
## A
(Two or Four
## Antenna Ports)
## 015/4
## 14/51
## 23/53/4
## 32/51/2

Table 3-8 Mapping between the cell bandwidth and the maximum number of RBs
## Cell Bandwidth
(MHz)
## 1.435101520
## Maximum
Number of RBs
## 615255075100

## P
max_out
## Calculation Example
Among the three parameters for configuring P
max_out
, PaPcOff and PB can be
configured according to Table 3-5. You only need to calculate the value of
ReferenceSignalPwr.
The following shows an example when the RRU provides a maximum transmit
power of 80 W and serves a 20 MHz cell with two antennas.
## P
max_out
= MAX {TypeA(P
max_out
), TypeB(P
max_out
## )} ≤ 80 W
where
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.20

●  TypeA(P
max_out
## )
= ReferenceSignalPwr x PowerFactorRatio x TypeA(N
## RE
## )
= ReferenceSignalPwr x 0.5 x 2400
= 1200 x
ReferenceSignalPwr
●  TypeB(P
max_out
## )
## =
ReferenceSignalPwr x TypeB(N
## RS
) + ReferenceSignalPwr x
PowerFactorRatio x TypeB(N
## RE
## )
= ReferenceSignalPwr x 400 + ReferenceSignalPwr x 0.5 x 1600
= 1200 x ReferenceSignalPwr
## NO TE
●  TypeA(N
## RE
) = Number of REs per RB x Number of RBs in a 20 MHz cell x Number of
antennas = 12 x 100 x 2 = 2400
●  TypeB(N
## RS
) = Number of RSs per RB x Number of RBs in a 20 MHz cell x Number of
antennas = 2 x 100 x 2 = 400
●  According to Table 3-5, the
PaPcOff parameter for a cell with two antennas is set to
DB_3_P_A(-3 dB). Therefore, for type A symbols, PowerFactorRatio =
## =
## 0.5.
●  According to Table 3-5, the value of the PB parameter for a cell with two antennas is 1.
According to Table 3-7, for a cell with two antennas, ρ
## B
## /ρ
## A
is 1. Therefore, for type B
symbols, PowerFactorRatio =  = 0.5.
●  TypeB(N
## RE
) = Number of REs per RB x Number of RBs in a 20 MHz cell x Number of
antennas = 8 x 100 x 2 = 1600
Based on the preceding calculation results, you can infer that:
## P
max_out
= 1200 x ReferenceSignalPwr ≤ 80 W
ReferenceSignalPwr ≤ 66.67 mW = 18.24 dBm
The value of
ReferenceSignalPwr cannot be greater than 18.24 dBm.
## 3.2 Network Analysis
## 3.2.1 Benefits
The major function of eNodeBs is to provide radio cell coverage for UEs. Cell
management is mandatory.
## 3.2.2 Impacts
## Network Impacts
●  System capacity
–   System capacities vary with bandwidths. A higher bandwidth allows more
UEs to access the network and to be scheduled and supports higher cell
throughput.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.21

–   The multi-carrier technology improves the uplink and downlink network
capacity.
●  Network performance
With the same CPU, digital signal processor (DSP), and memory
configurations, a higher cell bandwidth leads to better service key
performance indicators (KPIs) but higher resource usage.
## Function Impacts
RATFunction
## Name
Function SwitchReferenc
e
## Description
FDDNoneNoneNoneNone

## 3.3 Requirements
## 3.3.1 Licenses
Cell establishment requires capacity licenses. For details about capacity license
control items, see
## License Management.
## 3.3.2 Software
## Prerequisite Functions
## None
## Mutually Exclusive Functions
## RA
## T
## Function
## Name
Function SwitchReferenceDescription
## FD
## D
## Data-
learning-
based
downlink
intelligent
## AMC
## DL_INTEL_AMC_
## SELECTION_SW
option of the
CellIntelAmcConf
ig.IntelligentAm
cSwitch
parameter
eMIMO (FDD)Data-learning-
based downlink
intelligent AMC
cannot be enabled
when a downlink-
only cell is
established.
## FD
## D
## Downlink
intelligent
## JAMC
## CELL_DL_JOINT_I
## NTEL_AMC_SW
option of the
CellIntelAmcConf
ig.IntelligentAm
cSwitch
parameter
Smart 8T8R
## (FDD)
## Downlink
intelligent JAMC
cannot be enabled
when a downlink-
only cell is
established.

eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.22

## 3.3.3 Hardware
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
## Common Cells
Requirements for setting up a common cell are as follows:
●  In FDD, before establishing a cell, check whether hardware resources of BBPs,
CPRI ports, and RF modules meet the cell requirements. For hardware
requirements of macro and LampSite eNodeBs, see
## 3900 & 5900 Series Base
Station Technical Description. For hardware requirements of micro eNodeBs,
see
Micro BTS3900 Series Technical Description.
●  A cell works normally only when the transmit/receive mode of the cell
matches the number of transmit and receive channels of the RF module. For
details about the number of transmit and receive channels supported by the
RF module, see related technical specifications in
## 3900 & 5900 Series Base
## Station Product Documentation.
●  For FDD, if the transmit/receive mode of a cell is 4T4R, you can run the MOD
RXBRANCH command to disable two receive channels. Then, the cell will
work in 4T2R mode. This mode is used only to temporarily prevent
intermodulation interference. It is not recommended for normal use because
uplink coverage in this mode may shrink compared with that in 4T4R mode.
●  Frame offsets of LTE cells established on the same BBP must be the same. If
FDD and TDD cells are established on the same BBP, an identical frame offset
setting for these cells does not affect the performance of the FDD cells.
●  When selecting optical modules for BBPs, ensure that CPRI data rates of the
optical modules match the cell bandwidths and transmit/receive modes. For
the constraints between the CPRI data rates and the cell bandwidths and
transmit/receive modes, see
## 3900 & 5900 Series Base Station Technical
## Description
## .
●  The operating bands of the cells served by RRUs/RFUs must fall into the
frequency bands supported by the RRUs/RFUs.
●  To establish an FDD 4-antenna cell, ensure that its serving RRU/RFU supports
2T4R or 4T4R.
For details about 2T4R or 4T4R RRU/RFU models, see
## 3900 & 5900 Series
## Base Station Technical Description
## .
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.23

## NO TE
In the load-sharing topology where RRUs/RFUs are connected to the same BBP, 2.5
Gbit/s optical modules can be used. The load-sharing topology is not recommended.
## NO TE
The LBBPd supports multiple cell specifications. When a cell is activated and there is no UE
in the cell, the cell may be automatically deactivated and baseband resources may be
optimized to ensure optimal cell performance.
Cells in a Multi-Carrier Sector
To establish two cells in a sector, the following conditions must be met:
●  The RRU/RFU must support multiple carriers. For details about RRU/RFU
models that support multiple carriers, see
## 3900 & 5900 Series Base Station
## Technical Description.
●  For FDD, any combination of standard and non-standard bandwidths can be
used for the two carriers.
●  The frequency ranges of the two cells must be within the frequency bands
supported by the RRU/RFU.
●  The frequency ranges of the two cells cannot overlap.
●  The networking mode for CPRI ports must be star, chain, ring, or load sharing.
For details, see
RF Unit and Topology Management.
Combined-RRU/RFU-Sector Cells
●  For FDD, RRUs/RFUs must support combinations in the following manners:
–   Two 1T2R RRUs/RFUs of the same model can be combined to serve a
2T2R cell.
–   Two 1T2R RRUs/RFUs of the same model can be combined to serve a
2T4R cell.
–   Two 2T2R RRUs/RFUs of the same model can be combined to serve a
4T4R cell.
–   Two 2T4R RRUs/RFUs of the same model can be combined to serve a
4T4R cell.
–   Two 2T4R RRUs/RFUs of the same model can be combined to serve a
4T8R cell.
–   Two 4T4R RRUs of the same model can be combined to serve a 8T8R cell.
●  The length difference between the CPRI optical fibers used to connect the two
RRUs/RFUs to the BBU cannot exceed 2 km.
●  Only a star or cascading topology can be used for two RRUs/RFUs. For details
about topologies, see
RF Unit and Topology Management.
Digital Combination Cells (FDD)
●  Digital combination cells can be established only on the UBBP, LBBPd, or
## UMDU.
●  The RRUs must be RRU3821E modules.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.24

●  RRUs support two to eight levels of cascading connections. CPRI compression
can be enabled to save CPRI resources. A maximum of four levels of cascading
connections are recommended. If the number of cascading levels is greater
than four, cell performance is not guaranteed. In this case, you are advised to
configure more cells.
●  Only a chain topology, but not ring topology, can be used for RRUs serving a
digital combination cell.
●  Digital combination cells do not support extended CPs or the uplink
coordinated multipoint reception (UL CoMP) algorithm.
●  Digital combination cells work only on a bandwidth of 5 MHz, 10 MHz, 15
MHz, or 20 MHz. The transmit/receive mode of the cells must be 2T2R or
## 1T1R.
3.3.4 Others (FDD)
When a digital combination cell is established in multiple sectors, the RRUs
serving this cell must be installed as follows:
●  If the RRUs are not installed in a straight line, the distance between any two
RRUs cannot be greater than 1 km. As shown in Figure 3-7, RRUs 1 to 4 are
installed to serve a cell. The distance between RRU 1 and RRU 4 is the largest
and cannot exceed 1 km.
Figure 3-7 Example of RRUs not installed in a straight line
●  If RRUs are installed in a straight line, the distance between each pair of
neighboring RRUs cannot be greater than 1 km. As shown in Figure 3-8, four
RRUs are installed to serve a cell. The distance between two neighboring
RRUs (for example, RRU1 and RRU2) cannot exceed 1 km.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.25

Figure 3-8 Example of RRUs installed in a straight line
●  RRUs must be cascaded in a chain topology as shown in Figure 3-9.
Requirements of the length of optical fibers are as follows (L
n represents the
length of optical fibers between neighboring equipment):
–   The total length of optical fibers connected between the RRUs serving a
cell cannot exceed 5 km. That is, the sum of L2, L3, and L4 cannot be
greater than 5 km.
–   The total length of optical fibers connecting all the RRUs and the BBP
cannot exceed 20 km. That is, the sum of L1, L2, L3, and L4 cannot be
greater than 20 km.
Figure 3-9 Optical fiber length requirement
3.4 Operation and Maintenance
3.4.1 Data Configuration (FDD)
## 3.4.1.1 Data Preparation
The following table describes the parameters that must be set in a SECTOR MO to
configure a sector.
## Parameter Name
Parameter IDSetting Notes
Sector IDSECTOR.SECTORIDSet this parameter to a unique
value.
Sector NameSECTOR.SECNAMENone
Location NameSECTOR.LOCATIONN
## AME
## None
User LabelSECTOR.USERLABELNone
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.26

Parameter NameParameter IDSetting Notes
Antenna NumberSECTOR.ANTNUMNone
Cabinet No. of
Antenna 1 to
Cabinet No. of
## Antenna 8
SECTOR.ANT1CN to
## SECTOR.ANT8CN
## None
Subrack No. of
Antenna 1 to
Subrack No. of
## Antenna 8
SECTOR.ANT1SRN to
## SECTOR.ANT8SRN
## None
Slot No. of
Antenna 1 to Slot
No. of Antenna 8
SECTOR.ANT1SN to
## SECTOR.ANT8SN
In LampSite scenarios,
● If the pRRU3901 is used, set
this parameter to 255 to enable
automatic allocation of the slot
number to an antenna. If the
slot number is to be assigned
manually, set this parameter to
a value ranging from 1 to 3,
depending on the slot number
of the RF daughter board.
Only one mode of slot number
assignment can be used for a
pRRU, either manual or
automatic.
● If another RRU model is used,
set this parameter to 0.
Channel No. of
Antenna 1 to
Channel No. of
## Antenna 8
SECTOR.ANT1N to
## SECTOR.ANT8N
## None
## Create Default
## Sector Equipment
## SECTOR.CREATESECT
## OREQM
## None
## Default Sector
Equipment ID
## SECTOR.SECTOREQM
## ID
## None

The following table describes the parameters that must be set in a SECTOREQM
MO to configure a piece of sector equipment.
## Parameter Name
Parameter IDSetting Notes
## Sector Equipment
## ID
## SECTOREQM.SECTOR
## EQMID
## None
Sector IDSECTOREQM.SECTOR
## ID
## None
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.27

Parameter NameParameter IDSetting Notes
Antenna NumberSECTOREQM.ANTNU
## M
## None
Cabinet No. of
Antenna 1 to
Cabinet No. of
## Antenna 8
## SECTOREQM.ANT1C
N to
## SECTOREQM.ANT8C
## N
## None
Subrack No. of
Antenna 1 to
Subrack No. of
## Antenna 8
## SECTOREQM.ANT1SR
N to
## SECTOREQM.ANT8SR
## N
## None
Slot No. of
Antenna 1 to Slot
No. of Antenna 8
## SECTOREQM.ANT1S
N to
## SECTOREQM.ANT8S
## N
In LampSite scenarios,
● If the pRRU3901 is used, set
this parameter to 255 to enable
automatic allocation of the slot
number to an antenna. If the
slot number is to be assigned
manually, set this parameter to
a value ranging from 1 to 3,
depending on the slot number
of the RF daughter board.
Only one mode of slot number
assignment can be used for a
pRRU, either manual or
automatic.
● If another RRU model is used,
set this parameter to 0.
Channel No. of
Antenna 1 to
Channel No. of
## Antenna 8
## SECTOREQM.ANT1N
to
## SECTOREQM.ANT8N
## None
Antenna 1 RX/TX
Mode to Antenna
8 RX/TX Mode
## SECTOREQM.ANTTYP
E1 to
## SECTOREQM.ANTTYP
## E8
## None
TX Antenna 1
Master/Slave
Mode to TX
## Antenna 8
Master/Slave
## Mode
## SECTOREQM.TXBKP
MODE1 to
## SECTOREQM.TXBKP
## MODE8
Set this parameter to MASTER.
Do not set this parameter to
SLAVE because the eNodeB does
not support antennas working in
master/slave mode.

The following table describes the parameters that must be set in a CnOperator
MO to configure an operator.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.28

Parameter NameParameter IDSetting Notes
CN Operator IDCnOperator.CnOpera
torId
## None
CN Operator
name
CnOperator.CnOpera
torName
## None
CN Operator typeCnOperator.CnOpera
torType
Each eNodeB can be configured
with only one primary operator
but multiple secondary operators.
Mobile country
code
CnOperator.MccNone
Mobile network
code
CnOperator.MncNone

The following table describes the parameters that must be set in a CnOperatorTa
MO to configure a tracking area for an operator.
Parameter NameParameter IDSetting Notes
Local tracking
area ID
CnOperatorTa.Tracki
ngAreaId
This parameter uniquely identifies
a tracking area. This parameter is
used only within the eNodeB and
is not used during the information
exchange with the EPC. This is
different from the tracking area
identity (TAI) configured in the
EPC tracking area list (TAL).
According to NB-IoT specifications,
TAIs for NB-IoT must be different
from TAIs for LTE.
CN Operator IDCnOperatorTa.CnOpe
ratorId
## None
Tracking area
code
CnOperatorTa.TacNone

The following table describes the parameters that must be set in a Cell MO to
configure a cell.
## Parameter Name
Parameter IDSetting Notes
Local Cell IDCell.LocalCellIdNone
Cell NameCell.CellNameNone
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.29

Parameter NameParameter IDSetting Notes
Csg indicatorCell.CsgIndSet this parameter to its
recommended value.
Uplink cyclic
prefix length
Cell.UlCyclicPrefixSet this parameter to its
recommended value.
Downlink cyclic
prefix length
Cell.DlCyclicPrefixSet this parameter to its
recommended value.
Frequency bandCell.FreqBandNone
Uplink EARFCN
indication
Cell.UlEarfcnCfgIndNone
Uplink EARFCNCell.UlEarfcnThis parameter needs to be
configured only when the
Cell.UlEarfcnCfgInd parameter is
set to CFG.
Downlink EARFCNCell.DlEarfcnSet this parameter to a downlink
EARFCN within the frequency
band specified by the
Cell.FreqBand parameter.
In multi-carrier scenarios, ensure
that the frequency ranges of the
two cells do not overlap.
Uplink bandwidthCell.UlBandWidthNone
## Downlink
bandwidth
Cell.DlBandWidthNone
Cell IDCell.CellIdNone
Physical cell IDCell.PhyCellIdNone
## Additional
spectrum
emission
Cell.AdditionalSpectr
umEmission
## None
Cell FDD TDD
indication
Cell.FddTddIndSet this parameter to CELL_FDD.
Cell specific offsetCell.CellSpecificOff-
set
Set this parameter to its
recommended value.
Frequency offsetCell.QoffsetFreqSet this parameter to its
recommended value.
Root sequence
index
Cell.RootSequenceId
x
For details about setting
restrictions, see 3900 & 5900
Series Base Station MO and
## Parameter Reference
## .
Preamble formatCell.PreambleFmtNone
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.30

Parameter NameParameter IDSetting Notes
Cell radiusCell.CellRadiusThe value of this parameter must
be greater than or equal to the
actual cell radius. Otherwise, UEs
at the cell edge may fail to access
the network.
Set this parameter to a value less
than or equal to 9895 if more
than three physical cells are
established on a UBBPd8 or more
than six physical cells are
established on a UBBPd9.
## Customized
bandwidth
configure
indicator
Cell.CustomizedBand
WidthCfgInd
## None
Customized uplink
bandwidth
Cell.CustomizedULBa
ndWidth
This parameter needs to be
configured only when the
Cell.CustomizedBandWidthCf-
gInd parameter is set to CFG.
## Customized
downlink
bandwidth
Cell.CustomizedDLBa
ndWidth
This parameter needs to be
configured only when the
Cell.CustomizedBandWidthCf-
gInd parameter is set to CFG.
Ue max power
allowed configure
indicator
Cell.UePowerMaxCfg
## Ind
## None
Max transmit
power allowed
Cell.UePowerMaxThis parameter needs to be
configured only when the
Cell.UePowerMaxCfgInd
parameter is set to CFG.
Flag of Multi-RRU
## Cell
Cell.MultiRruCellFlagSet this parameter to
BOOLEAN_TRUE for multi-sector
cells.
Mode of Multi-
RRU Cell
Cell.MultiRruCellMo
de
This parameter needs to be
configured only when the
Cell.MultiRruCellFlag parameter
is set to BOOLEAN_TRUE.
CRS Port NumberCell.CrsPortNumSet this parameter based on the
number of downlink channels. For
example, set this parameter to 2 if
a cell works in 2T mode and to 1 if
the cell works in 1T1R mode.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.31

Parameter NameParameter IDSetting Notes
Cell transmission
and reception
mode
Cell.TxRxMode● In multi-sector scenarios, set
this parameter to the maximum
value of the ANTNUM
parameter in the Sector MO for
sectors in a cell.
● In other scenarios, set this
parameter to the same value of
the
ANTNUM parameter in the
Sector MO.
User labelCell.UserLabelNone
Work modeCell.WorkModeSet this parameter to
corresponding values for different
downlink-only cells.
● For a 1T/2T/4T cell that
operates in downlink-only
bands, set this parameter to
## DL_ONLY.
● For a 1T/2T/4T cell that
operates in uplink and
downlink bands, set this
parameter to UL_DL.
● For a massive MIMO cell that
operates in uplink and
downlink bands, set this
parameter to UL_DL.
Cell Slave BandCell.CellSlaveBandSet this parameter by running the
ADD CELLBAND command.
## Cell Standby
## Mode
Cell.EuCellStandbyM
ode
## None
CPRI CompressionCell.CPRICompressio
n
For details, see CPRI Compression.

The following table describes the parameters that must be set in an
eUCellSectorEqm MO to configure a piece of sector equipment for the cell.
## Parameter Name
Parameter IDSetting Notes
Local cell IDeUCellSectorEqm.Loc
alCellId
## None
Sector equipment
## ID
eUCellSectorEqm.Sec
torEqmId
## None
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.32

Parameter NameParameter IDSetting Notes
Reference signal
power
eUCellSectorEqm.Ref
erenceSignalPwr
If this parameter is set to 32767,
the RS power of the cell is
specified in the PDSCHCfg MO.
For the value calculation, see
## 3.1.4.3 Maximum Transmit
Power of a Cell.
## Baseband
equipment ID
eUCellSectorEqm.Bas
eBandEqmId
If this parameter is set to 255, no
baseband equipment is specified
for the cell. In this case, the cell
can use any baseband equipment
of the eNodeB.
This parameter must be
configured when massive MIMO
and non-massive-MIMO cells
share the same board.
Sector CPRI
## Compression
eUCellSectorEqm.Sec
torCpriCompression
This parameter specifies the CPRI
compression mode of each piece
of sector equipment. It is used
only when the
Cell.MultiRruCellMode parameter
is set to SFN.
● If this parameter is set to NULL,
the CPRI compression mode of
carriers is specified by the
CPRICompression parameter in
the Cell MO.
● If this parameter is set to
another value, the CPRI
compression mode of carriers is
specified by this parameter.
● This parameter does not apply
to hRRUs.
Auto Config FlageUCellSectorEqm.Aut
oCfgFlag
## None

The following table describes the parameters that must be set in a CellOp MO to
configure a cell operator.
## Parameter Name
Parameter IDSetting Notes
Local cell IDCellOp.LocalCellIdNone
Local tracking
area ID
CellOp.TrackingAreaI
d
## None
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.33

Parameter NameParameter IDSetting Notes
Cell reserved for
operator
CellOp.CellReservedF
orOp
## None
Operator uplink
RB used ratio
CellOp.OpUlRbUsedR
atio
## None
## Operator
downlink RB used
ratio
CellOp.OpDlRbUsedR
atio
## None

The following table describes the parameters that must be set in a
BASEBANDEQM MO to configure baseband equipment information.
Parameter NameParameter IDSetting Notes
## Baseband
Equipment ID
## BASEBANDEQM.BASE
## BANDEQMID
Each BASEBANDEQMID
parameter value identifies a piece
of baseband equipment.
One piece of baseband equipment
can include multiple BBPs. For
example, there are two SN
parameters in the following MML
command, indicating that
baseband equipment 0 includes
two BBPs. However, it is
recommended that one piece of
baseband equipment include only
one BBP.
## ADD BASEBANDEQM: BASEBANDEQMID=0,
## BASEBANDEQMTYPE=ULDL,
## UMTSDEMMODE=NULL, SN1=2, SN2=1;
A BBP cannot belong to multiple
pieces of baseband equipment.
## Baseband
## Equipment Type
## BASEBANDEQM.BASE
## BANDEQMTYPE
## None

The following table describes the parameters that must be set in a CellSiMap MO
to configure baseband equipment information.
## Parameter Name
Parameter IDOptionSetting Notes
## Cell System
## Information
## Switch
CellSiMap.SiSwitchForbidCellSiS
witch
This option must
be selected when
establishing a
downlink-only cell
in massive MIMO
scenarios.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.34


3.4.1.2 Using MML Commands
This section provides the MML command examples in different scenarios.
●Scenario 1: Establishing a Common Cell
●Scenario 2: Establishing a Split-RRU-Sector Cell
●Scenario 3: Establishing a Combined-RRU-Sector Cell
●Scenario 4: Establishing a Multi-Sector Cell
●Scenario 5: Establishing Cells in a Multi-Carrier Sector
●Scenario 6: Establishing a Downlink-only Cell
## NO TICE
● In UMPT+UMPT scenarios, the distributed cell deployment function and board
resource assignment mode 2 are mutually exclusive.
●  Board resource assignment mode 2 is specified by the
BRDRESASSIGNMENT.BRDASSIGNMENT parameter.
●  The distributed cell deployment function is controlled by the
eNodeBResModeAlgo.EnbCellDstDeploySw parameter.
● After the sector equipment or equipment group is added during the cell
establishment, the BBU needs to apply to RF modules for carrier resources. If a
cell is activated immediately after the sector equipment or equipment group is
added, the cell may fail to be activated within a short time. Afterward, services
of the cell are recovered. The DSP CELL command can be used to check the cell
status.
● The parameter settings in the following commands are used for reference only.
Set the parameters based on network requirements.
● For cell-related reconfiguration, see
eRAN Reconfiguration Guide.
Scenario 1: Establishing a Common Cell
## NO TE
●  The antenna transmit/receive mode must match the number of antennas in a sector.
Accordingly, the sector serving the cell must be configured with the required number of
antennas (specified by the SECTOR.
ANTNUM parameter). For example, if a cell works
in 4T4R mode, the SECTOR.ANTNUM parameter must be set to 4.
●  If the SECTOR.CREATESECTOREQM parameter is set to TRUE by running the ADD
SECTOR command, the ADD SECTOREQM command is not required. The default value
of this parameter is FALSE.
//(Optional) Adding a sector and sector equipment when an RRU is added
ADD SECTOR: SECTORID=0, ANTNUM=2, ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A, ANT2CN=0,
## ANT2SRN=60, ANT2SN=0, ANT2N=R0B, CREATESECTOREQM=TRUE, SECTOREQMID=0;
//Adding baseband equipment
ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL, SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.35

//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Adding a cell
ADD CELL: LocalCellId=0, CellName="cell0", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5020,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment to the
cell
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Adding an operator for the cell
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Activating the cell
ACT CELL: LocalCellId=0;
Scenario 2: Establishing a Split-RRU-Sector Cell
Establishing two 2T2R cells by splitting a 4T4R RRU is used as an example.
//Configuring two sectors with the SECTOR.ANTNUM parameter set to 2, and then allocating any two
antenna channels of the RRU to one sector and the other two antenna channels to the other sector (For
example, after two 2T2R sectors numbered 0 and 1 and related sector equipment are configured, sector 0
uses antenna channels A and B, and sector 1 uses antenna channels C and D)
## ADD SECTOR: SECTORID=0, SECNAME="0", LOCATIONNAME="0", USERLABEL="0", ANTNUM=2,
ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A, ANT2CN=0, ANT2SRN=60, ANT2SN=0, ANT2N=R0B,
## CREATESECTOREQM=TRUE, SECTOREQMID=0;
## ADD SECTOR: SECTORID=1, SECNAME="0", LOCATIONNAME="0", USERLABEL="0", ANTNUM=2,
ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0C, ANT2CN=0, ANT2SRN=60, ANT2SN=0, ANT2N=R0D,
## CREATESECTOREQM=TRUE, SECTOREQMID=1;
//Adding baseband equipment
ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL, SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Adding two cells
ADD CELL: LocalCellId=0, CellName="cell0", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5020,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
ADD CELL: LocalCellId=1, CellName="cell1", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5120,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=1, PhyCellId=1, FddTddInd=CELL_FDD,
RootSequenceIdx=1, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment to
each of the two 2T2R cells. Bind the two cells to two pieces of sector equipment.
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
ADD EUCELLSECTOREQM: LocalCellId=1, SectorEqmId=1, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Adding the operator information about two cells
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
ADD CELLOP: LocalCellId=1, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Activating the two cells
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.36

ACT CELL: LocalCellId=0;
ACT CELL: LocalCellId=1;
Scenario 3: Establishing a Combined-RRU-Sector Cell
Establishing a 4T4R cell by combining two 2T2R RRUs is used as an example.
//Adding a sector and sector equipment, and configuring one sector with the SECTOR.ANTNUM parameter
set to 4 (separating four antenna ports to two groups and configuring them to the two 2T2R RRUs)
ADD SECTOR: SECTORID=0, SECNAME="Sector0", LOCATIONNAME="River", USERLABEL="0", ANTNUM=4,
ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A, ANT2CN=0, ANT2SRN=60, ANT2SN=0, ANT2N=R0B,
ANT3CN=0, ANT3SRN=61, ANT3SN=0, ANT3N=R0A, ANT4CN=0, ANT4SRN=61, ANT4SN=0, ANT4N=R0B,
## CREATESECTOREQM=TRUE, SECTOREQMID=0;
//Adding baseband equipment
ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL, SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Adding a cell
ADD CELL: LocalCellId=0, CellName="cell0", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5020,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=4T4R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
//Adding an operator for the cell
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment to the
cell
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Activating the cell
ACT CELL: LocalCellId=0;
Scenario 4: Establishing a Multi-Sector Cell
Establishing a digital combination cell in two sectors is used as an example.
//(Optional) Adding sectors and sector equipment and establishing a sector on each RRU when RRUs are
added
ADD SECTOR: SECTORID=0, ANTNUM=2, ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A, ANT2CN=0,
## ANT2SRN=60, ANT2SN=0, ANT2N=R0B, CREATESECTOREQM=TRUE, SECTOREQMID=0;
ADD SECTOR: SECTORID=1, ANTNUM=2, ANT1CN=0, ANT1SRN=61, ANT1SN=0, ANT1N=R0A, ANT2CN=0,
## ANT2SRN=61, ANT2SN=0, ANT2N=R0B, CREATESECTOREQM=TRUE, SECTOREQMID=1;
//Adding baseband equipment
ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL, SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Adding a digital combination cell
ADD CELL: LocalCellId=0, CellName="Cell0", FreqBand=7, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=2900,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_TRUE, MultiRruCellMode=DIGITAL_COMBINATION, TxRxMode=2T2R,
CsgInd=BOOLEAN_FALSE, UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP,
AdditionalSpectrumEmission=1, CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0,
CellRadius=10000, CrsPortNum=CRS_PORT_2, WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment to the
cell. Bind the two pieces of established sector equipment to the same cell.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.37

ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=1, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Adding an operator for the cell
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Activating the cell
ACT CELL: LocalCellId=0;
Scenario 5: Establishing Cells in a Multi-Carrier Sector
## NO TICE
● Signals of other carriers will be interrupted intermittently when a carrier is
added to or removed from a multi-carrier RRU. Therefore, you are advised to
add or remove a carrier in off-peak hours.
● Before establishing multiple cells in a multi-carrier sector, ensure that the
multi-carrier capabilities supported by RRUs and CPRI ports and the cell
specifications of the BBP meet the requirements described in 3.3.3 Hardware.
Establishing cells in a dual-carrier sector is used as an example.
//(Optional) Adding a sector and sector equipment when an RRU is added
ADD SECTOR: SECTORID=0, ANTNUM=2, ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A, ANT2CN=0,
## ANT2SRN=60, ANT2SN=0, ANT2N=R0B, CREATESECTOREQM=TRUE, SECTOREQMID=0;
//Adding baseband equipment
ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL, SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Establishing two cells working on different frequencies (specified by Cell.
DlEarfcn) and ensuring that the
frequency bands do not overlap
ADD CELL: LocalCellId=0, CellName="cell0", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5020,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
ADD CELL: LocalCellId=1, CellName="cell1", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5120,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=1, PhyCellId=0, FddTddInd=CELL_FDD,
RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG, UePowerMaxCfgInd=NOT_CFG,
MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R, CsgInd=BOOLEAN_FALSE,
UlCyclicPrefix=NORMAL_CP, DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1,
CellSpecificOffset=dB0, QoffsetFreq=dB0, PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2,
WorkMode=UL_DL, CPRICompression=NO_COMPRESSION;
//Adding an operator for two cells
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
ADD CELLOP: LocalCellId=1, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment to the
cells. Set the eUCellSectorEqm.
SectorEqmId parameter to the same value for the cells. That is, bind the
piece of the established sector equipment to the two cells simultaneously.
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
ADD EUCELLSECTOREQM: LocalCellId=1, SectorEqmId=0, ReferenceSignalPwr=32767, BaseBandEqmId=255,
SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Activating the cells
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.38

ACT CELL: LocalCellId=0;
ACT CELL: LocalCellId=1;
Scenario 6: Establishing a Downlink-only Cell
## NO TE
●  The antenna transmit/receive mode must match the number of antennas in a sector.
Accordingly, the sector serving the cell must be configured with the required number of
antennas (specified by the SECTOR.
ANTNUM parameter). For example, if a cell works in
4T4R mode, the SECTOR.ANTNUM parameter must be set to 4.
●  If the SECTOR.CREATESECTOREQM parameter is set to TRUE by running the ADD
SECTOR command, the ADD SECTOREQM command is not required. The default value
of this parameter is FALSE.
●  Establishing a downlink-only cell in non-massive MIMO scenarios
//(Optional) Adding a sector and sector equipment when an RRU is added
## ADD SECTOR: SECTORID=0, ANTNUM=2, ANT1CN=0, ANT1SRN=60, ANT1SN=0, ANT1N=R0A,
## ANT2CN=0, ANT2SRN=60, ANT2SN=0, ANT2N=R0B, CREATESECTOREQM=TRUE, SECTOREQMID=0;
//Adding baseband equipment
## ADD BASEBANDEQM: BASEBANDEQMID=0, BASEBANDEQMTYPE=ULDL, UMTSDEMMODE=NULL,
## SN1=2;
//(Optional) Adding operator and tracking area information if unavailable
//Adding an operator
ADD CNOPERATOR: CnOperatorId=0, CnOperatorName="mobile",
CnOperatorType=CNOPERATOR_PRIMARY, Mcc="460", Mnc="01";
//Adding a tracking area for the operator
ADD CNOPERATORTA: TrackingAreaId=0, CnOperatorId=0, Tac=33;
//Adding a cell with its WorkMode parameter set to DL_ONLY
ADD CELL: LocalCellId=0, CellName="cell0", FreqBand=12, UlEarfcnCfgInd=NOT_CFG, DlEarfcn=5020,
UlBandWidth=CELL_BW_N50, DlBandWidth=CELL_BW_N50, CellId=0, PhyCellId=0,
FddTddInd=CELL_FDD, RootSequenceIdx=0, CustomizedBandWidthCfgInd=NOT_CFG,
UePowerMaxCfgInd=NOT_CFG, MultiRruCellFlag=BOOLEAN_FALSE, TxRxMode=2T2R,
WorkMode=DL_ONLY, CsgInd=BOOLEAN_FALSE, UlCyclicPrefix=NORMAL_CP,
DlCyclicPrefix=NORMAL_CP, AdditionalSpectrumEmission=1, CellSpecificOffset=dB0, QoffsetFreq=dB0,
PreambleFmt=0, CellRadius=10000, CrsPortNum=CRS_PORT_2, CPRICompression=NO_COMPRESSION;
//Adding cell sector equipment by binding the baseband equipment (optional) and sector equipment
to the cell
ADD EUCELLSECTOREQM: LocalCellId=0, SectorEqmId=0, ReferenceSignalPwr=32767,
BaseBandEqmId=255, SectorCpriCompression=NULL, AutoCfgFlag=AUTO_MODE_CFG;
//Adding an operator for the cell
ADD CELLOP: LocalCellId=0, TrackingAreaId=0, CellReservedForOp=CELL_NOT_RESERVED_FOR_OP,
OpUlRbUsedRatio=16, OpDlRbUsedRatio=16;
//Activating the cell
ACT CELL: LocalCellId=0;
●  Establishing a downlink-only cell in massive MIMO scenarios
//Establishing a common cell
//Configuring the corresponding algorithm switch
MOD CELLSIMAP: LocalCellId=0, SiSwitch=ForbidCellSiSwitch-1;
## Deactivation Command Examples
//Deactivating a cell
DEA CELL: LocalCellId=0;
3.4.1.3 Using the MAE-Deployment
For detailed operations, see Feature Configuration Using the MAE-Deployment.
## 3.4.2 Activation Observation
Step 1Run the DSP CELL command to check the cell status.
If the Cell instance state parameter is Normal, the cell has been activated.
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.39

Step 2Use a UE to access this cell.
Run the DSP CELLUECNT command. If the value of Cell Total Counter in the
command output is not 0, the UE accesses the cell successfully, indicating that the
cell works properly.
----End
## 3.4.3 Possible Issues
## Fault Description
Cell status is abnormal.
## Possible Issues
Step 1Monitor the cell status on the MAE-Access. If the cell is in the outage state, rectify
the fault by following the instructions in
Cell Outage Detection and
## Compensation
## .
Step 2View the alarms on the MAE-Access. If any alarm has been reported, clear the
alarm according to
## 3900 & 5900 Series Base Station Alarm Reference.
The following table lists the common alarms related to a cell.
Alarm ID
## Alarm Name
ALM-26816Licensed Feature Unusable
ALM-26818No License Running in System
ALM-29240Cell Unavailable
ALM-29243Cell Capability Degraded
ALM-29245Cell Blocked
ALM-29248RF Out of Service
----End
eRAN
## Cell Management Feature Parameter Description3 Cell Management
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.40

## 4 Parameters
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
## Cell Management Feature Parameter Description4 Parameters
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.41

## 5 Counters
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
## Cell Management Feature Parameter Description5 Counters
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.42

## 6 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
## Cell Management Feature Parameter Description6 Glossary
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.43

## 7 Reference Documents
-  3GPP TS 36.211: "Evolved Universal Terrestrial Radio Access (E-UTRA);
Physical channels and modulation"
-  3GPP TS 36.213: "Evolved Universal Terrestrial Radio Access (E-UTRA);
Physical layer procedures"
-  3GPP TS 36.331: "Evolved Universal Terrestrial Radio Access (E-UTRA); Radio
Resource Control (RRC) protocol specification"
## 4.
Micro BTS3900 Series Technical Description
5.3900 & 5900 Series Base Station MO and Parameter Reference
6.3900 & 5900 Series Base Station Initial Configuration Guide in 3900 & 5900
## Series Base Station Product Documentation
## 7.3900 & 5900 Series Base Station Alarm Reference
## 8.3900 & 5900 Series Base Station Technical Description
## 9.  FDD: SFN
10.CPRI Compression
11.License Management
12.RRUxxxx Hardware Description (RRUxxxx indicates the RRU model.)
## 13.
Extended CP
14.Extended Cell Range
15.eRAN Reconfiguration Guide
16.Base Station Equipment Reliability
17.Multi-Band Compatibility Enhancement
18.Carrier Aggregation
19.RF Unit and Topology Management
20.Cell Outage Detection and Compensation
- FDD: Compact Bandwidth (FDD)
22.eMIMO (FDD)
23.Smart 8T8R (FDD)
eRAN
## Cell Management Feature Parameter Description7 Reference Documents
Issue 05 (2023-09-14)Copyright © Huawei Technologies Co., Ltd.44