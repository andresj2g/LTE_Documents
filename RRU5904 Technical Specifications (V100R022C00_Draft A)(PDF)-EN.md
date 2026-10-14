

## RRU5904
## V100R022C00
## Technical Specifications
IssueDraft A
## Date2025-06-30
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
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.i



## Security Declaration

## Vulnerability
Huawei's regulations on product vulnerability management are subject to the Vul. Response Process. For
details about this process, visit the following web page:
https://www.huawei.com/en/psirt/vul-response-process
For vulnerability information, enterprise customers can visit the following web page:
https://securitybulletin.huawei.com/enterprise/en/security-advisory




## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.ii

## Contents
1 RRU5904 Technical Specifications.......................................................................................1
2 Changes in RRU5904 Technical Specifications ................................................................3
3 RRU5904 (1800 MHz) Technical Specifications................................................................4
3.1 RRU5904 (1800 MHz) RF Specifications......................................................................................................................... 4
3.2 RRU5904 (1800 MHz) Engineering Specifications.......................................................................................................9
3.3 RRU5904 (1800 MHz) CPRI Port Specifications......................................................................................................... 11
4 RRU5904 (2100 MHz) Technical Specifications............................................................. 13
4.1 RRU5904 (2100 MHz) RF Specifications.......................................................................................................................13
4.2 RRU5904 (2100 MHz) Engineering Specifications.................................................................................................... 18
4.3 RRU5904 (2100 MHz) CPRI Port Specifications......................................................................................................... 20
5 RF Output Power Configuration Rules.............................................................................22
## RRU5904
Technical SpecificationsContents
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.iii

1 RRU5904 Technical Specifications
This document describes the radio frequency (RF) specifications, engineering
specifications, and common public radio interface (CPRI) port specifications of the
## RRU5904.
## NO TICE
The specifications that are not mentioned in this document or described as
unsupported may be configurable. The device supports only the specifications that
are mentioned in this document and meet specific constraints. If the specifications
that are not mentioned in this document or described as unsupported are
configured, services may be affected or the network may be out of service.
## Product Versions
The following table lists the base station product versions related to the RRU.
## Product Name
Solution VersionProduct Version
## RRU5904SRAN22.0V100R022C00
For details about the software
versions of RF modules, see
Software and Hardware
## Compatibility Description.

## Intended Audience
This document is intended for:
●  Network planners
●  Onsite engineers
●  System engineers
## RRU5904
Technical Specifications1 RRU5904 Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.1

## Organization
## RRU5904
Technical Specifications1 RRU5904 Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.2

2 Changes in RRU5904 Technical
## Specifications
This chapter describes the changes in RRU5904 Technical Specifications.
## Draft A (2025-06-30)
This is a draft.
Compared with Issue 01 (2025-03-10) of V100R021C10, this issue does not include
any new topics.
Compared with Issue 01 (2025-03-10) of V100R021C10, this issue includes the
following changes.
## Topic
## Change Description
5 RF Output Power
## Configuration Rules
Revised the description of the impact when the
carrier output power of a cell is less than the
minimum configurable output power in the general
output power configuration rules.

Compared with Issue 01 (2025-03-10) of V100R021C10, this issue does not
exclude any topics.
## RRU5904
Technical Specifications2 Changes in RRU5904 Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.3

3 RRU5904 (1800 MHz) Technical
## Specifications
The technical specifications of an RRU5904 (1800 MHz) include RF specifications,
engineering specifications, and CPRI port specifications.
3.1 RRU5904 (1800 MHz) RF Specifications
The RF specifications include the supported radio access technologies (RATs),
frequency bands, TX/RX modes, capacity, output power, carrier configurations, and
receiver sensitivity.
3.2 RRU5904 (1800 MHz) Engineering Specifications
The engineering specifications include the input power, dimensions, weight, power
consumption, and environmental specifications.
3.3 RRU5904 (1800 MHz) CPRI Port Specifications
The CPRI port specifications include the number of CPRI ports, port protocol, port
rate, and maximum level of cascading and maximum distance with a BBU.
3.1 RRU5904 (1800 MHz) RF Specifications
The RF specifications include the supported radio access technologies (RATs),
frequency bands, TX/RX modes, capacity, output power, carrier configurations, and
receiver sensitivity.
●  In the following, G is short for GSM, L is short for LTE FDD, M is short for LTE
NB-IoT, and N (FDD) is short for NR FDD.
●  In the following, SUL is short for supplementary uplink and N (SUL) is short
for NR SUL.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.4

Supported Frequency Bands and RATs
Table 3-1 Frequency bands and RATs supported by an RRU5904 (1800 MHz)
## Frequency
## Band
(MHz)
## Protocol
## -defined
## Band
## RX
## Frequency
## Band
(MHz)
## TX
## Frequency
## Band
(MHz)
## RATIBW
(MHz)
1800Band
## 3/n3
1710 to
## 1785
1805 to
## 1880
## GSM, LTE FDD,
GL, LTE NB-IoT,
## GM, LM, GLM,
## LN (SUL), GLN
## (SUL), NR FDD,
## GN (FDD), LN
## (FDD), GLN
## (FDD), MN
## (FDD), LMN
## (FDD)
## 45

TX/RX Modes and Capacity
Table 3-2 TX/RX modes and capacity of an RRU5904 (1800 MHz)
## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## TX/RX
## Mode
a
## Capacity
b
## Supported
## Bandwidth
(MHz)
c
1800Band
## 3/n3
4T4RGSM: 8 carriers
LTE FDD: 3 carriers
LTE NB-IoT: 8 carriers
when the NB-IoT multi-
carrier function is
enabled and 1 carrier
when the NB-IoT multi-
carrier function is
disabled
NR SUL: 1 carrier
NR FDD: 3 carriers
## LTE FDD:
## 5/10/15/20
## NR SUL: 15/20
## NR FDD:
## 5/10/15/20/25/
## 30
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.5

## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## TX/RX
## Mode
a
## Capacity
b
## Supported
## Bandwidth
(MHz)
c
a: mTnR in the TX/RX Mode column indicates that the RF module uses m
transmit channels and n receive channels.
b: The number of carriers in the Capacity column refers to the maximum
number of carriers that can be configured for the module with the RAT
configured, not the number of carriers that can be configured for a single
channel. For details about the module-level and channel-level carrier
configurations supported in single-mode and multimode scenarios, see the
Output Power Configuration column in the following table. When the module
is used with a feature, see the feature specifications in the corresponding
feature parameter description to learn the module-level or channel-level carrier
configurations that are supported after the feature is enabled.
c: The bandwidth information in Supported Bandwidth is the standard
bandwidth that can be configured for a carrier when only one carrier is
configured for the module working in a single mode. In any carrier combination
scenario, the difference between the absolute value of the highest frequency
and the absolute value of the lowest frequency of the involved carriers
operating on the same band cannot exceed the instantaneous bandwidth (IBW).
For details about the bandwidth that can be configured for each carrier in each
carrier combination scenario, see Output Power Configuration in the following
table. For details about non-standard bandwidths that can be configured for LTE
FDD carriers, see
Compact Bandwidth (FDD) > Compact Bandwidth >
Requirements > Hardware > RF Modules in eRAN FDD Feature
## Documentation.

## NO TE
●  In the Supported Bandwidth column, the 5/10/15/20 MHz bandwidth per NR FDD
carrier is supported from 5G RAN3.1 onwards, the 30 MHz bandwidth per NR FDD
carrier is supported from 5G RAN5.1 onwards, and the 25 MHz bandwidth per NR FDD
carrier is supported from 5G RAN6.0 onwards.
## NO TE
The NB-IoT multi-carrier function is an NB-IoT multi-carrier transmission technology
introduced based on 3GPP Release 13. A cell can have multiple carriers and assigns UEs to
multiple carriers to increase cell capacity. For details about this function and related
parameter settings, see
NB-IoT Enhancements (FDD) > Capacity Enhancement > Multi-
Carrier Transmission in eRAN FDD Feature Documentation.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.6

Output Power and Carrier Configurations
Table 3-3 Output power and carrier configurations of an RRU5904 (1800 MHz)
## Frequency
Band (MHz)
## Maximum Output
## Power
a
## Output Power Configuration
18004x60 WRRU Typical carrier and power
configurations (excluding NB-IoT)
Typical Carrier and Power
Configurations for RRUs (NB-IoT
only)
a: mxP W in Maximum Output Power indicates that the number of TX
channels of the RF module is m and the maximum output power of each
channel is P W. The output power that can be configured for each carrier
combination can be less than or equal to the maximum output power. For
details about the power configuration for each carrier combination, see Typical
Carrier and Power Configurations
## .

## NO TE
●  The Typical Carrier and Power Configurations document includes the configurable
carrier combinations and the output power of each carrier in each combination. Before
referring to this document, you must be familiar with the output power configuration
rules. For details, see 5 RF Output Power Configuration Rules.
●  The carrier bandwidths supported by carriers with different power may be different. For
details about the output power of carriers and supported carrier bandwidth, see the
Typical Carrier and Power Configurations document. Each Output Power per Carrier
value in the
Typical Carrier and Power Configurations document indicates the maximum
output power of each carrier under the corresponding configuration while ensuring the
network performance. The actually configured carrier power of RF modules can be less
than or equal to the value of Output Power per Carrier. The power configurations that
are not mentioned in the
Typical Carrier and Power Configurations document may be
configurable on the software. Performance can only be ensured under the listed power
configurations in the
Typical Carrier and Power Configurations document.
NR SUL Carrier Configurations
This section describes the numbers of LTE FDD carriers and NR FDD carriers that
can be configured on the LTE uplink spectrum after the LTE and NR uplink
spectrum sharing feature is enabled.
Table 3-4 SUL carrier configurations of an RRU5904 (LN, 1800 MHz, 4R)
Maximum Number of
LTE FDD Carriers
Maximum Number of
NR SUL Carriers
Bandwidth per NR SUL
Carrier (MHz)
## 3 (MIMO)115/20

## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.7

Table 3-5 SUL carrier configurations of an RRU5904 (GLN, 1800 MHz, 4R)
## Maximum
Number of GSM
## Carriers
## Maximum
Number of LTE
FDD Carriers
## Maximum
Number of NR
SUL Carriers
Bandwidth per
NR SUL Carrier
(MHz)
## 82 (MIMO)115/20

## NO TE
The uplink bandwidth of an LTE carrier enabled with uplink spectrum sharing must be the
same as the uplink bandwidth of an NR carrier. For detailed bandwidth, see the value in the
Bandwidth per NR SUL Carrier (MHz) column in the preceding table. The uplink
bandwidth of an LTE carrier that is not enabled with uplink spectrum sharing is not limited
by the NR SUL bandwidth.
## Receiver Sensitivity
Table 3-6 Receiver sensitivity of an RRU5904 (1800 MHz)
## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## Receiver
## Sensitivity
with One
## Antenna
(dBm)
## Receiver
## Sensitivity
with Two
## Antennas
(dBm)
## Receiver
Sensitivity with
## Four Antennas
(dBm)
1800Band
## 3/n3
## GSM: -114.0
## LTE FDD: -106.6
LTE NB-IoT:
## -127.3
## NR FDD: -106.3
## GSM: -116.8
## LTE FDD: -109.4
LTE NB-IoT:
## -130.1
## NR FDD: -109.1
## GSM: -119.5
(theoretical value)
## LTE FDD: -112.1
LTE NB-IoT: -132.8
## NR FDD: -111.8

## NO TE
●  The GSM receiver sensitivity, as recommended in 3GPP TS 51.021, is measured at the
antenna connector assuming that the channel rate is 13 kbit/s and the bit error rate
(BER) is lower than or equal to 2%.
●  The LTE FDD receiver sensitivity, as recommended in 3GPP TS 36.141, is measured under
a 5 MHz bandwidth based on the FRC A1-3 in Annex A.1 (QPSK, R = 1/3, 25 RBs)
standard.
●  The LTE NB-IoT receiver sensitivity, as recommended in 3GPP TS 36.141, is measured
under a 200 kHz bandwidth and a 15 kHz subcarrier spacing based on the FRC A14-1 in
Annex A.14 (π/2 BPSK, R = 1/3, 1 RB) standard.
●  The NR FDD receiver sensitivity, as recommended in 3GPP TS 38.141, is measured under
a 5 MHz bandwidth based on the Annex A.1 (QPSK, R = 1/3) standard.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.8

## NO TICE
With respect to configuration in actual networking, especially in leaky cable
networking scenarios such as subway and high-speed railway tunnel scenarios,
prevent high-power signals from directly entering the RX channel of an RF
module. Otherwise, the RF module may be damaged.
RF Compliance Standards
Table 3-7 RF compliance standards for an RRU5904 (1800 MHz)
ItemStandard
GSM standard3GPP TS 45.005
LTE standard3GPP TS 36.104
NR standard3GPP TS 38.104
Multimode standard3GPP TS 37.104

3.2 RRU5904 (1800 MHz) Engineering Specifications
The engineering specifications include the input power, dimensions, weight, power
consumption, and environmental specifications.
## Input Power
Table 3-8 Input power of an RRU5904 (1800 MHz)
## Power Input Type
## Operating Voltage
-48 V DC–36 V DC to –57 V DC

## NO TE
DC RRUs can use external power modules to support AC scenarios. For details about the
types of external power modules supported by each type of RRU, see section "RRU Auxiliary
Devices" in the corresponding RRU hardware description. For details about the external
power modules, see user guides of the corresponding models.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.9

Dimensions and Weight
Table 3-9 Dimensions and weight of an RRU5904 (1800 MHz)
ItemSpecifications
Dimensions (H x W x D)● Without the protective structure: 400 mm x 300
mm x 150 mm (15.75 in. x 11.81 in. x 5.91 in.)
## (18 L)
● With the protective structure: 400 mm x 300
mm x 170 mm (15.75 in. x 11.81 in. x 6.69 in.)
Weight22 kg (48.51 lb, excluding mounting kits)

## Module Power Consumption
Table 3-10 Power consumption of an RRU5904 (1800 MHz)
Frequency Band (MHz)
Typical Power Consumption (W)
a
## 1800492
a: The typical power consumption of an RF module is measured when the
ambient temperature is 25°C (77°F) and the traffic load reaches 50%. The
actual power consumption has a 10% deviation from this value.

## Environmental Specifications
Table 3-11 Environmental specifications of an RRU5904 (1800 MHz)
## Item
## Specifications
Operating temperature● Without sunlight exposure: –40°C to +55°C (–
40°F to +131°F)
● With sunlight exposure of 1120 W/m
## 2
: –40°C to
+50°C (–40°F to +122°F)
Relative humidity5% RH to 100% RH
Absolute humidity
1 g/m
## 3
to 30 g/m
## 3
Altitude≤ 4000 m (13123.36 ft)

## NO TE
The output power of an RRU temporarily decreases when it operates at temperature ranges
10ºC (18ºF) less than or equal to its maximum operating temperature. This is dependent on
installation scenario, traffic load, and carrier configuration.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.10

Table 3-12 Surge protection specifications of ports on an RRU5904 (1800 MHz)
PortSurge Protection ModeSpecifications
DC power portSurge current20 kA

## NO TE
●  Unless otherwise specified, the surge protection specifications are based on the surge
waveform of 8/20 μs.
●  In surge protection specifications of ports, unless otherwise specified as maximum discharge
current, all the surge current items refer to nominal discharge current.
Table 3-13 Environment compliance standards for an RRU5904 (1800 MHz)
ItemSpecifications
Operating environmentETSI EN 300 019-1-4 Class 4.1
Storage environment
a
ETSI EN 300 019-1-1 Class 1.2
Shockproof protectionNEBS GR63 zone4
Ingress protection ratingIP65
Surge protection● IEC 62305-1
## ● ITU-T K.35
## ● ITU-T K.56
## ● ITU-T K.112
## ● ETSI EN 300 253
a: The validity period is one year. The product can function properly within the
validity period if the storage environment meets the preceding standards.

3.3 RRU5904 (1800 MHz) CPRI Port Specifications
The CPRI port specifications include the number of CPRI ports, port protocol, port
rate, and maximum level of cascading and maximum distance with a BBU.
Table 3-14 CPRI port protocol and rate of an RRU5904 (1800 MHz)
Number of CPRI Ports
Protocol TypePort Rate (Gbit/s)
## 2CPRI1.25/2.5/4.9/9.8

The maximum level of cascading between an RRU and a BBU depends on the
cascading capability of the RRU working in different RATs and the bandwidth
resources of the CPRI ports on the BBU side. The following table provides the
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.11

maximum level of cascading and maximum distance between an RRU and a BBU
when the RRU works in a single mode. When the RRU works in multimode
concurrency scenarios, the maximum level of cascading and maximum distance
between the multimode RRU and a BBU are determined by the capabilities for the
mode with the lowest capabilities.
Table 3-15 Maximum level of cascading and maximum distance between an
RRU5904 (1800 MHz) and a BBU
ModeMaximum Level of
Cascading with a
## BBU
Maximum Distance from a BBU (km)
## GSM640
LTE FDD4● When the LBBPc or LBBPd1 is
configured: 20
● When the LBBPd2 or UBBP is
configured: 40
● When the LBBPd3 is configured: 40
(number of cells ≤ 3); 20 (number
of cells ≥ 4)
LTE NB-IoT420
## NR SUL420
## NR FDD420

## NO TE
●  For details about the CPRI topologies supported by each RRU model, see RF Unit and
Topology Management > Topologies > Principles > RF Modules > Basic RRU
Information in the feature documentation of the corresponding RAT (for example,
eRAN Feature Documentation)..
●  For details about the ALD capabilities supported by each RRU model (for example, the
capabilities of RF ports supporting RET antennas and TMAs), see
ALD Management >
General Principles in the feature documentation of the corresponding RAT (for
example, eRAN Feature Documentation).
●  For details about the CPRI compression ratios supported by LTE-capable RRUs, see
## CPRI
## Compression
> CPRI Compression > Requirements > Hardware in eRAN Feature
Documentation. For details about the CPRI compression ratios supported by NR-
capable RRUs, see
CPRI Compression > CPRI Compression (Macro) > Requirements >
Hardware in 5G RAN Feature Documentation.
## RRU5904
Technical Specifications3 RRU5904 (1800 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.12

4 RRU5904 (2100 MHz) Technical
## Specifications
The technical specifications of an RRU5904 (2100 MHz) include RF specifications,
engineering specifications, and CPRI port specifications.
4.1 RRU5904 (2100 MHz) RF Specifications
The RF specifications include the supported radio access technologies (RATs),
frequency bands, TX/RX modes, capacity, output power, carrier configurations, and
receiver sensitivity.
4.2 RRU5904 (2100 MHz) Engineering Specifications
The engineering specifications include the input power, dimensions, weight, power
consumption, and environmental specifications.
4.3 RRU5904 (2100 MHz) CPRI Port Specifications
The CPRI port specifications include the number of CPRI ports, port protocol, port
rate, and maximum level of cascading and maximum distance with a BBU.
4.1 RRU5904 (2100 MHz) RF Specifications
The RF specifications include the supported radio access technologies (RATs),
frequency bands, TX/RX modes, capacity, output power, carrier configurations, and
receiver sensitivity.
●  In the following, U is short for UMTS, L is short for LTE FDD, M is short for
LTE NB-IoT, and N (FDD) is short for NR FDD.
●  In the following, SUL is short for supplementary uplink and N (SUL) is short
for NR SUL.
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.13

Supported Frequency Bands and RATs
Table 4-1 Frequency bands and RATs supported by an RRU5904 (2100 MHz)
## Frequency
## Band
(MHz)
## Protocol
## -defined
## Band
## RX
## Frequency
## Band
(MHz)
## TX
## Frequency
## Band
(MHz)
## RATIBW
(MHz)
2100Band
## 1/n1
1920 to
## 1980
2110 to
## 2170
## UMTS, LTE
## FDD, UL, ULM,
## LN (SUL), ULN
## (SUL), NR FDD,
## UN (FDD), LN
## (FDD), ULN
## (FDD), LM
## 60

TX/RX Modes and Capacity
Table 4-2 TX/RX modes and capacity of an RRU5904 (2100 MHz)
## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## TX/RX
## Mode
a
## Capacity
b
## Supported
## Bandwidth
(MHz)
c
2100Band
## 1/n1
4T4RUMTS: 8 carriers
(without MIMO) and 4
carriers (with MIMO)
LTE FDD: 3 carriers
LTE NB-IoT: 1 carrier
NR SUL: 1 carrier
NR FDD: 3 carriers
## LTE FDD:
## 5/10/15/20
## NR SUL: 15/20
## NR FDD:
## 5/10/15/20/25/
## 30/40
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.14

## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## TX/RX
## Mode
a
## Capacity
b
## Supported
## Bandwidth
(MHz)
c
a: mTnR in the TX/RX Mode column indicates that the RF module uses m
transmit channels and n receive channels.
b: The number of carriers in the Capacity column refers to the maximum
number of carriers that can be configured for the module with the RAT
configured, not the number of carriers that can be configured for a single
channel. For details about the module-level and channel-level carrier
configurations supported in single-mode and multimode scenarios, see the
Output Power Configuration column in the following table. When the module
is used with a feature, see the feature specifications in the corresponding
feature parameter description to learn the module-level or channel-level carrier
configurations that are supported after the feature is enabled.
c: The bandwidth information in Supported Bandwidth is the standard
bandwidth that can be configured for a carrier when only one carrier is
configured for the module working in a single mode. In any carrier combination
scenario, the difference between the absolute value of the highest frequency
and the absolute value of the lowest frequency of the involved carriers
operating on the same band cannot exceed the instantaneous bandwidth (IBW).
For details about the bandwidth that can be configured for each carrier in each
carrier combination scenario, see Output Power Configuration in the following
table. For details about non-standard bandwidths that can be configured for LTE
FDD carriers, see
Compact Bandwidth (FDD) > Compact Bandwidth >
Requirements > Hardware > RF Modules in eRAN FDD Feature
## Documentation.

## NO TE
●  In the Supported Bandwidth column, the 5/10/15/20 MHz bandwidth per NR FDD
carrier is supported from 5G RAN3.1 onwards, the 30/40 MHz bandwidth per NR FDD
carrier is supported from 5G RAN5.1 onwards, and the 25 MHz bandwidth per NR FDD
carrier is supported from 5G RAN6.0 onwards.
Output Power and Carrier Configurations
Table 4-3 Output power and carrier configurations of an RRU5904 (2100 MHz)
## Frequency
Band (MHz)
## Maximum Output
## Power
a
## Output Power Configuration
21004x60 WRRU Typical carrier and power
configurations (excluding NB-IoT)
Typical Carrier and Power
Configurations for RRUs (NB-IoT
only)
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.15

## Frequency
Band (MHz)
## Maximum Output
## Power
a
## Output Power Configuration
a: mxP W in Maximum Output Power indicates that the number of TX
channels of the RF module is m and the maximum output power of each
channel is P W. The output power that can be configured for each carrier
combination can be less than or equal to the maximum output power. For
details about the power configuration for each carrier combination, see Typical
Carrier and Power Configurations
## .

## NO TE
●  The Typical Carrier and Power Configurations document includes the configurable
carrier combinations and the output power of each carrier in each combination. Before
referring to this document, you must be familiar with the output power configuration
rules. For details, see 5 RF Output Power Configuration Rules.
●  The carrier bandwidths supported by carriers with different power may be different. For
details about the output power of carriers and supported carrier bandwidth, see the
Typical Carrier and Power Configurations document. Each Output Power per Carrier
value in the
Typical Carrier and Power Configurations document indicates the maximum
output power of each carrier under the corresponding configuration while ensuring the
network performance. The actually configured carrier power of RF modules can be less
than or equal to the value of Output Power per Carrier. The power configurations that
are not mentioned in the
Typical Carrier and Power Configurations document may be
configurable on the software. Performance can only be ensured under the listed power
configurations in the Typical Carrier and Power Configurations document.
NR SUL Carrier Configurations
This section describes the numbers of LTE FDD carriers and NR FDD carriers that
can be configured on the LTE uplink spectrum after the LTE and NR uplink
spectrum sharing feature is enabled.
Table 4-4 SUL carrier configurations of an RRU5904 (LN, 2100 MHz, 4R)
Maximum Number of
LTE FDD Carriers
Maximum Number of
NR SUL Carriers
Bandwidth per NR SUL
Carrier (MHz)
## 3 (MIMO)115/20

Table 4-5 SUL carrier configurations of an RRU5904 (ULN, 2100 MHz, 4R)
## Maximum
Number of UMTS
## Carriers
## Maximum
Number of LTE
FDD Carriers
## Maximum
Number of NR
SUL Carriers
Bandwidth per
NR SUL Carrier
(MHz)
## 82 (MIMO)115/20
## 2 (MIMO)2 (MIMO)115/20
## 3 (MIMO)1 (MIMO)115/20

## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.16

## NO TE
The uplink bandwidth of an LTE carrier enabled with uplink spectrum sharing must be the
same as the uplink bandwidth of an NR carrier. For detailed bandwidth, see the value in the
Bandwidth per NR SUL Carrier (MHz) column in the preceding table. The uplink
bandwidth of an LTE carrier that is not enabled with uplink spectrum sharing is not limited
by the NR SUL bandwidth.
## Receiver Sensitivity
Table 4-6 Receiver sensitivity of an RRU5904 (2100 MHz)
## Frequency
## Band
(MHz)
## Protocol-
defined
## Band
## Receiver
## Sensitivity
with One
## Antenna
(dBm)
## Receiver
## Sensitivity
with Two
## Antennas
(dBm)
## Receiver
Sensitivity with
## Four Antennas
(dBm)
2100Band
## 1/n1
## UMTS: -126.1
## LTE FDD: -106.9
LTE NB-IoT:
## -127.3
## NR FDD: -106.6
## UMTS: -128.9
## LTE FDD: -109.7
LTE NB-IoT:
## -130.1
## NR FDD: -109.4
## UMTS: -131.6
## LTE FDD: -112.4
LTE NB-IoT: -132.8
## NR FDD: -112.1

## NO TE
●  The UMTS receiver sensitivity, as recommended in 3GPP TS 25.141, is measured at the
antenna connector assuming that the channel rate is 12.2 kbit/s and the bit error rate
(BER) is lower than or equal to 0.001.
●  The LTE FDD receiver sensitivity, as recommended in 3GPP TS 36.141, is measured under
a 5 MHz bandwidth based on the FRC A1-3 in Annex A.1 (QPSK, R = 1/3, 25 RBs)
standard.
●  The LTE NB-IoT receiver sensitivity, as recommended in 3GPP TS 36.141, is measured
under a 200 kHz bandwidth and a 15 kHz subcarrier spacing based on the FRC A14-1 in
Annex A.14 (π/2 BPSK, R = 1/3, 1 RB) standard.
●  The NR FDD receiver sensitivity, as recommended in 3GPP TS 38.141, is measured under
a 5 MHz bandwidth based on the Annex A.1 (QPSK, R = 1/3) standard.
## NO TICE
With respect to configuration in actual networking, especially in leaky cable
networking scenarios such as subway and high-speed railway tunnel scenarios,
prevent high-power signals from directly entering the RX channel of an RF
module. Otherwise, the RF module may be damaged.
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.17

RF Compliance Standards
Table 4-7 RF compliance standards for an RRU5904 (2100 MHz)
ItemStandard
UMTS standard3GPP TS 25.104
LTE standard3GPP TS 36.104
NR standard3GPP TS 38.104
Multimode standard3GPP TS 37.104

4.2 RRU5904 (2100 MHz) Engineering Specifications
The engineering specifications include the input power, dimensions, weight, power
consumption, and environmental specifications.
## Input Power
Table 4-8 Input power of an RRU5904 (2100 MHz)
## Power Input Type
## Operating Voltage
-48 V DC–36 V DC to –57 V DC

## NO TE
DC RRUs can use external power modules to support AC scenarios. For details about the
types of external power modules supported by each type of RRU, see section "RRU Auxiliary
Devices" in the corresponding RRU hardware description. For details about the external
power modules, see user guides of the corresponding models.
Dimensions and Weight
Table 4-9 Dimensions and weight of an RRU5904 (2100 MHz)
## Item
## Specifications
Dimensions (H x W x D)● Without the protective structure: 400 mm x 300
mm x 150 mm (15.75 in. x 11.81 in. x 5.91 in.)
## (18 L)
● With the protective structure: 400 mm x 300
mm x 170 mm (15.75 in. x 11.81 in. x 6.69 in.)
Weight22 kg (48.51 lb, excluding mounting kits)

## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.18

## Module Power Consumption
Table 4-10 Power consumption of an RRU5904 (2100 MHz)
Frequency Band (MHz)
Typical Power Consumption (W)
a
## 2100492
a: The typical power consumption of an RF module is measured when the
ambient temperature is 25°C (77°F) and the traffic load reaches 50%. The
actual power consumption has a 10% deviation from this value.

## Environmental Specifications
Table 4-11 Environmental specifications of an RRU5904 (2100 MHz)
ItemSpecifications
Operating temperature● Without sunlight exposure: –40°C to +55°C (–
40°F to +131°F)
● With sunlight exposure of 1120 W/m
## 2
: –40°C to
+50°C (–40°F to +122°F)
Relative humidity5% RH to 100% RH
Absolute humidity
1 g/m
## 3
to 30 g/m
## 3
Altitude≤ 4000 m (13123.36 ft)

## NO TE
The output power of an RRU temporarily decreases when it operates at temperature ranges
10ºC (18ºF) less than or equal to its maximum operating temperature. This is dependent on
installation scenario, traffic load, and carrier configuration.
Table 4-12 Surge protection specifications of ports on an RRU5904 (2100 MHz)
## Port
Surge Protection ModeSpecifications
DC power portSurge current20 kA

## NO TE
●  Unless otherwise specified, the surge protection specifications are based on the surge
waveform of 8/20 μs.
●  In surge protection specifications of ports, unless otherwise specified as maximum discharge
current, all the surge current items refer to nominal discharge current.
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.19

Table 4-13 Environment compliance standards for an RRU5904 (2100 MHz)
ItemSpecifications
Operating environmentETSI EN 300 019-1-4 Class 4.1
Storage environment
a
ETSI EN 300 019-1-1 Class 1.2
Shockproof protectionNEBS GR63 zone4
Ingress protection ratingIP65
Surge protection● IEC 62305-1
## ● ITU-T K.35
## ● ITU-T K.56
## ● ITU-T K.112
## ● ETSI EN 300 253
a: The validity period is one year. The product can function properly within the
validity period if the storage environment meets the preceding standards.

4.3 RRU5904 (2100 MHz) CPRI Port Specifications
The CPRI port specifications include the number of CPRI ports, port protocol, port
rate, and maximum level of cascading and maximum distance with a BBU.
Table 4-14 CPRI port protocol and rate of an RRU5904 (2100 MHz)
Number of CPRI Ports
Protocol TypePort Rate (Gbit/s)
## 2CPRI1.25/2.5/4.9/9.8

The maximum level of cascading between an RRU and a BBU depends on the
cascading capability of the RRU working in different RATs and the bandwidth
resources of the CPRI ports on the BBU side. The following table provides the
maximum level of cascading and maximum distance between an RRU and a BBU
when the RRU works in a single mode. When the RRU works in multimode
concurrency scenarios, the maximum level of cascading and maximum distance
between the multimode RRU and a BBU are determined by the capabilities for the
mode with the lowest capabilities.
Table 4-15 Maximum level of cascading and maximum distance between an
RRU5904 (2100 MHz) and a BBU
## Mode
Maximum Level of
Cascading with a
## BBU
Maximum Distance from a BBU (km)
## UMTS640
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.20

ModeMaximum Level of
Cascading with a
## BBU
Maximum Distance from a BBU (km)
LTE FDD4● When the LBBPc or LBBPd1 is
configured: 20
● When the LBBPd2 or UBBP is
configured: 40
● When the LBBPd3 is configured: 40
(number of cells ≤ 3); 20 (number
of cells ≥ 4)
LTE NB-IoT420
## NR SUL420
## NR FDD420

## NO TE
●  For details about the CPRI topologies supported by each RRU model, see RF Unit and
## Topology Management
> Topologies > Principles > RF Modules > Basic RRU
Information in the feature documentation of the corresponding RAT (for example,
eRAN Feature Documentation)..
●  For details about the ALD capabilities supported by each RRU model (for example, the
capabilities of RF ports supporting RET antennas and TMAs), see
ALD Management >
General Principles in the feature documentation of the corresponding RAT (for
example, eRAN Feature Documentation).
●  For details about the CPRI compression ratios supported by LTE-capable RRUs, see
## CPRI
## Compression
> CPRI Compression > Requirements > Hardware in eRAN Feature
Documentation. For details about the CPRI compression ratios supported by NR-
capable RRUs, see
CPRI Compression > CPRI Compression (Macro) > Requirements >
Hardware in 5G RAN Feature Documentation.
## RRU5904
Technical Specifications4 RRU5904 (2100 MHz) Technical Specifications
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.21

5 RF Output Power Configuration Rules
The rules for configuring RF output power include both general rules that apply to
all RATs and specific rules for each RAT. This section outlines the general rules for
RF modules across all models. For details about the power configuration for each
carrier combination for each RF module, see
Typical Carrier and Power
## Configurations.
## General Rules
●  The total output power of all carriers on a single channel cannot exceed the
maximum output power of a single channel.
●  It is recommended that a module be located at an altitude less than or equal
to 4000 m (13123.36 ft). The output power is 1 dB less than the standard
power when a module is located at an altitude of 3500 m (11482.80 ft) to
4500 m (14763.60 ft) and is 2 dB less than the standard power when a
module is located at an altitude of 4500 m (14763.60 ft) to 6000 m (19684.80
ft).
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.22

## NO TICE
● For details about the minimum configurable output power for each channel,
see the output power configuration rules of each RAT. Ensure that the carrier
output power of the cell is not less than the minimum configurable output
power of the RAT. Otherwise, the cell performance on the channel cannot be
ensured, and there is a possibility that the RF module functions abnormally and
hardware alarms are falsely reported.
● Assume that an RF module works in multiple frequency bands and a single
channel is configured with multiple cells in different frequency bands. Avoid
setting the carrier output power less than the minimum configurable output
power for all of the cells that work in the same frequency band. Such setup
cannot ensure the cell performance, RF performance, and power precision in
this frequency band, and significantly affects the cell performance, RF
performance, and power precision in other frequency bands on the same
channel. The minimum configurable output power of a cell varies depending on
the RAT. For details, see the output power configuration rules of each RAT.
For example, a single channel of an RF module is configured with one NR cell
in the 1800 MHz frequency band and one LTE cell in the 2100 MHz frequency
band. The carrier output power of the NR cell in the 1800 MHz frequency band
is 1 mW, which is less than the minimum configurable output power of the NR
cell on a single channel of the module. In this case, the cell performance, RF
performance, and power precision of the NR cell in the 1800 MHz frequency
band cannot be guaranteed. In addition, the cell performance and RF
performance of the LTE cell working in the 2100 MHz frequency band may
deteriorate, and the transmit power may be too low or too high.
GSM Output Power Configuration Rules
●  The standard bandwidth per GSM carrier is 200 kHz.
●  If the output power per GSM carrier on a single channel is required to be 60
W, the corresponding power license item must be purchased.
●  Before using the GSM power sharing function, ensure that the license item
"LGMIDPS-Dynamic Power Sharing (per TRX)" has been purchased. To enable
the power sharing function, run the SET GCELLCHMGAD command with
QTRUPWRSHARE set to DYNAMIC and MultiGSMDynPWShareSW set to
## ON.
●  For the GBTS and eGBTS, the output power per carrier of the same RF module
is the same. However, the unit of the output power per carrier is W for the
GBTS and dBm for the eGBTS. Power
P (unit: W) can be converted to x (unit:
dBm) by using the following formula: .
For example, when an RF module works in GSM mode, the output power per
carrier that can be configured for the GBTS is 60 W (GMSK). Then, the output
power per carrier that can be configured for the eGBTS is
, which is rounded
off to 47.8 dBm (GMSK).
●  To ensure the performance of a GSM cell and other cells that share the same
channel as the cell, the minimum configurable carrier output power per
channel for the GSM cell is equal to the total rated power per PA for an RF
module (unit: W) divided by 100. For example, the maximum output power of
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.23

an RF module is 2x80 W. When you configure a GSM cell, the minimum
configurable carrier output power per channel for the GSM cell is 0.8 W (80
## W/100).
●  The following table lists the available power configurations for each GSM
carrier. For details about the configurable GSM carrier power in different
carrier combinations, see
Typical Carrier and Power Configurations.
Table 5-1 Available power configurations for each GSM carrier
Output Power per Carrier (W)Output Power per Carrier (dBm)
## 80.049.0
## 60.047.8
## 40.046.0
## 31.044.9
## 30.044.8
## 27.044.3
## 25.044.0
## 20.043.0
## 16.042.0
## 15.041.8
## 14.041.5
## 13.341.2
## 13.041.1
## 12.040.8
## 11.040.4
## 10.040.0
## 9.539.8
## 9.039.5
## 8.539.3
## 8.039.0
## 7.538.8
## 7.038.5
## 6.037.8
## 5.537.4
## 5.037.0
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.24

Output Power per Carrier (W)Output Power per Carrier (dBm)
## 4.036.0
## 3.735.7
## 3.134.9
## 3.034.8
## 2.534.0
## 2.033.0
## 1.531.8
## 1.030.0

UMTS Output Power Configuration Rules
●  The standard bandwidth per UMTS carrier is 5 MHz.
●  The maximum output power of a UMTS cell is 100 W. To ensure the
performance of the UMTS cell and other cells that share the same channel as
the cell, the minimum configurable carrier output power per channel for the
UMTS cell is equal to the total rated power per PA for an RF module (unit: W)
divided by 100. For example, the maximum output power of an RF module is
2x80 W. When you configure a UMTS cell, the minimum configurable carrier
output power per channel for the UMTS cell is 0.8 W (80 W/100).
●  For details about the power configuration for each carrier combination when
the module works in UMTS mode, see
Typical Carrier and Power
## Configurations
## .
LTE FDD Output Power Configuration Rules
●  When multiple LTE FDD carriers are configured, it is recommended that the
power spectral density (PSD) of each carrier be set to the same value. PSD =
Carrier output power/Carrier bandwidth (1.4 MHz and 3 MHz bandwidths are
considered as 5 MHz bandwidth in this formula.)
●  To ensure the performance of an LTE cell and other cells that share the same
channel as the cell, the minimum configurable carrier output power per
channel for the LTE cell is equal to the total rated power per PA for an RF
module (unit: W) divided by 16. For example, the maximum output power of
an RF module is 2x80 W. When you configure an LTE cell, the minimum
configurable carrier output power per channel for the LTE cell is 5 W (80 W/
## 16).
●  For details about the power configuration for each carrier combination when
the module works in LTE FDD mode, see
Typical Carrier and Power
## Configurations
## .
LTE NB-IoT Output Power Configuration Rules
●  The formulas for calculating the minimum NB-IoT power per PA for an RF
module are as follows:
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.25

–   Minimum NB-IoT power per PA for an RF module when NB-IoT cells work
in guardband or in-band mode = min(23 dBm, maximum output power
per PA for an RF module – 40 dB)
–   Minimum NB-IoT power per PA for an RF module when NB-IoT cells work
in standalone mode = min(23 dBm, maximum output power per PA for
an RF module – 20 dB)
●  In standalone mode, the bandwidth spacing between two NB-IoT carriers
must be less than or equal to 300 kHz.
●  When the LTE bandwidth is 5 MHz, LTE NB-IoT cells cannot be deployed in
guardband mode.
●  After the NB-IoT multi-carrier function is enabled, one NB-IoT multi-carrier
cell can be configured with multiple NB-IoT carriers.
–   When an NB-IoT multi-carrier cell is configured in standalone mode, a
maximum of four NB-IoT carriers can be configured.
–   When an NB-IoT multi-carrier cell is configured in in-band mode and the
LTE bandwidth is 5 MHz, a maximum of four NB-IoT carriers can be
configured. If the LTE bandwidth is 10/15/20 MHz, a maximum of eight
NB-IoT carriers can be configured for an NB-IoT multi-carrier cell.
–   When a cell is configured with multiple NB-IoT carriers, the cell can have
only one anchor carrier but can have multiple non-anchor carriers.
## NO TE
The NB-IoT multi-carrier function is an NB-IoT multi-carrier transmission
technology introduced based on 3GPP Release 13. A cell can have multiple
carriers and assigns UEs to multiple carriers to increase cell capacity. For details
about this function and related parameter settings, see
NB-IoT Enhancements
## (FDD)
> Capacity Enhancement > Multi-Carrier Transmission in eRAN FDD
## Feature Documentation.
●  For details about the power configuration for each carrier combination when
the module works in LTE NB-IoT mode, see Typical Carrier and Power
## Configurations.
NR Output Power Configuration Rules
●  When multiple NR carriers are configured, it is recommended that the power
spectral density (PSD) of each carrier be set to the same value. The following
formula applies: PSD = Carrier output power/Carrier bandwidth.
●  To ensure the performance of an NR cell and other cells that share the same
channel as the cell, the minimum configurable carrier output power per
channel for the NR cell is equal to the total rated power per PA for an RF
module (unit: W) divided by 16. For example, the maximum output power of
an RF module is 2x80 W. When you configure an NR cell, the minimum
configurable carrier output power per channel for the NR cell is 5 W (80 W/
## 16).
●  For a single 4T cell, it is recommended that the carriers configured on the four
channels have the same power. Unbalanced power configurations are also
supported. For details about unbalanced power configurations, see
## Cell
## Management
## > Cell Management > Principles > Cell-related Parameters >
Cell Power in 5G RAN Feature Documentation.
●  For details about the power configuration for each carrier combination when
the module works in NR mode, see
Typical Carrier and Power Configurations.
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.26

## Multimode Output Power Configuration Rules
●  GUL/GUN (FDD)/GULN (FDD) carriers cannot be configured on the same
channel simultaneously in a single frequency band.
●  The output power per carrier must be balanced among multiple channels if
possible.
●  To ensure the performance of a cell and other cells that share the same
channel as the cell, the minimum total configurable output power of all
carriers per channel is equal to the total rated power per PA for an RF module
(unit: W) divided by 16. For example, if the maximum output power of an RF
module is 2x80 W, the minimum total output power of all carriers per each
channel is 5 W (80 W/16).
●  Non-MSR and MSR
–   Non-MSR: Carriers of different RATs cannot be configured on the same
RF channel. For example, a 2T RF module supports GU. If GSM carriers
are configured on PA1, then UMTS carriers cannot be configured on PA1.
That is, UMTS carriers can be configured only on PA2, and GSM carriers
cannot be configured on PA2.
–   MSR: Carriers of different RATs can be configured on the same RF
channel. For example, a 2T RF module supports GU. Both GSM carriers
and UMTS carriers can be configured on PA1 or PA2 simultaneously.
●  When LTE and NR carrier are configured, it is recommended that the power
spectral density (PSD) of each carrier be set to the same value. PSD = Carrier
output power/Carrier bandwidth (1.4 MHz and 3 MHz bandwidths are
considered as 5 MHz bandwidth in this formula.)
●  The GU frequency spacing can be calculated using the following formula: GU
frequency spacing ≥ [(GSM bandwidth/2) + (UMTS bandwidth/2)].
●  For details about the power configuration for each carrier combination when
the module works in multiple modes, see
Typical Carrier and Power
## Configurations
## .
## RRU5904
Technical Specifications5 RF Output Power Configuration Rules
## Issue Draft A
## (2025-06-30)
## Copyright © Huawei Technologies Co., Ltd.27