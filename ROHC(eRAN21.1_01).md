

eRAN
ROHC Feature Parameter
## Description
## Issue01
## Date2025-03-10
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
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 Change History.........................................................................................................................1
1.1 eRAN21.1 01 (2025-03-10)..................................................................................................................................................1
1.2 eRAN21.1 Draft B (2025-02-10)........................................................................................................................................ 1
1.3 eRAN21.1 Draft A (2024-12-31)........................................................................................................................................ 1
2 About This Document.............................................................................................................3
2.1 General Statements................................................................................................................................................................ 3
2.2 Applicable RAT......................................................................................................................................................................... 3
2.3 Features in This Document.................................................................................................................................................. 4
3 Overview....................................................................................................................................5
4 ROHC.......................................................................................................................................... 6
4.1 Principles.................................................................................................................................................................................... 6
4.1.1 Related Concepts................................................................................................................................................................. 6
4.1.2 Principles and Framework of ROHC..............................................................................................................................8
4.1.2.1 ROHC Entities in E-UTRAN........................................................................................................................................... 8
4.1.2.2 Basic Framework............................................................................................................................................................ 10
4.1.2.2.1 Compression Mechanism......................................................................................................................................... 10
4.1.2.2.2 Decompression Mechanism.................................................................................................................................... 11
4.1.2.2.3 Context Replication....................................................................................................................................................11
4.1.2.3 ROHC States.................................................................................................................................................................... 12
4.1.2.3.1 Compressor States......................................................................................................................................................12
4.1.2.3.2 Decompressor States................................................................................................................................................. 12
4.1.2.4 ROHC Operating Modes.............................................................................................................................................. 13
4.1.2.4.1 Operating Mode Transition..................................................................................................................................... 13
4.1.2.4.2 U-Mode.......................................................................................................................................................................... 14
4.1.2.4.3 O-Mode..........................................................................................................................................................................15
4.1.2.4.4 R-Mode...........................................................................................................................................................................16
4.1.2.5 Factors Affecting the ROHC Efficiency................................................................................................................... 17
4.1.3 ROHC Procedure and Parameter Negotiation.........................................................................................................18
4.1.3.1 Procedure for Starting ROHC upon Initial Access...............................................................................................18
4.1.3.2 Procedure for ROHC During a Handover...............................................................................................................20
4.1.3.3 Procedure for ROHC upon RRC Connection Reestablishment........................................................................22
4.2 Network Analysis.................................................................................................................................................................. 22
eRAN
ROHC Feature Parameter DescriptionContents
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.iii

4.2.1 Benefits................................................................................................................................................................................. 22
4.2.2 Impacts..................................................................................................................................................................................23
4.3 Requirements......................................................................................................................................................................... 24
4.3.1 Licenses................................................................................................................................................................................. 24
4.3.2 Functions.............................................................................................................................................................................. 24
4.3.2.1 Prerequisite Functions.................................................................................................................................................. 24
4.3.2.2 Mutually Exclusive Functions..................................................................................................................................... 24
4.3.2.3 Function Impacts............................................................................................................................................................25
4.3.3 Hardware..............................................................................................................................................................................27
4.3.4 Others....................................................................................................................................................................................27
4.4 Operation and Maintenance.............................................................................................................................................27
4.4.1 Data Configuration........................................................................................................................................................... 27
4.4.1.1 Data Preparation............................................................................................................................................................ 27
4.4.1.2 Using MML Commands............................................................................................................................................... 29
4.4.1.3 Using the MAE-Deployment...................................................................................................................................... 29
4.4.2 Activation Verification......................................................................................................................................................29
4.4.3 Network Monitoring.........................................................................................................................................................32
5 Parameters..............................................................................................................................35
6 Counters.................................................................................................................................. 36
7 Glossary................................................................................................................................... 37
8 Reference Documents...........................................................................................................38
eRAN
ROHC Feature Parameter DescriptionContents
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.iv

## 1 Change History
This chapter describes changes not included in the "Parameters", "Counters",
"Glossary", and "Reference Documents" chapters. These changes include:
●  Technical changes
Changes in functions and their corresponding parameters
●  Editorial changes
Improvements or revisions to the documentation
1.1 eRAN21.1 01 (2025-03-10)
This issue does not include any changes.
1.2 eRAN21.1 Draft B (2025-02-10)
This issue includes the following changes.
## Technical Changes
## None
## Editorial Changes
Added descriptions of ROHC during intra-cell handovers. For details, see 4.1.3.2
Procedure for ROHC During a Handover.
Revised other descriptions in this document, which do not involve changes in
meanings and therefore are not detailed.
1.3 eRAN21.1 Draft A (2024-12-31)
This issue introduces the following changes to eRAN20.1 01 (2024-03-09).
## Technical Changes
## None
eRAN
ROHC Feature Parameter Description1 Change History
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.1

## Editorial Changes
Revised descriptions in this document, which do not involve changes in meanings
and therefore are not detailed.
eRAN
ROHC Feature Parameter Description1 Change History
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.2

## 2 About This Document
## 2.1 General Statements
## Purpose
This document is intended to acquaint readers with:
●  The technical principles of features and their related parameters
●  The scenarios where these features are used, the benefits they provide, and
the impact they have on networks and functions
●  Requirements that must be met before feature activation
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
This document applies to TDD.
eRAN
ROHC Feature Parameter Description2 About This Document
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.3

2.3 Features in This Document
This document describes the following TDD features.
Feature IDFeature NameChapter/Section
TDLOFD-001017RObust Header
## Compression
## (ROHC)
## 4 ROHC
eRAN
ROHC Feature Parameter Description2 About This Document
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.4

## 3 Overview
ROHC provides a header compression mechanism for data packets. It is specially
designed for lowering the bit error rate and delay of radio links and saving radio
resources.
This feature is applicable in the following scenarios:
●  Voice packet header compression
This compression applies to QCI 1 voice bearers, QCI 65 and QCI 66 bearers
for PTT services, or extended QCI bearers for PTT services.
●  Uplink Transmission Control Protocol (TCP)/IP packet header decompression
This decompression applies to services in acknowledged mode (AM) on the
Radio Link Control (RLC) layer. This decompression does not apply to QCI 1
voice bearers, QCI 65 and QCI 66 bearers for PTT services, or extended QCI
bearers for PTT services.
The ROHC-TCP function decompresses the headers of uplink TCP/IP packets.
eRAN
ROHC Feature Parameter Description3 Overview
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.5

## 4 ROHC
## 4.1 Principles
ROHC reduces header overheads and packet loss and shortens the response time,
improving network performance. ROHC has the following advantages over other
header compression mechanisms, such as IP Header Compression (IPHC):
●  High reliability:
Due to its feedback mechanism, ROHC is robust on the radio links with high
BERs and long RTT.
●  High compression efficiency:
Some simple header compression algorithms, such as IPHC and Compressed
Real-Time Transport Protocol (CRTP), can compress the header to 2 bytes,
while ROHC can compress headers into only 1 byte.
As shown in Figure 4-1, the header is compressed from 40 bytes to 1 byte. A
smaller payload increases gains from ROHC header compression.
Figure 4-1 ROHC header compression
Despite that ROHC is more complex than other header compression schemes and
requires higher computing capabilities of a processor, it is suitable in radio systems
where air interface resources are more valuable. It is mainly used for voice over IP
(VoIP) or TCP/IP services.
## 4.1.1 Related Concepts
Table 4-1 explains the concepts related to ROHC.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.6

Table 4-1 Concepts related to ROHC
ConceptExplanation
CompressorIt is at the transmit (TX) end, and is responsible for
compressing the packet header based on the profile and the
context.
DecompressorIt is at the receive (RX) end, and is responsible for restoring the
packet header based on the profile and the context.
Data radio
bearer (DRB)
A DRB is a radio bearer that carries data on the user plane.
● Multiple DRBs can be established between a UE and the E-
## UTRAN.
● Each DRB can carry one or more packet flows.
Packet flowA packet flow is a series of data packets using the same
compression algorithm and associated with a single context.
For example, a voice over Long Term Evolution (VoLTE) service
is composed of two packet flows, of which one is compliant
with the Real-Time Transport Protocol (RTP) and the other is
compliant with the RTP Control Protocol (RTCP).
ContextA context contains the information about compression and
decompression characteristics of a packet header. Each context
is identified by a unique context identifier (CID).
● Each context consists of static and dynamic fields.
– Static fields, such as the source and destination IP
addresses, remain unchanged within a particular packet
flow. Static fields are sent only when the compressor is in
the Initialization and Refresh (IR) state.
– Dynamic fields, such as the serial number, change based
on certain rules. Dynamic fields need to be updated in
real time.
For details, see A.1 "General classification" in IETF RFC 3095.
● The number of concurrently activated contexts depends on
the processing capabilities of the compressor and
decompressor. The maximum number of contexts that an
eNodeB or a UE supports is user-defined. When ROHC is
enabled, the compressor and decompressor must negotiate
the maximum number of contexts.
– For VoIP services, the number of contexts for each bearer
that a Huawei eNodeB supports meets a VoLTE service
compressing requirement.
– For TCP/IP services, a Huawei eNodeB supports a
maximum of 16 contexts for each bearer.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.7

ConceptExplanation
ProfileROHC is an extensible framework consisting of different profiles
for packet flows compliant with different protocols. Profiles
define the compression modes for packet flows with different
types of protocol headers. Each profile is identified by a profile
ID. Profile 0x0000 indicates that packet headers are not
compressed.

Table 4-2 maps profile IDs to their corresponding protocols. Descriptions of
profiles 0x0003 and 0x0004 in this document apply only to macro and LampSite
eNodeBs.
Table 4-2 Mapping between profile IDs and protocols
Profile IDProtocolRemarks
0x0001RTP, User
## Datagram
## Protocol
(UDP), and IP
For details, see RFC 3095 and RFC 4815.
0x0002UDP and IP
0x0003Encapsulating
## Security
Payload (ESP)
and IP
0x0004IPFor details, see RFC 3843 and RFC 4815.
0x0006TCP/IPFor details, see RFC 6846 and RFC 5795.

## NO TE
ROHC can be used for Internet Protocol version 4 (IPv4) and Internet Protocol version 6
(IPv6) headers.
4.1.2 Principles and Framework of ROHC
4.1.2.1 ROHC Entities in E-UTRAN
The ROHC entities are located in the user-plane PDCP entities in the UE and
eNodeBs. Figure 4-2 shows the locations of the PDCP entities in the protocol
stacks of the UE and eNodeB.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.8

Figure 4-2 Locations of the PDCP entities
As shown in Figure 4-3, ROHC entities are used only for header compression and
decompression for data packets on the user plane. When DRBs between the UE
and eNodeB are already established, the UE and eNodeB can implement ROHC in
each DRB independently.
Figure 4-3 ROHC in PDCP
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.9

## NO TE
In this figure, "Packets not associated with any PDCP SDU" provides decompression
feedback.
For downlink services, the compressor is located within the eNodeB, and the
decompressor is located within the UE. For uplink services, the compressor is
located within the UE, and the decompressor is located within the eNodeB.
## 4.1.2.2 Basic Framework
The ROHC framework defines the mechanism for header compression and
decompression. Figure 4-4 shows the framework of ROHC that uses profile
## 0x0001.
●  The compressor sends the header-compressed data packets (including the
information about the header compression).
●  The compressor and decompressor maintain the context at the TX and RX
ends respectively to ensure the context consistency.
●  The decompressor restores the data packets based on the context.
Figure 4-4 ROHC framework
## 4.1.2.2.1 Compression Mechanism
## Normal Compression
The normal header compression mechanism of ROHC is as follows:
-  The compressor identifies a packet flow based on the source IP address,
destination IP address, port number, and supported profile. Each packet flow
is associated with a context, which describes the characteristics of the header
fields in the flow-specific packets.
-  Based on the field characteristics, the compressor selects different coding
schemes, such as least significant bit (LSB) or Window-based LSB.
-  The compressor sends the IR packets to the decompressor to establish the
context for decompression. The context on the decompressor side is identical
to that on the compressor side for a given packet flow.
-  The compressor compresses the packet headers and transmits the packets.
-  If the compressor detects that the context has changed or receives feedback
from the decompressor that the decompression has failed, the compressor
sends updated information to the decompressor for context synchronization.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.10

## NO TE
●  An IR packet, containing the profile and context, is sent only when no context is
established or needs to be updated.
●  To prevent errors from propagating, the compressor can add cyclic redundancy
check (CRC) fields to compressed packets for the decompressor to detect errors.
●  When a DRB carries more than one packet flow, each packet flow carries its
associated CID to inform the decompressor of its context.
## List Compression
Certain information from packet headers to be compressed may be ordered into a
list, such as an RTP contributing source (CSRC) and TCP Option lists. ROHC list
compression applies to ordered lists, which are constant between packets. Figure
4-5 presents the list structure.
Figure 4-5 List structure
The basic principle for list compression is as follows:
●  When a list remains unchanged for packets, compressed headers do not
include the list information.
●  Small changes in the list are represented in compressed headers as additions
(Insertion scheme), or deletions (Removal scheme), or both (Remove Then
Insert scheme).
●  The list can also be sent in its entirety (Generic scheme). This scheme is used
during context setup for ROHC or as required by the compressor.
Huawei eNodeBs support ROHC list compression only for RTP CSRC and TCP
Option lists.
## 4.1.2.2.2 Decompression Mechanism
The header decompression mechanism of ROHC is as follows:
-  The decompressor receives the IR packets sent by the compressor to establish
the context.
-  The decompressor receives data packets with compressed headers,
decompresses the headers based on the context, sends the successfully
decompressed packets to the upper layer, and sends feedback to inform the
compressor of successful decompression. If the decompression fails, the
decompressor discards the packets and informs the compressor of the failure.
-  When the compressor updates the context, the decompressor receives the
update information and updates the context.
## 4.1.2.2.3 Context Replication
Context replication is an optional mechanism for ROHC-TCP context initialization.
The eNodeB supports ROHC-TCP context replication. For short-lived TCP flows, the
eNodeB can establish new contexts based on the existing contexts, reducing the
overhead during context setup.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.11

For details about the state transition mechanism of context replication, see "State
Machine with Context Replication" in IETF RFC 4164.
4.1.2.3 ROHC States
## 4.1.2.3.1 Compressor States
The ROHC compressor may operate in any of the following states:
●  IR state
The IR state ranks the lowest. The compressor operates in this state when the
static part of the context on the decompressor side is not established yet or if
the decompression fails due to decompressor issues. In this state, only IR
packets (including uncompressed data packets and the compression context)
are sent.
●  First Order (FO) state
When the compressor detects any changes in the dynamic fields of the packet
flow, the compressor enters this state and sends the compressed packets.
●  Second Order (SO) state
This is the optimal compression state, in which the compressor sends the data
packets with the maximum compression efficiency. The compressor operates
in this state in most cases.
The compressor initially operates in the lowest compression state (IR) and
switches gradually to higher compression states (FO and SO). The compressor
makes decisions about compression state transitions based on the following
criteria:
●  Variations in the static part or dynamic part of packet headers
●  Feedback from the decompressor (ACK or NACK)
●  Periodic timeout
State transition of the compressor is related to the operating mode of ROHC. For
the compressor's state transition in different operating modes, see 4.1.2.4 ROHC
## Operating Modes.
## 4.1.2.3.2 Decompressor States
The ROHC decompressor operates in any of the following states:
## ●  No Context
If the context is not established yet or is unusable on the decompressor side,
the decompressor operates in the No Context state.
## ●  Static Context
The decompressor enters this state when detecting that the dynamic fields in
the context are invalid.
## ●  Full Context
The decompressor enters this state after a complete context is established
based on successful decompression of a data packet. In this state, the
decompressor can decompress the data packets compressed with the
maximum compression efficiency.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.12

For the state transition of the decompressor, see Figure 4-6.
Figure 4-6 State transition of the decompressor
●  The decompressor initially operates in the No Context state. It enters the Full
Context state when the IR packet is successfully decompressed and a
complete context is established.
●  The decompressor switches to the Static Context state from the Full Context
state when the dynamic fields in the context become invalid.
●  In the Static Context state, the decompressor can switch back to the Full
Context state after restoring the context, or to the No Context state if the
static fields in the context also become invalid.
4.1.2.4 ROHC Operating Modes
ROHC operates in Unidirectional Mode (U-Mode), Bidirectional Optimistic Mode
(O-Mode), or Bidirectional Reliable Mode (R-Mode). The ROHC reliability and
overheads used for transmitting feedback differ between modes.
## 4.1.2.4.1 Operating Mode Transition
●  For VoIP services, ROHC has the following benefits:
The initial operating mode of the compressor is U-Mode. After confirming
packet reception by the decompressor and receiving the expected-mode
indication from the decompressor, the compressor switches to O-Mode or R-
Mode. The decompressor determines the operating mode transition.
–   When the eNodeB is the compressor, the UE functions as the
decompressor and triggers operating mode transition for the eNodeB.
–   When the eNodeB is the decompressor, it determines the target operating
mode based on the PdcpRohcPara.
HighestMode parameter and
instructs the UE to change the operating mode.
▪If the PdcpRohcPara.
HighestMode parameter is set to R_MODE, the
UE can switch to a higher mode (O-Mode or R-Mode) and stay in R-
## Mode.
▪If the PdcpRohcPara.
HighestMode parameter is set to O_MODE,
the UE can switch to and stay in O-Mode.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.13

●  For TCP/IP services, ROHC has the following benefits:
The initial operating mode of the compressor is U-Mode. After confirming
packet reception by the decompressor and receiving the expected-mode
indication from the decompressor, the compressor switches to O-Mode. The
operating mode transition is implemented by periodically updating the
contexts and using the optimal method to reduce the transmission data,
improving the compression efficiency.
–   Periodic context update
Before a feedback channel is established, the compressor switches back
to a lower state periodically and sends IR/IR-DYN (dynamic) data packets.
The compressor updates the contexts periodically until the feedback
channel is established.
–   Optimal method
▪When the compressor sends to the decompressor for the first time,
IR/IR-CR packets are sent.
▪Before confirming packet reception by the decompressor, the
compressor transmits the packet with least changed fields if a field
changes.
## NO TE
The eNodeB exits ROHC in any of the following scenarios:
●  Excessive packet loss times on the eNodeB
●  Excessive UE decompression failures
●  System overload
If ROHC works in O-Mode or R-Mode, the eNodeB exits ROHC when it fails to decompress
packets for an excessive number of times.
When the eNodeB exits ROHC, ROHC parameters are re-negotiated only during inter-cell
handovers and reestablishments (corresponding to steps 2 to 3 in Figure 4-11). For details,
see 4.1.3.2 Procedure for ROHC During a Handover and 4.1.3.3 Procedure for ROHC
upon RRC Connection Reestablishment.
4.1.2.4.2 U-Mode
In U-Mode, packets can be sent only from the compressor to the decompressor.
Feedback channels are not mandatory. Compared with O-Mode and R-Mode, U-
Mode has the lowest reliability but requires the minimum overheads for feedback.
In U-Mode, the compressor sends a data packet carrying the context for many
times to ensure that the context on the decompressor side is synchronized. In
addition, the compressor periodically switches to a lower state to ensure the
context synchronization even in error conditions. Figure 4-7 shows the state
transition of the compressor in U-Mode.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.14

Figure 4-7 State transition of the compressor in U-Mode
The compressor initially operates in the IR state. With the optimistic approach, the
compressor switches to a higher state. State transition happens when the
compressor confirms that the decompressor has received the context after sending
the data packets containing the context information for multiple times.
If the compressor is informed that the decompressor has received some of the
packets, the compressor in the IR state switches to the FO state. If the compressor
confirms that the decompressor has received all packets, the compressor switches
to the SO state.
Decompression may fail if the decompressor does not receive enough packets
containing the context. Therefore, the compressor must periodically switch back to
a lower state. In the FO state, the compressor periodically switches back to the IR
state. In the SO state, the compressor periodically switches back to the FO or IR
state. If the packet header needs to be updated, the compressor in the SO state
switches back to the FO state.
4.1.2.4.3 O-Mode
In O-Mode, the decompressor can inform the compressor of successful or failed
context synchronization. O-Mode uses the context transmission method and
feedback information of U-Mode. Therefore, it provides higher reliability than U-
Mode and leads to less feedback than R-Mode.
Figure 4-8 shows the state transition of the compressor in O-Mode.
●STATIC_NACK means that there is no context or the static fields of the
context are invalid.
●NACK means that dynamic fields of the context are invalid.
●ACK means that the decompressor has successfully received the packets from
the compressor.
●Update means that the decompressor is informed that the packet headers are
updated.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.15

Figure 4-8 State transition of the compressor in O-Mode
The compressor initially operates in the IR state and later switches to a higher
state (FO or SO) based on the optimistic approach principle or after receiving an
ACK message from the decompressor. If the compressor in a higher state receives
a STATIC_NACK message, it switches back to the IR state. If a compressor in the
SO state is informed of a need for an update in packet headers, it switches to the
FO state.
ROHC feedback enhancement in O-Mode can adjust the feedback mechanism to
restore contexts of the UE and eNodeB as soon as possible, reducing the ROHC
decompression failure rate.
●  When this function is enabled, the eNodeB immediately sends NACK or
STATIC_NACK messages to the UE after failing to decompress packets.
●  When this function is disabled, the eNodeB sends NACK or STATIC_NACK
messages to the UE after a certain number of packets fail to be
decompressed.
ROHC feedback enhancement in O-Mode is specified by the
ROHC_FEEDBACK_ENHANCEMENT_SW option of the
PdcpRohcPara.
RohcOptimizationSwitch parameter.
4.1.2.4.4 R-Mode
In R-Mode, sending feedback is the only method to ensure context synchronization
between the compressor and decompressor. The compressor repeatedly sends the
context updating packets until receiving acknowledgment from the decompressor.
R-Mode leads to greatest amount of acknowledgment data and largest link
overhead, but provides the most reliable contexts.
Figure 4-9 shows the state transition of the compressor in R-Mode.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.16

Figure 4-9 State transition of the compressor in R-Mode
The compressor initially operates in the IR state and later switches to a higher
state (FO or SO) based on the received ACK message from the decompressor. If
the compressor in a higher state receives a STATIC_NACK message, it switches
back to the IR state. If a compressor in the SO state is informed of a need for an
update in packet headers, it switches to the FO state.
4.1.2.5 Factors Affecting the ROHC Efficiency
The factors affecting the ROHC efficiency can be classified into controllable or
uncontrollable ones by the eNodeB.
●  Of the uncontrollable factors, the most significant are those having to do with
the service data. These factors are also the primary elements impacting ROHC
efficiency. They include:
–   Header format of the data packets on a DRB
The header format determines the ROHC efficiency. The UE or the
eNodeB compresses the packet headers based on the header format
using an appropriate profile. In most cases, packets with larger-sized
headers have higher compression efficiency.
–   Payload of each data packet on a DRB
The smaller the payload of a packet, the higher the proportion of headers
to the total data traffic and the higher the ROHC efficiency.
–   Number of packet flows on a DRB
If the number of packet flows exceeds the maximum number of ROHC
CIDs supported by the UE or eNodeB, the UE or eNodeB can compress
the packet headers only in some packet flows. In this situation, the ROHC
efficiency decreases.
–   Method used to handle data packet headers at the application layer
If UDP is used to transmit data at the application layer, the ROHC
efficiency drops when the UDP header checksum mechanism is enabled.
–   Operating mode of ROHC used in the downlink
This mode is determined by UEs. In U-Mode, the compressor periodically
switches to a lower state, which decreases the compression efficiency. In
O-Mode or R-Mode, the compressor does not need to periodically switch
to a lower state, which helps increase the compression efficiency.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.17

●  The controllable factors include:
–   Operating mode of ROHC used in the uplink
This mode is determined by eNodeBs. In U-Mode, the compressor
periodically switches to a lower state, which decreases the compression
efficiency. In O-Mode or R-Mode, the compressor does not need to
periodically switch to a lower state, which helps increase the compression
efficiency.
–   Lower-layer transmission quality
In O-Mode or R-Mode, if a compressed packet fails to be decompressed
or a decompressed packet fails CRC, the decompressor sends a NACK
message to the compressor, and then the compressor switches to a lower
state. In this case, the compression efficiency decreases. Better lower-
layer transmission quality leads to a lower probability of decompression
failures or CRC failures and higher compression efficiency.
4.1.3 ROHC Procedure and Parameter Negotiation
ROHC starts when the EPC initiates DRB setup for VoIP services. When the DRBs
are established, the eNodeB and UE begin to negotiate ROHC parameters. After
the parameter negotiation, the compressor or the decompressor performs header
compression or decompression based on the negotiated ROHC parameters.
4.1.3.1 Procedure for Starting ROHC upon Initial Access
If both the compressor and the decompressor support ROHC and ROHC is
enabled, ROHC starts by default when a VoIP service bearer is set up during initial
access of a UE. For TCP/IP services, ROHC is started only when coverage is weak.
The EPC sends an E-RAB SETUP REQUEST message over the S1 interface,
requesting that the eNodeB set up DRBs for data transmission on the user plane
and start ROHC. Figure 4-10 shows the procedure for starting ROHC.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.18

Figure 4-10 Procedure for starting ROHC upon initial access
-  ROHC is specified by CellAlgoSwitch.RohcSwitch and corresponding
PdcpRohcPara.
## Profiles.
-  For VoIP services, go to step 3 in Figure 4-10 when a VoIP service bearer is set
up.
For TCP/IP services, determine whether the coverage is weak. The threshold
for determining weak coverage is specified by the
PdcpRohcPara.
RohcTcpSinrTriggerThld parameter. If the SINR measured by
the UE is less than or equal to the threshold specified by the
PdcpRohcPara.
RohcTcpSinrTriggerThld parameter, the next step is
performed. Otherwise, ROHC-TCP is not started.
-  The ROHC capability of a UE includes the maximum number of concurrent
contexts (MAX_CID) and the profiles supported by the UE. The UE informs the
EPC about its ROHC capability during the initial registration.
The eNodeB can acquire the profiles supported by the UE from the EPC or
directly from the UE. After the RRC connection is set up, the EPC sends an
Initial Context Setup Request message over the S1 interface to inform the
eNodeB of the UE radio capability reported by the UE during initial
registration. If the eNodeB fails to obtain the UE's ROHC capability
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.19

information from the EPC, the eNodeB sends a UE Capability Enquiry message
over the Uu interface to query the UE's ROHC capability.
-  The eNodeB compares the MAX_CID in the ROHC capability information
reported by the UE with the eNodeB-supported maximum number of
concurrently active contexts per UE, and chooses the smaller one as the
maximum number of concurrent contexts supported by the UE.
-  The eNodeB identifies the UE-supported profiles using the intersection of the
following two profiles:
–   UE-supported profiles stored on the eNodeB
–   eNodeB-supported profiles specified by the PdcpRohcPara.
## Profiles
parameter
## NO TE
If the compressor and decompressor support any of the profiles listed in Table 4-2,
they support profile 0x0000.
-  The eNodeB reallocates the number of concurrent contexts for each DRB of
the UE based on the maximum number of concurrent contexts supported by
the UE. Then, the eNodeB sends the reallocated number of concurrent
contexts and the determined profiles as the ROHC parameters to the UE
through the Uu interface.
## NO TE
The reallocation of the number of concurrent contexts does not lead to a change in
the number of concurrent contexts already allocated for the UE's DRBs.
The eNodeB can use an RRCConnectionReconfiguration or
RRCConnectionReestablishment message to inform the UE of the negotiated ROHC
parameters.
-  After ROHC is started, the compressor and decompressor operate within the
ROHC framework for both the uplink and downlink.
4.1.3.2 Procedure for ROHC During a Handover
●  If an intra-cell handover is triggered by the exit of ROHC, ROHC parameters
are removed during the handover. If an intra-cell handover is triggered by
other reasons, ROHC parameters remain unchanged and do not need to be
renegotiated.
●  In the case of inter-cell handovers, the ROHC parameters need to be
renegotiated.
–   For an intra-base-station handover, the source cell notifies the UE of the
new ROHC parameters of the target cell through RRC reconfiguration. For
details about how to calculate the new ROHC parameters of the target
cell, see 4.1.3.1 Procedure for Starting ROHC upon Initial Access.
–   In an inter-base-station handover, the source eNodeB notifies the target
eNodeB of the ROHC capability of the UE, and the target eNodeB
recalculates the ROHC parameters. After the handover, the UE and the
target eNodeB operate with the new ROHC parameters. Figure 4-11
shows the detailed procedure.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.20

Figure 4-11 Procedure for ROHC during an inter-base-station handover
i.   The UE sends a measurement report in the source cell.
ii.  The source eNodeB makes a handover decision. If the eNodeB
decides to perform the handover, it sends a Handover Request
message including the UE's ROHC capability information to the
target eNodeB.
iii.  After deciding to admit the handed-over UE, the target eNodeB
calculates the ROHC parameters supported by both the UE and the
target eNodeB. Then, the target eNodeB sends a Handover Request
Acknowledge message carrying the new ROHC parameters to the
source eNodeB. For details about the procedure for calculating the
new ROHC parameters of the target eNodeB, see 4.1.3.1 Procedure
for Starting ROHC upon Initial Access.
iv.  The source eNodeB sends an RRC Connection Reconfiguration
message to instruct the UE to perform the handover. The message
carries the new ROHC parameters sent by the target eNodeB.
v.  The UE attempts to access the target cell.
vi.  After the UE successfully accesses the target cell, the UE and the
target eNodeB begin data transmission on the user plane using the
new ROHC parameters.
## NO TE
●  During an intra- or inter-base-station handover, the source cell does not transmit
the ROHC context to the target cell. The eNodeB reestablishes the corresponding
context if the target cell decides to start ROHC.
●  If the X2 interface is not set up between the source and target eNodeBs, the
handover is performed over the S1 interface. In this case, the ROHC parameter
negotiation process is the same as that performed over the X2 interface.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.21

4.1.3.3 Procedure for ROHC upon RRC Connection Reestablishment
The ROHC procedure for RRC connection reestablishment varies according to
target cells.
●  If an RRC connection is reestablished with the same cell, the original context
for ROHC is retained.
●  If an RRC connection is reestablished with another cell, the original context
for ROHC needs to be renegotiated.
●  If an RRC connection is reestablished with a cell served by another Huawei
eNodeB, the target eNodeB sends a Huawei proprietary message to the
source eNodeB to learn the UE's ROHC capability and then calculates the
ROHC parameters. If the settings of new ROHC parameters differ from those
of the original ones, the target eNodeB informs the UE of the new parameters
in the first RRC_CONN_RECFG message after the RRC connection is
reestablished.
## NO TE
If an RRC connection is reestablished with a cell served by another eNodeB deployed
by a different vendor, the procedure for ROHC upon RRC connection reestablishment
will fail.
## 4.2 Network Analysis
## 4.2.1 Benefits
●  For VoIP services, ROHC has the following benefits:
–   Compresses the headers of voice packets. If all the UEs on the live
network support ROHC, the compression efficiency can reach 15%.
–   Reduces the amount of data transmitted over the air interface. For voice
service users at the cell edge, it helps to reduce the number of Radio Link
Control (RLC) segments and decrease the voice packet delivery delay. It
can increase the uplink coverage by about 1 dB to 2 dB and ensure voice
quality, for example, maintaining the voice quality at a mean opinion
score (MOS) of 3.0. The uplink packet loss rate of users at the cell edge
decreases.
Packet loss rate = L.Traffic.UL.FarUE.PktLoss.Loss.QCI.1/
L.Traffic.UL.FarUE.PktLoss.Tot.QCI.1 x 100%
–   Reduces the average number of resource blocks (RBs) used for a single
voice service user. For example, if voice service users with 12.65 kbit/s
Adaptive Multirate (AMR) transmission are evenly distributed in a cell,
the number of RBs used for these users will be reduced by about 20% on
average after ROHC is enabled. The RBs saved by ROHC can be used to
increase the data service throughput of the cell or the number of voice
service users in the cell. The amount of the increase depends on many
factors, such as:
▪User locations
▪User quantity
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.22

▪User data service model (such as full buffer and burst services)
▪RB usage
▪Availability of PDCCH control channel elements (CCEs)
▪ROHC operating mode
▪ROHC efficiency
▪Support and compatibility of UEs for ROHC
▪AMR used for voice service users
Average number of uplink RBs used for a single voice service user =
L.ChMeas.PRB.UL.DrbUsed.Avg.VoIP/L.Traffic.User.VoIP.Avg
Average number of downlink RBs used for a single voice service user =
L.ChMeas.PRB.DL.DrbUsed.Avg.VoIP/L.Traffic.User.VoIP.Avg
The increase in the data service throughput of a cell is positively
correlated with the number of RBs used for data service users if all the
following conditions are met:
## ▪
RBs of a cell are limited.
## ▪
PDCCH CCEs in the cell are sufficient.
## ▪
ROHC works properly.
## ▪
Users are evenly distributed and require a large data service volume
in the cell.
●  For TCP/IP services, ROHC has the following benefits:
–   Compresses the headers of uplink TCP packets. If all the UEs on the live
network support ROHC, the compression efficiency can reach 20% to
## 50%.
–   Reduces the amount of data transmitted over the air interface. For uplink
TCP/IP services in weak coverage networks, it helps to reduce the number
of RLC segments and improve the user throughput and uplink coverage
by about 2 dB to 3 dB.
–   Reduces the RBs used for voice service users. For UEs supporting ROHC-
TCP, the number of RBs used for these UEs will be reduced by about 15%
after ROHC is enabled.
## 4.2.2 Impacts
The impacts between this function and other functions are described in 4.3.2.3
## Function Impacts.
ROHC reduces the amount of data transmitted over the air interface as well as the
traffic volume.
VoLTE UEs found incompatible with ROHC in interoperability tests (IOTs) always
transmit uncompressed IR packets even after ROHC is enabled. In this case, the
expected coverage or capacity gains offered by ROHC are not achieved, and the
number of RBs used for UEs running voice services slightly increases.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.23

However, the amount of feedback depends on the ROHC operating mode. More
feedback uses more radio resources, limiting system capacity expansion.
## 4.3 Requirements
## 4.3.1 Licenses
The following are TDD license requirements.
Feature IDFeature NameModelSales Unit
TDLOFD-001017RObust Header
## Compression
## (ROHC)
LT1ST0ROHC00per RRC Connected
## User

## NO TE
The insufficiency of certain feature licenses affects cell activation. For details, see the Is Cell
Activation Affected by License Insufficiency column in
## License Control Item Lists.
## 4.3.2 Functions
Before activating this function, ensure that its prerequisite functions have been
activated and mutually exclusive functions have been deactivated, if there are any.
For detailed operations, see the relevant feature documents.
Additionally, understand any potential function impacts before activating this
function. To deactivate any impacted functions, follow the operations described in
the relevant feature documents.
## 4.3.2.1 Prerequisite Functions
## None
## 4.3.2.2 Mutually Exclusive Functions
## None
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.24

## 4.3.2.3 Function Impacts
RATFunction
## Name
## Function
## Switch
## Referenc
e
## Description
TDDVoIP
## Semi-
## Persistent
## Schedulin
g
## Uplink:
SpsSchS
witch
option of
the
CellAlgoS
witch.
UlS
chSwitch
paramete
r
## Downlink:
SpsSchS
witch
option of
the
CellAlgoS
witch.
DlS
chSwitch
paramete
r
VoLTEWhen ROHC is enabled,
compressed packet sizes fluctuate,
even during talk spurts, due to
changes in the quality of the radio
channels, the ROHC operating
mode used, and variations in the
dynamic fields of the packet
headers at the application layer.
Therefore, ROHC has an impact on
semi-persistent scheduling. If the
packet size is greater than the
maximum size allowable for semi-
persistent scheduling, the eNodeB
uses dynamic scheduling for the
data beyond the size limit.
TDDVoice
characteri
stic
awarenes
s
schedulin
g
AmrVoice
FrameSm
artCovery
## Sw
option of
the
CellUlsch
## Algo.
UlE
nhenced
VoipSchS
w
paramete
r
VoLTEThe smart AMR voice frame
recovery function provides higher
gains when it is working with
## ROHC.
TDDNormal
preallocat
ion
PreAlloca
tionSwitc
h option
of the
CellAlgoS
witch.
UlS
chSwitch
paramete
r
## Uplink
## Schedulin
g
When the uplink normal or smart
preallocation function is enabled,
ROHC will yield few gains in
resource saving in the uplink if the
sizes of packets scheduled by the
eNodeB in preallocation are
greater than those of voice
packets.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.25

RATFunction
## Name
## Function
## Switch
## Referenc
e
## Description
TDDSmart
preallocat
ion
SmartPre
## Allocatio
nSwitch
option of
the
CellAlgoS
witch.
UlS
chSwitch
paramete
r
## Uplink
## Schedulin
g
TDDUplink
data
compressi
on
BasicUdc
## Switch
option of
the
CellAlgoS
witch.
## Ud
cAlgoSwi
tch
paramete
r
## Uplink
## Data
## Compress
ion
Uplink data compression and
ROHC-TCP can be enabled
simultaneously. However, for a
given UE:
● Both uplink data compression
and ROHC-TCP can take effect
simultaneously on bearers with
different QCIs.
● Uplink data compression and
ROHC-TCP cannot take effect
simultaneously on bearers with
the same QCI. The function
whose activation conditions are
met first takes effect first. The
other function can take effect
only after the function that has
taken effect terminates.
## TDDNSA
networkin
g based
on EPC
## NSA_DC_
## CAPABILI
## TY_SWIT
## CH
option of
the
NsaDcMg
mtConfig
## .
NsaDcAl
goSwitch
paramete
r
## EPC-
based
## NSA
## Basics
If the MCG bearer, MCG split
bearer, or SCG split bearer is set
up for an NSA UE, the PDCP of the
bearer will be set to NR PDCP (in
compliance with 3GPP TS 38.323).
However, if voice services or
TCP/IP-based data services with
ROHC are performed, only the
MCG_Bearer_EUTRA_PDCP bearer
can be set up and the PDCP of the
bearer must be set to E-UTRA
PDCP (in compliance with 3GPP TS
36.323). Therefore, ROHC and NSA
networking based on EPC cannot
take effect at the same time.

eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.26

## 4.3.3 Hardware
For details about the compatibility between the hardware described in this section,
see the technical specifications and hardware description of the corresponding
hardware in 3900 & 5900 Series Base Station Product Documentation.
## Base Station Models
No requirements
## Boards
●  For VoIP: no requirements
●  For ROHC-TCP: The LBBPc is not supported.
RF Modules
No requirements
## 4.3.4 Others
●  Before VoIP services are deployed, mainstream commercial VoLTE UEs need to
pass IOTs.
●  Before TCP/IP services are deployed, mainstream commercial ROHC-TCP UEs
need to pass IOTs.
4.4 Operation and Maintenance
## 4.4.1 Data Configuration
## 4.4.1.1 Data Preparation
Table 4-3 describes the parameters used for function activation.
Table 4-3 Parameters used for activation
## Parameter
## Name
Parameter IDOptionSetting Notes
ROHC switchCellAlgoSwit
ch.RohcSwitc
h
NoneSet this parameter to ON.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.27

## Parameter
## Name
Parameter IDOptionSetting Notes
## ROHC
Highest mode
PdcpRohcPar
a.HighestMo
de
NoneThis parameter specifies the
highest operating mode of
ROHC only in the uplink. The
highest operating mode of
ROHC in the downlink is
controlled by UEs.
Value O_MODE is
recommended.
The reasons are as follows:
● When U-Mode is used, the
compression will be
inefficient if the radio link
quality is poor.
● R-Mode introduces more
feedback data than O-
Mode although these two
modes have similar
compression efficiency. In
addition, frame loss may
occur on some VoLTE UEs
working in R-Mode.
## Compression
profiles
PdcpRohcPar
a.Profiles
## Profile0x0001
## Profile0x0002
## Profile0x0006
● For VoIP services, you are
advised to select the
Profile0x0001 and
Profile0x0002 options of
this parameter because
commercial VoLTE UEs
currently do not support
the Profile0x0003 or
Profile0x0004 option.
● For TCP/IP services, select
the Profile0x0006 option if
the turbo start video
function is enabled. For
details, see
## Video
## Experience Optimization.
## ROHC TCP
SINR Trigger
## Threshold
PdcpRohcPar
a.RohcTcpSin
rTriggerThld
NoneRetain the default value.
## ROHC
## Optimization
## Switch
PdcpRohcPar
a.RohcOptim
izationSwitch
## ROHC_FEEDB
## ACK_ENHANC
## EMENT_SW
Select this option.

eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.28

## NO TE
If the PdcpRohcPara.Profiles parameter is adjusted during eNodeB operation, the
adjustment affects only new services instead of ongoing services.
4.4.1.2 Using MML Commands
Before using MML commands, refer to 4.3 Requirements and complete the
parameter configurations for related functions based on the impact, dependency,
and mutually exclusive relationships between the functions, as well as the actual
network scenario. In addition, ensure that the license, hardware, networking, and
cell requirements are met.
Before using MML commands, confirm the related parameter modification
precautions by referring to the fields including "Service Interrupted After
Modification" and "Caution" for the corresponding parameters in the parameter
reference.
## Activation Command Examples
●  Macro eNodeB
MOD CELLALGOSWITCH: LocalCellId=0, RohcSwitch=ON;
MOD PDCPROHCPARA: HighestMode=O_MODE,
Profiles=Profile0x0001-1&Profile0x0002-1&Profile0x0003-0&Profile0x0004-0,
RohcTcpSinrTriggerThld=0, RohcOptimizationSwitch=ROHC_FEEDBACK_ENHANCEMENT_SW-1;
## Deactivation Command Examples
●  Macro eNodeB
MOD CELLALGOSWITCH: LocalCellId=0, RohcSwitch=OFF;
4.4.1.3 Using the MAE-Deployment
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
## NO TE
Due to differences between OSS versions, the GUIs in the interactive video may differ
from the actual OSS GUIs and are thus for reference only.
## 4.4.2 Activation Verification
Step 1On the MAE-Access, create and start a Uu interface tracing task.
Step 2Use an ROHC-capable UE to perform a VoIP service. Check the RRC_UE_CAP_INFO
message to determine whether the UE supports ROHC and which profiles the UE
supports.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.29

As shown in Figure 4-12, if the value of any profile is TRUE, the UE supports
ROHC and such a profile.
Figure 4-12 RRC_UE_CAP_INFO message
Step 3Check the RRC_CONN_RECFG message delivered when the bearer with QCI 1 is set
up to determine whether ROHC has been activated.
●  If the information elements (IEs) pdcp-Config > headerCompression > rohc
are displayed, as shown in Figure 4-13, ROHC has been activated.
●  If the IEs pdcp-Config > headerCompression > notUsed: NULL are displayed,
as shown in Figure 4-14, ROHC has not been activated.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.30

Figure 4-13 RRC_CONN_RECFG message (after activation)
Figure 4-14 RRC_CONN_RECFG message (before activation)
Step 4Check the performance counters on the MAE-Access after the ROHC feature has
been activated.
## NO TE
ROHC can only be used on the user plane. Ensure that the values of the preceding
performance counters are collected when the eNodeB is transmitting user-plane data.
●  In the downlink: A smaller value of L.PDCP.DL.ROHC.Voice.HdrComp.Bytes/
L.PDCP.DL.ROHC.Voice.Hdr.Bytes or L.PDCP.DL.RoHC.PktCompRatio
indicates higher compression efficiency.
●  In the uplink:
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.31

–   A smaller value of L.PDCP.UL.RoHC.FailDecomp.VoLTE/
L.PDCP.UL.RoHC.TotalDecomp.VoLTE indicates a higher decompression
success rate. If the value is 0, the decompression success rate is 100%.
–   A smaller value of L.PDCP.UL.ROHC.Voice.HdrComp.Bytes/
L.PDCP.UL.ROHC.Voice.Hdr.Bytes or L.PDCP.UL.RoHC.PktCompRatio
indicates higher compression efficiency.
## NO TE
After ROHC is enabled, the values of L.PDCP.DL.ROHC.Voice.HdrComp.Bytes/
L.PDCP.DL.ROHC.Voice.Hdr.Bytes, L.PDCP.DL.RoHC.PktCompRatio,
L.PDCP.UL.ROHC.Voice.HdrComp.Bytes/L.PDCP.UL.ROHC.Voice.Hdr.Bytes, and
L.PDCP.UL.RoHC.PktCompRatio have the following characteristics:
●   If ROHC is working under extreme conditions such as ping-pong handovers caused by
poor radio conditions and the compressor sends only IR packets (data packets cannot
be compressed) which have more bytes than original packets, the counter values may
be greater than or equal to 100%. This rarely occurs.
●   If ROHC is working under normal radio conditions, the counter values are less than
## 100%.
----End
## 4.4.3 Network Monitoring
After ROHC is enabled, monitor the counters listed in the following table.
Table 4-4 Performance counters to be monitored
Counter ID
## Counter
## Name
DescriptionPrinciple
1526728523L.PDCP.UL.Ro
HC.PktComp
## Ratio
Compression rate of all uplink
PDCP SDUs (including headers
and payloads) after the ROHC
## Smaller
values
indicate
higher
compression
efficiency.
1526727350L.PDCP.DL.Ro
HC.PktComp
## Ratio
Compression rate of all
downlink PDCP SDUs
(including headers and
payloads) after the ROHC
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.32

Counter IDCounter
## Name
DescriptionPrinciple
1526745690L.PDCP.UL.Ro
HC.FailDeco
mp.VoLTE
Number of uplink VoLTE
packets that fail to be
decompressed by ROHC in a
cell
d
## ROHC
decompressio
n failure rate
of uplink
VoLTE
packets
a
## . A
smaller
counter value
indicates a
higher
decompressio
n success rate,
and a larger
counter value
indicates a
higher
decompressio
n failure rate.
1526746015L.PDCP.UL.Ro
HC.TotalDeco
mp.VoLTE
Number of uplink VoLTE
packets that need to be
decompressed in ROHC
d
1526728524L.Traffic.User.
RoHC.Max
Maximum number of UEs on
which ROHC takes effect in a
cell
The number
of UEs on
which ROHC
takes effect
has a positive
correlation
with the
values of
these
counters.
1526728525L.Traffic.User.
RoHC.Avg
Average number of UEs on
which ROHC takes effect in a
cell
## 1526746663L.PDCP.UL.RO
HC.Voice.Hdr
Comp.Bytes
Number of bytes of uplink
voice service PDCP SDU
headers before ROHC-based
header decompression in a cell
ROHC ratio of
uplink voice
services
b
## . A
smaller
counter value
indicates
higher
compression
efficiency.
## 1526746658L.PDCP.UL.RO
HC.Voice.Hdr.
## Bytes
Number of bytes of uplink
voice service PDCP SDU
headers after ROHC-based
header decompression in a cell
## 1526746657L.PDCP.DL.RO
HC.Voice.Hdr
Comp.Bytes
Number of bytes of downlink
voice service PDCP SDU
headers after ROHC-based
header compression in a cell
ROHC ratio of
downlink
voice
services
c
## . A
smaller
counter value
indicates
higher
compression
efficiency.
## 1526746662L.PDCP.DL.RO
HC.Voice.Hdr.
## Bytes
Number of bytes of downlink
voice service PDCP SDU
headers before ROHC-based
header compression in a cell
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.33

Counter IDCounter
## Name
DescriptionPrinciple
a: ROHC decompression failure rate of uplink VoLTE packets =
L.PDCP.UL.RoHC.FailDecomp.VoLTE/L.PDCP.UL.RoHC.TotalDecomp.VoLTE
b: ROHC header compression ratio of uplink voice services =
L.PDCP.UL.ROHC.Voice.HdrComp.Bytes/L.PDCP.UL.ROHC.Voice.Hdr.Bytes
c: ROHC header compression ratio of downlink voice services =
L.PDCP.DL.ROHC.Voice.HdrComp.Bytes/L.PDCP.DL.ROHC.Voice.Hdr.Bytes
d: For PTT voice services, the number of uplink VoLTE packets that fail to be
decompressed by ROHC and the number of uplink VoLTE packets that need to
be decompressed by ROHC are measured in
L.PDCP.UL.RoHC.FailDecomp.VoLTE and L.PDCP.UL.RoHC.TotalDecomp.VoLTE,
respectively.
eRAN
ROHC Feature Parameter Description4 ROHC
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.34

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
the software version used on the live network from the "Man-Machine Interface Reference"
node in the 3900 & 5900 Series Base Station Product Documentation delivered with that
version.
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
ROHC Feature Parameter Description5 Parameters
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.35

## 6 Counters
The following hyperlinked EXCEL files of performance counter reference match the
software version with which this document is released.
●  Node Performance Counter Summary: contains device and transport counters.
●  eNodeBFunction Performance Counter Summary: contains all counters related
to radio access functions, including air interface management, access control,
mobility control, and radio resource management.
●  eNodeBFunction Used Reserved Counter List: contains the reserved counters
that are in use and those that have been disused.
## NO TE
You can find the EXCEL files of performance counter reference and used reserved counter
list for the software version used on the live network from the "Man-Machine Interface
Reference" node in the
3900 & 5900 Series Base Station Product Documentation delivered
with that version.
FAQ: How do I find the counters related to a certain feature from
performance counter reference?
Step 1Open the EXCEL file of performance counter reference.
Step 2On the Counter Summary(En) sheet, filter the Feature ID column. Click Text
Filters and choose Contains. Enter the feature ID, for example, LOFD-001016 or
## TDLOFD-001016.
Step 3Click OK. All counters related to the feature are displayed.
----End
eRAN
ROHC Feature Parameter Description6 Counters
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.36

## 7 Glossary
For the acronyms, abbreviations, terms, and definitions, see Glossary.
eRAN
ROHC Feature Parameter Description7 Glossary
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.37

## 8 Reference Documents
-  3GPP TS 36.323, "Packet Data Convergence Protocol (PDCP) specification"
-  3GPP TS 38.323, "Packet Data Convergence Protocol (PDCP) specification"
-  IETF RFC 3095, "RObust Header Compression (ROHC)"
-  IETF RFC 4164, "State Machine with Context Replication"
## 5.
VoLTE
6.Uplink Scheduling
7.EPC-based NSA Basics
8.Uplink Data Compression
9.Video Experience Optimization
eRAN
ROHC Feature Parameter Description8 Reference Documents
Issue 01 (2025-03-10)Copyright © Huawei Technologies Co., Ltd.38