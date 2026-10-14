

RRU5904&RRU5904N&RRU5904w&RRU5304&RRU
## 5304w
## Hardware Description
## Issue17
## Date2025-06-24
## HUAWEI TECHNOLOGIES CO., LTD.



Copyright © Huawei Technologies Co., Ltd. 2025. All rights reserved.
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
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w Hardware Description
.........................................................................................................................................................1
1.1 Changes in RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w Hardware Description..................2
1.2 RRU Introduction.....................................................................................................................................................................7
1.2.1 RRU Exterior...........................................................................................................................................................................7
1.2.2 RRU Functions.................................................................................................................................................................... 10
1.2.3 RRU Technical Specifications.........................................................................................................................................12
1.2.4 RRU Ports............................................................................................................................................................................. 12
1.2.5 RRU Indicators....................................................................................................................................................................15
1.2.6 Optical Modules.................................................................................................................................................................17
1.3 RRU Cables..............................................................................................................................................................................20
1.3.1 RRU Cable List.................................................................................................................................................................... 20
1.3.2 RRU PGND Cable...............................................................................................................................................................22
1.3.3 RRU Power Cable...............................................................................................................................................................23
1.3.4 CPRI Optical Fiber............................................................................................................................................................. 25
1.3.5 RRU RF Jumper...................................................................................................................................................................29
1.3.6 RRU AISG Multi-Wire Cable...........................................................................................................................................30
1.3.7 RRU AISG Extension Cable............................................................................................................................................. 31
1.4 RF Cable Connections for the RRU................................................................................................................................. 33
1.5 RRU Auxiliary Devices..........................................................................................................................................................34
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
Hardware DescriptionContents
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.iii

1 RRU5904&RRU5904N&RRU5904w&RRU5
304&RRU5304w Hardware Description
## Overview
This document provides reference for planning and deploying a DC blade
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w (referred to as RRU in
this document), and describes the RRU exterior, ports, functions, cable
classifications, connector specifications, and cable connections.
The exteriors of components and cables in this document are for reference only.
The actual exteriors may be different.
## Product Version
The following table lists the RRU product versions related to this document.
## Product
## Name
Solution VersionProduct Version
## RRU5904
## RRU5304
SRAN11.1 and
later
V100R011C10 and later
For details about the software versions of
RF modules, see Software and Hardware
## Compatibility Description.
RRU5904w
RRU5304w
SRAN12.1 and
later
V100R012C10 and later
For details about the software versions of
RF modules, see Software and Hardware
## Compatibility Description.
RRU5904NSRAN13.1 and
later
V100R013C10 and later
For details about the software versions of
RF modules, see Software and Hardware
## Compatibility Description.

## Intended Audience
This document is intended for:
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.1

●  Base station installation engineers
●  System engineers
●  Site maintenance engineers
## Organization
1.1 Changes in RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w
## Hardware Description
This section describes the changes in
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w Hardware Description.
1.2 RRU Introduction
This section describes the exterior, ports, indicators, functions, and other
information of an RRU.
1.3 RRU Cables
This section describes RRU cables.
1.4 RF Cable Connections for the RRU
RF cable connections for the RRU vary depending on the configurations of the
RRU and antenna. The RF cable connections in this document are for reference
only. The actual cable connections depend on onsite conditions.
1.5 RRU Auxiliary Devices
This section describes RRU auxiliary devices.
1.1 Changes in
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304
w Hardware Description
This section describes the changes in
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5304w Hardware Description.
## 17 (2025-06-24)
This is the seventeenth commercial release.
Compared with Issue 16 (2024-11-12), this issue does not include any new topics.
Compared with Issue 16 (2024-11-12), this issue includes the following changes.
## Topic
## Change Description
1.2.6 Optical ModulesRevised descriptions.

Compared with Issue 16 (2024-11-12), this issue does not exclude any topics.
## 16 (2024-11-12)
This is the sixteenth commercial release.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.2

Compared with Issue 15 (2024-09-06), this issue does not include any new topics.
Compared with Issue 15 (2024-09-06), this issue includes the following changes.
TopicChange Description
1.3.3 RRU Power CableAdded the description "If a small
integrated DC power supply device is
provided by the customer, contact
Huawei engineers."

Compared with Issue 15 (2024-09-06), this issue does not exclude any topics.
## 15 (2024-09-06)
This is the fifteenth commercial release.
Compared with Issue 14 (2023-09-10), this issue does not include any new topics.
Compared with Issue 14 (2023-09-10), this issue includes the following changes.
TopicChange Description
1.4 RF Cable Connections for the
## RRU
Revised descriptions.

Compared with Issue 14 (2023-09-10), this issue does not exclude any topics.
## 14 (2023-09-10)
This is the fourteenth commercial release.
Compared with Issue 13 (2023-07-15), this issue does not include any new topics.
Compared with Issue 13 (2023-07-15), this issue includes the following changes.
## Topic
## Change Description
## 1
RRU5904&RRU5904N&RRU5904w
&RRU5304&RRU5304w Hardware
## Description
Added descriptions to indicate that the
exteriors of components and cables in
this document are for reference only.

Compared with Issue 13 (2023-07-15), this issue does not exclude any topics.
## 13 (2023-07-15)
This is the thirteenth commercial release.
Compared with Issue 12 (2023-04-23), this issue does not include any new topics.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.3

Compared with Issue 12 (2023-04-23), this issue includes the following changes.
TopicChange Description
1.2.6 Optical ModulesAdded the storage environment
requirements of optical modules.

Compared with Issue 12 (2023-04-23), this issue does not exclude any topics.
## 12 (2023-04-23)
This is the twelfth commercial release.
Compared with Issue 11 (2022-06-27), this issue does not include any new topics.
Compared with Issue 11 (2022-06-27), this issue includes the following changes.
TopicChange Description
1.3.3 RRU Power CableAdded information about the power
supply device(s).
1.5 RRU Auxiliary DevicesModified RPCU-related information.

Compared with Issue 11 (2022-06-27), this issue does not exclude any topics.
## 11 (2022-06-27)
This is the eleventh commercial release.
Compared with Issue 10 (2020-12-29), this issue does not include any new topics.
Compared with Issue 10 (2020-12-29), this issue includes the following changes.
## Topic
## Change Description
1.2.6 Optical ModulesAdded the CPRI port rates supported by
optical modules.

Compared with Issue 10 (2020-12-29), this issue does not exclude any topics.
## 10 (2020-12-29)
This is the tenth commercial release.
Compared with Issue 09 (2020-10-31), this issue does not include any new topics.
Compared with Issue 09 (2020-10-31), this issue includes the following changes.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.4

TopicChange Description
Entire documentAdded the RRU5904w (850M).

Compared with Issue 09 (2020-10-31), this issue does not exclude any topics.
## 09 (2020-10-31)
This is the ninth commercial release.
Compared with Issue 08 (2020-08-30), this issue does not include any new topics.
Compared with Issue 08 (2020-08-30), this issue includes the following changes.
TopicChange Description
1.3.5 RRU RF JumperAdded descriptions of feeders.

Compared with Issue 08 (2020-08-30), this issue does not exclude any topics.
## 08 (2020-08-30)
This is the eighth commercial release.
Compared with Issue 07 (2019-10-28), this issue does not include any new topics.
Compared with Issue 07 (2019-10-28), this issue includes the following changes.
## Topic
## Change Description
Entire documentAdded the RRU5904N.

Compared with Issue 07 (2019-10-28), this issue does not exclude any topics.
## 07 (2019-10-28)
This is the seventh commercial release.
Compared with Issue 06 (2019-08-30), this issue does not include any new topics.
Compared with Issue 06 (2019-08-30), this issue includes the following changes.
## Topic
## Change Description
Entire documentAdded the RRU5304w (700M).

Compared with Issue 06 (2019-08-30), this issue does not exclude any topics.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.5

## 06 (2019-08-30)
This is the sixth commercial release.
Compared with Issue 05 (2019-07-20), this issue does not include any new topics.
Compared with Issue 05 (2019-07-20), this issue includes the following changes.
TopicChange Description
1.3.3 RRU Power CableAdded the RRU power cable (screw-
free type).

Compared with Issue 05 (2019-07-20), this issue does not exclude any topics.
## 05 (2019-07-20)
This is the fifth commercial release.
Compared with Issue 04 (2018-10-30), this issue does not include any new topics.
Compared with Issue 04 (2018-10-30), this issue includes the following changes.
## Topic
## Change Description
1.3.3 RRU Power CableModified the power cable
specifications.

Compared with Issue 04 (2018-10-30), this issue does not exclude any topics.
## 04 (2018-10-30)
This is the fourth commercial release.
Compared with Issue 03 (2018-09-30), this issue does not include any new topics.
Compared with Issue 03 (2018-09-30), this issue includes the following changes.
## Topic
## Change Description
Entire documentRevised descriptions in this document.

Compared with Issue 03 (2018-09-30), this issue does not exclude any topics.
## 03 (2018-09-30)
This is the third commercial release.
Compared with Issue 02 (2018-07-20), this issue does not include any new topics.
Compared with Issue 02 (2018-07-20), this issue includes the following changes.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.6

TopicChange Description
Entire documentAdded information about the
RRU5304w.

Compared with Issue 02 (2018-07-20), this issue does not exclude any topics.
## 02 (2018-07-20)
This is the second commercial release.
Compared with Issue 01 (2017-12-30), this issue does not include any new topics.
Compared with Issue 01 (2017-12-30), this issue includes the following changes.
TopicChange Description
Entire documentAdded information about the RRU5304
and RRU5904w.

Compared with Issue 01 (2017-12-30), this issue does not exclude any topics.
## 01 (2017-12-30)
This is the first commercial release.
Compared with Draft A (2017-09-30), this issue does not include any new topics.
Compared with Draft A (2017-09-30), this issue does not include any changes.
Compared with Draft A (2017-09-30), this issue does not exclude any topics.
## Draft A (2017-09-30)
This is a draft.
1.2 RRU Introduction
This section describes the exterior, ports, indicators, functions, and other
information of an RRU.
1.2.1 RRU Exterior
This section describes the exterior and dimensions of an RRU.
The following figure shows an RRU.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.7

Figure 1-1 Exterior of the
RRU5904&RRU5904N&RRU5904w(1.8G)&RRU5904w(1.9G)&RRU5304&RRU5304
w(2.6G)

Figure 1-2 Exterior of the RRU5304w(700M)&RRU5904w(850M)
The following figure shows RRU dimensions.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.8

## NO TE
In the figure, 150 mm is the actual depth of the module, and 170 mm is the depth
including the protective structure.
Figure 1-3 Dimensions of the
RRU5904&RRU5904N&RRU5904w(1.8G)&RRU5904w(1.9G)&RRU5304&RRU5304
w(2.6G)

Figure 1-4 Dimensions of the RRU5304w(700M)&RRU5904w(850M)
You can obtain the RRU name, frequency band, and power supply information
from the nameplate on the cover plate of the cabling cavity. The following figure
shows the position of the nameplate on the RRU.
## NO TE
The nameplate on the RRU in the figure is only for reference.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.9

Figure 1-5 Nameplate position
(1) Nameplate(2) Module name(3) Frequency band(4) Power supply

1.2.2 RRU Functions
This section describes main functions of an RRU.
The RRU consists of the high-speed interface module, signal processing unit,
power amplifier, duplexer, extension ports, and power module.
The following figure shows the functional structure of the RRU.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.10

Figure 1-6 Functional structure of an RRU

## NO TE
For details about the extension ports, see 1.2.4 RRU Ports.
The RRU performs the following functions:
●  Receives downlink baseband data from the BBU and sends uplink baseband
data to the BBU.
●  Receives RF signals from the antenna system, down-converts the signals to
intermediate frequency (IF) signals, amplifies the IF signals, and performs
analog-to-digital conversion. Filters downlink signals, performs digital-to-
analog (D/A) signal conversion, and up-converts RF signals to the transmit
(TX) band on the TX channel.
●  Multiplexes receive (RX) and TX signals on the RF channel so that these
signals can share the same antenna channel, and filters the RX and TX signals.
●  Provides a built-in bias tee (BT). Besides receiving and transmitting RF signals,
RF ports A and B also can transmit OOK signals to antennas through the
built-in BT and supply DC power to the tower-mounted amplifier (TMA). RF
ports C and D can supply DC power to the TMA.
●  Works with the monitoring extension box (MEB). The MEB can transmit
external RS485 communication signals and dry contact monitoring signals
into the RRU, implementing information monitoring and reporting. For details
about the MEB, see user guides of the corresponding models.
●  DC RRUs can use external power modules (such as OPM15M(Ver.B) and
OPM50M(Ver.B)) to support AC scenarios. For details about the external
power modules, see user guides of the corresponding models.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.11

1.2.3 RRU Technical Specifications
This section describes technical specifications of an RRU, including supported RATs,
frequency bands, RF specifications, engineering specifications, and antenna
capabilities.
●  For details about technical specifications of the RRU5904, see RRU5904
## Technical Specifications.
●  For details about technical specifications of the RRU5904w, see RRU5904w
## Technical Specifications.
●  For details about technical specifications of the RRU5304, see RRU5304
## Technical Specifications.
●  For details about technical specifications of the RRU5304w, see RRU5304w
## Technical Specifications.
●  For details about technical specifications of the RRU5904N, see RRU5904N
## Technical Specifications.
1.2.4 RRU Ports
This section describes RRU ports at the bottom and in the cabling cavity and
indicators.
Figure 1-7 shows the ports on the
RRU5904&RRU5904N&RRU5904w(1.8G)&RRU5904w(1.9G)&RRU5304&RRU5304
w(2.6G). Figure 1-8 shows the ports on the
RRU5304w(700M)&RRU5904w(850M).
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.12

Figure 1-7 Ports on the
RRU5904&RRU5904N&RRU5904w(1.8G)&RRU5904w(1.9G)&RRU5304&RRU5304
w(2.6G)

RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.13

Figure 1-8 Ports on the RRU5304w(700M)&RRU5904w(850M)

The following table describes the bottom ports, ports in the cabling cavity, and
indicators on the RRU.
Table 1-1 Ports and indicators on the RRU panels
## Item
SilkscreenConnectorDescription
(1) Ports at the
bottom
## A T/R4.3-10
female
connector
TX/RX RF port A, supporting
RET signal transmission
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.14

ItemSilkscreenConnectorDescription
## C T/R4.3-10
female
connector
TX/RX RF port C
## D T/R4.3-10
female
connector
TX/RX RF port D
## B T/R4.3-10
female
connector
TX/RX RF port B, supporting
RET signal transmission
RETDB9 female
connector
Communication port for the
RET antenna, supporting RET
signal transmission
(2) Ports in the
cabling cavity
RTN(+)Male fast
connector
Power port
## NEG(-)
CPRI0SFP female
connector
Optical port 0, connected to
the BBU or an upper-level RRU
CPRI1SFP female
connector
Optical port 1, connected to a
lower-level RRU or the BBU
(3) IndicatorsRUNN/AFor details, see 1.2.5 RRU
## Indicators.
## ALM
## ACT
## VSWR
## CPRI0
## CPRI1

## NO TE
● The port for transmitting RET signals is determined by the software.
● The CPRI0 port is connected to the BBU by default in single-mode scenarios.
1.2.5 RRU Indicators
There are six indicators on an RRU. They indicate the running status of the RRU.
For detailed positions of the RRU indicators, see 1.2.4 RRU Ports.
The following table describes the RRU indicators.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.15

Table 1-2 RRU indicators
IndicatorColorStatusDescription
RUNGreenSteady onThere is power supply, but the board is
faulty.
Steady offThere is no power supply, or the board
is faulty.
Blinking (on for
1s and off for
## 1s)
The board is running properly.
Blinking (on for
0.125s and off
for 0.125s)
Software is being loaded to the board,
or the board is not started.
ALMRedSteady onAlarms are generated, and the module
must be replaced.
Blinking (on for
1s and off for
## 1s)
Alarms are generated. The alarms may
be caused by the faults on the related
boards or ports. Therefore, you need
to locate the fault before deciding
whether to replace the module.
Steady offNo alarm is generated.
ACTGreenSteady onThe module is working properly when
TX channels are enabled or when
software is being loaded to the
module that is not started.
Blinking (on for
1s and off for
## 1s)
The board is working properly with TX
channels disabled.
VSWRRedSteady offNo voltage standing wave ratio
(VSWR) alarm is generated.
Steady onVSWR alarms are generated on one or
more ports.
## CPRI0/
## CPRI1
Red or
green
Steady greenThe CPRI link is working properly.
Steady redAn optical module fails to receive or
transmit signals because the optical
module is faulty or the optical fiber is
broken.
Blinking red
(on for 1s and
off for 1s)
The CPRI link is out of lock because of
mutual lock of dual-mode clock
sources or mismatched data rates over
CPRI ports.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.16

IndicatorColorStatusDescription
Steady offThe optical module is not properly
installed.

## 1.2.6 Optical Modules
An optical module transmits optical signals between an optical port and an optical
fiber.
Optical modules can be classified into single-mode and multimode optical
modules, which can be distinguished as follows:
●  The puller of a single-mode optical module is blue and the puller of a
multimode optical module is black or gray.
●  The transmission mode is displayed as "SM" on the label of a single-mode
optical module and "MM" on the label of a multimode optical module.
Optical modules must be used in pairs on both ends of an optical fiber. The
following table describes the mapping.
## NO TICE
● Each type of optical module has its own mapping. If different types of optical
modules are used, performance risks may arise, for example, alarms, bit errors,
and interrupted links.
● To ensure that optical modules are connected and working properly, Huawei
equipment must be used with the original optical modules. As the compatibility
and quality of third-party optical modules cannot be guaranteed, using such
modules may cause connection exceptions or even damage to the main
equipment.
Table 1-3 Optical module mapping
## Optical Module Type
Mapping Between the BBU and RRU
SFP duplex (two-fiber
bidirectional, duplex for
short) optical module
SFP duplex optical modules with the same
specifications are used on both sides.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.17

Optical Module TypeMapping Between the BBU and RRU
SFP BIDI (single-fiber
bidirectional, BIDI for
short) optical module
SFP BIDI optical modules are used on both sides,
or the DSFP optical module is used on the BBU
side and the SFP BIDI optical module is used on
the RRU side.
● The receive and transmit wavelengths of an
optical module on both sides have the
mapping relationship. For example, if the
receive and transmit wavelengths of the optical
module on the BBU side are 1270TX/1330RX,
those on the RRU side are 1330TX/1270RX.
● Except for wavelengths, the specifications of
optical modules are the same.
For details about the DSFP optical module, see the
hardware description of the corresponding BBU.

The rate of the optical module to be installed must match the rate of the
corresponding port. When selecting an optical module with an appropriate rate,
consider factors such as carrier bandwidth, CPRI networking topology, CPRI
compression configuration, and capabilities of the baseband processing unit and
RF module. The following table lists the CPRI port rates supported by optical
modules with different rates. An RF module must be configured with an optical
module as required.
Table 1-4 CPRI port rates supported by optical modules
## Optical
## Module
## Type
CPRI Port Rate Supported or Not
## 1.25G2.5G4.9G6.1G9.8G10.1G24.3G
## 25G
optical
module
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Support
ed
## Support
ed
## Support
ed
## 10.1G/
## 9.8G
optical
module
## Not
support
ed
## Not
support
ed
## Support
ed
## Support
ed
## Support
ed
## Support
ed
## Not
support
ed
## 6G
optical
module
## Support
ed
## Support
ed
## Support
ed
## Support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## 4.9G
optical
module
## Support
ed
## Support
ed
## Support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## 2.5G
optical
module
## Support
ed
## Support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.18

## Optical
## Module
## Type
CPRI Port Rate Supported or Not
## 1.25G2.5G4.9G6.1G9.8G10.1G24.3G
## 1.25G
optical
module
## Support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed
## Not
support
ed

Table 1-5 Compliance standards for optical modules
ItemStandard
Safety standardIEC 60825-1
## IEC 62368-1
Storage environmentThe product must be stored in a dry and well-
ventilated environment with no corrosive gas in the
air. The temperature and humidity requirements are
as follows:
● Temperature: –10°C to 35°C (14°F to 95°F)
● Humidity: 20% RH to 75% RH
## NOTE
● The validity period is one year.
● The product can function properly within the validity
period if the storage environment meets the
preceding standards.

## NO TE
● The exteriors and labels of optical modules in this section are for reference only. The
actual exteriors and labels may be different.
● Only Huawei Wireless-certified optical modules can be used with Huawei wireless
equipment. The optical modules must meet the environment, feature, and specification
requirements of the equipment on which the optical modules are to be installed.
● Note that the supported maximum distances vary with optical modules. Select optical
modules based on application scenarios. For details, see "CPRI Optical Fiber" in "Base
## Station Cables".
SFP Optical Module
The following figure shows the exteriors of SFP optical modules.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.19

Figure 1-9 SFP optical modules
a: duplex optical moduleb: BIDI optical module
There is a label on each optical module, which provides information such as the
rate, wavelength, and transmission mode, as shown in the following figure.
Figure 1-10 Label structure
## (1) Rate
## (2) Wavelength(3) Transmission
distance
(4) Transmission mode

1.3 RRU Cables
This section describes RRU cables.
1.3.1 RRU Cable List
This section describes RRU cable connections.
The following table lists RRU cables.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.20

Table 1-6 RRU cable list
CableOne EndThe Other End
ConnectorConnected
## To...
ConnectorConnected
## To...
## RRU
## PGND
cable
OT terminal
(M6, 16 mm
## 2
[0.025 in.
## 2
## ])
## Ground
terminal on
the RRU
OT terminal (M8,
16 mm
## 2
## [0.025
in.
## 2
## ])
## Ground
terminal on
the ground
bar
## RRU
power
cable
Female fast
connector
(pressfit type
or screw-free
type)
NEG(-) and
RTN(+) on the
## RRU
Depending on
power equipment
## External
power
equipment
## CPRI
optical
fiber
## DLC
connector
● CPRI0 port
on the RRU
● CPRI1 port
on the RRU
DLC connector● CPRI port
on the
BBU or
CPRI1 port
on the
upper-level
## RRU
● CPRI0 port
on the
lower-level
RRU or
CPRI port
on the
## BBU
## RRU RF
jumper
4.3-10 male
connector
RF port on the
## RRU
4.3-10 male
connector or DIN
male connector
## NOTICE
Determine the
cable type based
on the connector
used at the other
end of the cable
on the live
network.
## Antenna
system
## RRU AISG
multi-wire
cable
## DB9
waterproof
male
connector
RET port on
the RRU
AISG standard
female connector
## AISG
standard
male
connector on
the RCU or
## AISG
extension
cable
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.21

CableOne EndThe Other End
ConnectorConnected
## To...
ConnectorConnected
## To...
## RRU AISG
extension
cable
## AISG
standard
male
connector
AISG standard
female
connector on
the AISG
multi-wire
cable
AISG standard
female connector
## AISG
standard
male
connector on
the RCU

1.3.2 RRU PGND Cable
A PGND cable connects an RRU and a ground bar, ensuring proper grounding of
the RRU. The maximum length of a PGND cable is 8 m (26.25 ft).
## Exterior
A PGND cable is green or green and yellow with an OT terminal at each end and a
cross-sectional area of 16 mm
## 2
(0.025 in.
## 2
). The following figure shows the
exterior of a PGND cable.
Figure 1-11 Exterior of a PGND cable
(1) OT terminal (M6, 16 mm
## 2
[0.025 in.
## 2
])(2) OT terminal (M8, 16 mm
## 2
[0.025 in.
## 2
## ])

## NO TE
● If the customer prepares the PGND cable, a copper-core cable with a cross-sectional
area of 16 mm
## 2
(0.025 in.
## 2
) or larger is recommended.
● One OT terminal must be added to each end of the PGND cable onsite.
● You can determine the color of the cable and whether to use corresponding two-hole
OT terminals based on local regulations.
The following figure shows a two-hole OT terminal.
Figure 1-12 Two-hole OT terminal
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.22


1.3.3 RRU Power Cable
The RRU power cable is a -48 V DC shielded cable. It feeds -48 V DC power to an
RRU. The maximum length supported by an RRU power cable is 100 m (328.08 ft).
## NO TE
● If a small integrated DC power supply device is provided by the customer, contact
Huawei engineers.
● If a power supply device is provided by the customer, the recommended specification of
the circuit breaker on this device is 25 A to 30 A.
## Exterior
The connector at one end of an RRU power cable is a female fast connector
(pressfit type or screw-free type) and the connector at the other end depends on
the power device. The connectors must be prepared onsite. Figure 1-13 and
Figure 1-14 show the cable exterior.
Figure 1-13 RRU power cable (pressfit type)
(1) -48 V DC power cable
(2) Shield layer(3) Female fast connector
(pressfit type)

Figure 1-14 RRU power cable (screw-free type)
(1) -48 V DC power cable
(2) Shield layer(3) Female fast connector
(screw-free type)
## Cable Description
The following table lists the specifications of the RRU power cable length and its
core wires.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.23

Table 1-7 Specifications of the RRU power cable length and its core wires
## RRU
## Model
## Power
## Supply
## Device
## Stan
dard
## Cable
## Length
## Cross-
## Sectional
Area of Core
## Wire
Number of
OCBs on the
RRU Side
## Outer
## Diamet
er of
## Power
## Cable
for RRU
## RRU5904
## ,
## RRU5904
w,
## RRU5304
## ,
## RRU5304
w,
## RRU5904
## N
## DCDU-1
## 2B/
## APM593
## 0/
## APM595
## 0H/
## APM595
## 0H-L
## (-48 V)
## Euro
pean
stan
dard
s
0 m to
70 m
(0 ft to
## 229.66
ft)
6 mm
## 2
(0.0093 in.
## 2
## )
09.9 mm
to 14.4
mm
(0.39 in.
to 0.57
in.)
71 m to
100 m
## (232.94
ft to
## 328.08
ft)
10 mm
## 2
(0.015 in.
## 2
## )
## ● 1 (when
round
power
cables are
used)
a
● This item
is not
required
when D-
type
power
cables are
used.
## Nort
h
## Ame
rican
stan
dard
s
0 m to
70 m
(0 ft to
## 229.66
ft)
5.3 mm
## 2
(0.0082 in.
## 2
## ,
## 10 AWG)
## 0
71 m to
100 m
## (232.94
ft to
## 328.08
ft)
8.2 mm
## 2
(0.013 in.
## 2
## , 8
## AWG)
## 0
a: 10 mm
## 2
(0.015 in.
## 2
) round power cables do not meet this RRU's requirements
for the outer diameter of power cables. Therefore, an OCB is required.

RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.24

## NO TE
● The power requirements for a DCDU-12B depend on its application scenarios and load
configurations. For details, navigate to 3900 & 5900 Series Base Station Model
Description > 5900 Series Base Stations > Power Requirements of a DBS5900 and
choose a related section based on the application scenario of the DCDU-12B.
● For details about the power requirements for an APM5930/APM5950H/APM5950H-L,
navigate to 3900 & 5900 Series Base Station Model Description > 5900 Series Base
Stations > Power Requirements of a DBS5900 and choose a related section.
The following table lists the wire colors of an RRU power cable.
Table 1-8 Wire colors of an RRU power cable
CableWireWire Color in Most
## Regions
Wire Color in Other
## Regions
## North
## American
## Standards
## European
## Standards
UKChina
RRU power
cable
RTN(+)BlackBrownBlueRed
NEG(-)BlueBlueGrayBlue

1.3.4 CPRI Optical Fiber
CPRI optical fibers are classified into multimode optical fibers and single-mode
optical fibers. They transmit CPRI or eCPRI signals.
A multimode optical fiber connects a BBU to an RRU or connects RRUs in a
cascade mode. The maximum length of a multimode optical fiber connecting a
BBU and an RRU is 150 m (492.12 ft). The default length of a multimode optical
fiber connecting RRUs in a cascade mode is 10 m (32.81 ft). If the distance
between two RRUs exceeds 10 m (32.81 ft), contact Huawei engineers.
The single-mode optical fiber can be divided into two types: single-mode optical
fiber directly connecting a BBU to an RRU or connecting RRUs in a cascade mode
(shortened to directly connected single-mode optical fiber) and single-mode
optical fiber connecting an ODF to a BBU or RRU (shortened to single-mode
pigtail). The length of the directly connected single-mode optical fiber cannot
exceed the maximum allowed distance between the BBU and RRU. The maximum
length of the single-mode pigtail between an ODF and a BBU is 20 m (65.62 ft).
The maximum length of the single-mode pigtail between an ODF and an RRU is
70 m (229.66 ft).
## NO TE
● The ODF is an outdoor transfer box for optical fibers, which interconnects the single-
mode pigtail and trunk single-mode optical fiber.
● The ODF and trunk single-mode optical fiber are provided by the customer and must
comply with the ITU-T G.652 standard.
● A multimode optical fiber is used together with a multimode optical module, and a
single-mode pigtail is used together with a single-mode optical module.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.25

## Selection Principle
The following table lists the principles for selecting CPRI optical fibers.
Table 1-9 Principles for selecting CPRI optical fibers
## Optical
## Fiber
## Length
a
## Data
## Rate
(Gbit/s)
of the
## Optical
## Module
Selection PrincipleConnects...to...Description
≤ 150 m
## (492.12
ft)
2.5 to
## 6.144
Multimode optical
fiber/Directly
connected single-
mode optical fiber
Connects a BBU
to an RRU or
AAU, or
connects RRUs
or AAUs in a
cascade mode
b
When multiple
RRUs or AAUs
are cascaded,
multimode
optical fibers
and single-mode
optical fibers can
be used
together.
9.8 to 25Directly connected
single-mode optical
fiber
≤ 20 km
## (12.43
mi.)
≤ 25Single-mode optical
fiber (single-mode
pigtail and trunk
single-mode optical
fiber)
Connects a BBU
to an RRU or
AAU, or
connects RRUs
or AAUs in a
cascade mode
The single-mode
pigtail at the
RRU/AAU or
BBU side is
connected to the
trunk single-
mode optical
fiber by using an
## ODF.
≤ 70 m
## (229.66
ft)
40/100OM3 multimode
optical fiber
Connects a BBU
to an AAU
## Short-distance
connection
between the
BBU and AAU
70 m to
100 m
## (229.66
ft to
## 328.08
ft)
40/100OM4 multimode
optical fiber
100 m
to 10
km
## (328.08
ft to
## 32808.4
0 ft)
## 40/50/1
## 00
Single-mode optical
fiber (single-mode
pigtail and trunk
single-mode optical
fiber)
Connects a BBU
to an RRU or
AAU, or
connects RRUs
or AAUs in a
cascade mode
The single-mode
pigtail at the
RRU/AAU or
BBU side is
connected to the
trunk single-
mode optical
fiber by using an
## ODF.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.26

## Optical
## Fiber
## Length
a
## Data
## Rate
(Gbit/s)
of the
## Optical
## Module
Selection PrincipleConnects...to...Description
a: The optical fiber length indicates the distance between the BBU and the first
RRU or AAU or the distance between two RRUs or AAUs.
b: The default length of a multimode optical fiber connecting RRUs in a cascade
mode is 10 m (32.81 ft). If the distance between two RRUs exceeds 10 m (32.81
ft), contact Huawei engineers.

## Exterior
Multimode optical fiber or directly connected single-mode optical fiber: It can
be a dual-core optical fiber with DLC connectors as shown in Figure 1-15 or a
single-core optical fiber with LC connectors as shown in Figure 1-16.
Figure 1-15 Dual-core optical fiber with DLC connectors
(1) DLC connector
(2) Breakout cable(3) Label on the breakout
cable

Figure 1-16 Single-core optical fiber with LC connectors
(1) LC connector
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.27

## NO TE
● When an optical fiber connects a BBU3900/BBU3910/BBU5900/BBU5910 to an RRU, the
breakout cables on the BBU side and on the RRU side are 0.34 m (1.12 ft) and 0.03 m
(0.098 ft), respectively.
● When an optical fiber connects a BBU3910A/BBU3910C/BBU5900C to an RRU, the
breakout cables on the BBU side and on the RRU side are both 0.03 m (0.098 ft).
● When an optical fiber connects RRUs in a cascade mode, the breakout cables on both
sides are 0.03 m (0.098 ft).
Single-mode pigtail: It has a DLC connector at one end and an FC, LC, or SC
connector at the other end, as shown in the following figure.
Figure 1-17 Single-mode pigtail
## (1) DLC
connector
## (2) Breakout
cable
(3) Label on
the breakout
cable
## (4) FC
connector
## (5) LC
connector
## (6) SC
connector

## NO TE
● When a single-mode pigtail connects a BBU to an ODF, the breakout cables on the BBU
side and ODF side are 0.34 m (1.12 ft) and 0.8 m (2.62 ft), respectively.
● When a single-mode pigtail connects an RRU to an ODF, the breakout cables on the
RRU side and ODF side are 0.03 m (0.098 ft) and 0.8 m (2.62 ft), respectively.
## Label Description
The following table describes the labels on the breakout cables of a CPRI optical
fiber and recommended cable connections.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.28

Table 1-10 Labels on the breakout cables of a CPRI optical fiber
Label on the
## Breakout
## Cable
## Installation Position
## Connection
Between a BBU
and an RRU or
Between an
OFD06 and an
## RRU
## Connection
Between RRUs
## Connection
Between a BBU or
RRU and an ODF
1ACPRI RX port on
the RRU
CPRI RX port on
## RRU 1
RX port on the BBU
or CPRI RX port on
the RRU
1BCPRI TX port on
the RRU
CPRI TX port on
## RRU 1
TX port on the BBU
or CPRI TX port on
the RRU
2AOFD06 or TX port
on the BBU
CPRI TX port on
## RRU 0
## ODF
2BOFD06 or RX port
on the BBU
CPRI RX port on
## RRU 0
## ODF

1.3.5 RRU RF Jumper
The RRU uses 1/2" RF jumpers for input and output of RF signals. A fixed-length
RF jumper used by an RRU is 2 m (6.56 ft), 3 m (9.84 ft), 4 m (13.12 ft), 6 m
(19.68 ft), or 10 m (32.81 ft). A variable-length RRU RF jumper has a maximum
length of 10 m (32.81 ft).
## NO TE
● When the distance between an RRU and an antenna is within 10 m (32.81 ft), one end of
the RF jumper is connected to an RF port at the bottom of the RRU, and the other end is
connected to the antenna.
● When the distance between an RRU and an antenna is greater than 10 m (32.81 ft), it is
recommended that one end of the RF jumper be connected to an RF port at the bottom of
the RRU, the other end be connected to one end of the feeder, and the other end of the
feeder be connected to the antenna.
● If the customer prepares the RF jumper, the length of the RF jumper should be as short as
possible and not exceed 2 m (6.56 ft).
● If feeders are used, the length of a feeder should not exceed 100 m (328.08 ft) and the
difference in the length between any two feeders connected to RF ports should not exceed 2
m (6.56 ft).
## Exterior
For an RF jumper, one end is connected to a 4.3-10 male connector, and the other
end is connected to a connector based on onsite requirements, which is a 4.3-10
male connector or DIN male connector.
Figure 1-18 shows the exterior of an RF jumper with two ends connected to
4.3-10 male connectors.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.29

Figure 1-18 RF jumper
(1) 4.3-10 male connector

1.3.6 RRU AISG Multi-Wire Cable
An AISG multi-wire cable connects an RRU to a remote control unit (RCU) to
transmit control signals from a base station to an RET antenna. This cable is
configured to transmit RS485 signals when the RRU is connected to an RET
antenna. The length of an AISG multi-wire cable is 5 m (16.40 ft), 10 m (32.81 ft),
or 20 m (65.62 ft).
## NO TE
An RCU is a driving motor used for the phase shifter in the RET antenna. It receives control
commands from a base station and runs the commands to drive the stepper motor. Using a
gear, the stepper motor drives the adjustable phase shifter in the antenna to change the
downtilt angle.
## Exterior
An AISG multi-wire cable has a DB9 waterproof male connector at one end and
an AISG standard female connector at the other end, as shown in Figure 1-19 or
## Figure 1-20.
Figure 1-19 AISG multi-wire cable (1)
(1) DB9 waterproof male connector
(2) AISG standard female connector

RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.30

Figure 1-20 AISG multi-wire cable (2)
(1) DB9 waterproof male connector(2) AISG standard female connector

## Pin Assignment
Table 1-11 describes the pin assignment for the wires of an AISG multi-wire cable.
Table 1-11 Pin assignment for the wires of an AISG multi-wire cable
X1 End (Pin of
the DB9
## Waterproof
## Male
## Connector)
X2 End (Pin of the
AISG Standard
## Female
## Connector)
## Core Wire
## Color
## Core Wire
## Description
## Core Wire
## Type
## X1.1X2.1
White and
blue
## +12V
## Twisted
pair
## Blue
X1.3X2.3White and
orange
## RS485 B
## Twisted
pair
X1.5X2.5OrangeRS485 A
X1.4X2.4White and
green
## GND-
X1.9 and X1.4 are
interconnected.
## --GND-
-X2.1 and X2.6 are
interconnected.
## -+12V-
-X2.4 and X2.7 are
interconnected.
## -GND-

1.3.7 RRU AISG Extension Cable
When the distance between an RRU and an RCU exceeds 5 m (16.40 ft), a 5-m
AISG multi-wire cable is not long enough to connect the RRU and the RCU. In this
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.31

case, an AISG extension cable is used to extend the AISG multi-wire cable for
transmitting RS485 signals. The length of an AISG extension cable is 15 m (49.21
ft).
## NO TE
● The AISG extension cable can be used only when the AISG multi-wire cable with a
length of 5 m (16.40 ft) is used.
● When the distance between an RRU and an RCU exceeds 5 m (16.40 ft), the AISG multi-
wire cable with a length of 10 m (32.81 ft) or 20 m (65.62 ft) is preferred. Connecting
them with the AISG multi-wire cable and the AISG extension cable is only a backup
solution.
## Exterior
An AISG extension cable has an AISG standard male connector on one end and an
AISG standard female connector on the other end, as shown in Figure 1-21.
Figure 1-21 AISG extension cable
(1) AISG standard male connector
(2) AISG standard female connector

## Pin Assignment
Table 1-12 describes the pin assignment for the wires of an AISG extension cable.
Table 1-12 Pin assignment for the wires of an AISG extension cable
X1 End (Pin
of the AISG
## Standard
## Male
## Connector)
X2 End (Pin
of the AISG
## Standard
## Female
## Connector)
## Core Wire
## Color
## Core Wire
## Description
## Core Wire
## Type
X1.1X2.1White and
blue
+12VTwisted pair
## Blue
X1.7X2.7White and
orange
DC ReturnTwisted pair
## Orange
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.32

X1 End (Pin
of the AISG
## Standard
## Male
## Connector)
X2 End (Pin
of the AISG
## Standard
## Female
## Connector)
## Core Wire
## Color
## Core Wire
## Description
## Core Wire
## Type
X1.3X2.3White and
green
RS485 BTwisted pair
X1.5X2.5GreenRS485 A
X1.6X2.6White and
brown
+24VTwisted pair
## Brown

1.4 RF Cable Connections for the RRU
RF cable connections for the RRU vary depending on the configurations of the
RRU and antenna. The RF cable connections in this document are for reference
only. The actual cable connections depend on onsite conditions.
Description of RF Cable Connections
This section describes the typical RF cable connections for the RRU serving a single
sector. The following table lists the typical RF cable connections for the RRU.
Table 1-13 Typical RF cable connections for the RRU
RRU Model
Typical ScenarioIllustration of Cable
## Connections
## RRU5904,
RRU5904w,
## RRU5304,
RRU5304w(2.6G),
## RRU5904N
1T1R+1T1R+1T1R+1T1RSee illustration 1 in Figure
## 1-22.
2T2RSee illustration 2 in Figure
## 1-22.
2T2R+2T2RSee illustration 3 in Figure
## 1-22.
## ● 2T4R
## ● 4T4R
See illustration 4 in Figure
## 1-22.

RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.33

Table 1-14 Typical RF cable connections for the RRU
RRU ModelTypical ScenarioIllustration of Cable
## Connections
RRU5304w(700M)2T2RSee illustration 2 in Figure
## 1-22.
2T2R+2T2RSee illustration 3 in Figure
## 1-22.
## ● 2T4R
## ● 4T4R
See illustration 4 in Figure
## 1-22.

Typical Illustration of Cable Connections
Figure 1-22 Typical RF cable connections for the RRU

1.5 RRU Auxiliary Devices
This section describes RRU auxiliary devices.
## Indoor Floor Installation Support
## ●IFS06
IFS06, an indoor floor installation support, is used for installing indoor RRUs.
For details about the exterior, specifications, and installation of an IFS06, see
IFS06 Hardware Description and IFS06 Installation Guide.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.34

## ●IFS5906
IFS5906, an indoor floor installation support, is used for installing indoor
blade RRUs.
IFS5906 is supported in V100R016C00 and later versions.
For details about the structure, functions, installation, and maintenance of an
IFS5906, see IFS5906 Hardware Description and IFS5906 Installation Guide.
## Outdoor Pole Support
OFP06, short for Outdoor Flexible Pole For 6, is an outdoor pole support and
provides a solution for extended installation of Huawei products on towers or
building tops.
For details about the exterior and installation of an OFP06, see
OFP06 User Guide.
## OCB
An outdoor cable conversion box (OCB) interconnects cables of different core
diameters. Power cables shipped with RRUs cannot support long-distance power
supply. Therefore, when power supply is far from the equipment, cables with large
core diameters are used, and an OCB connects these cables and RRU power
cables.
For details about the structure, functions, installation, and maintenance of an
OCB, see
OCB User Guide or OCB-01M User Guide.
## Power Module
A power module is used to convert external input power into -48 V DC or -57 V
DC for the DC RRU. The following power modules are available.
●  OPM15M (Ver.B): supported in V100R010C10 and later.
●  OPM50M (Ver.B): supported in V100R010C10 and later.
●  OPM200/OPM200 (Ver.B): supported in V100R015C10 and later.
For details about the structure, functions, installation, and maintenance of a
power module as well as its support for RRUs, see the user guide of the
corresponding power module.
## Fiber Distribution Box
The ODM03D is small distribution equipment, which supports RRU capacity
expansion, power cable reuse, and optical fiber reuse.
For details about the structure, functions, installation, and maintenance of an
ODM03D, see
ODM03D User Guide.
## RMU
The RMU3900A (shortened to RMU in this document) is a radio multiplex unit. It
converges and deconverges CPRI data to reduce the required CPRI optical fibers
between a BBU and RRUs.
The RMU3900A is supported in V100R012C00 and later versions.
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.35

For details about the structure, functions, installation, and maintenance of an
RMU3900A, see RMU3900A User Guide.
## MEB
The monitoring extension box (MEB) converts external RS485 communication
signals and dry contact alarm signals into power circuit signals, implementing
power supply monitoring. The following MEB models are available.
●  MEB06D: supported in V100R012C10 and later.
●  MEB06D (Ver.B): supported in V100R017C00 and later.
For details about the structure, functions, installation, and maintenance of an
MEB, see
MEB06D User Guide or MEB06D (Ver.B) User Guide.
## RFC5906
The RFC5906 is used in the DBS3900, DBS5900, BTS3900A, and BTS5900A base
stations to accommodate blade RRUs.
The RFC5906 is supported in V100R015C10 and later versions.
For details about the structure, functions, installation, and maintenance of an
RFC5906, see
RFC5906 User Guide.
## RPCU
The radio phase calibration unit (RPCU) is used with the RRU.
The RPCU is supported in V100R016C10 and later versions.
For details about the structure, functions, installation, maintenance, and other
information of an RPCU, see
RPCU (1700 MHz to 2700 MHz) User Guide or RPCU
(700 MHz to 2700 MHz) User Guide
## .
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w
## Hardware Description
## 1
RRU5904&RRU5904N&RRU5904w&RRU5304&RRU5
## 304w Hardware Description
Issue 17 (2025-06-24)Copyright © Huawei Technologies Co., Ltd.36