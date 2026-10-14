Page 1 of 9
WHITE PAPER
Discussions of timing and synchronization
often make reference to accuracy and
precision. In many cases, the difference
does not matter within the context, however,
```
for a more complete understanding; figure
```
2 draws an analogy to hitting the center of
a target.
Carrier networks achieve the necessary
precision and accuracy by basing
performance on a very precise and
accurate primary reference. The reference,
in nearly all cases, is from signals
transmitted by GNSS satellite systems
```
(GPS, GLONASS or Beidou). A high quality
```
GNSS receiver derives frequency and
Introduction
Once a routine network function, timing
and synchronization requirements are
changing rapidly as mobile network and
backhaul technologies evolve. Carriers
successfully solved the problem of
distributing frequency synchronization
through asynchronous Ethernet backhaul
networks using the IEEE 1588 Precision
```
Time Protocol (PTP) and/or Synchronous
```
```
Ethernet (SyncE). Looking forward, LTE-
```
Time Division Duplex and LTE-Advanced
impose new, very stringent time and phase
synchronization requirements. With the
advent of small cells, several additional
backhaul technologies are in the mix.
Together, stringent timing for phase and
new backhaul technologies for small cells
have pushed cell site synchronization
issues to the forefront.
This paper reviews the requirements and
challenges of timing and synchronization
for LTE-TDD, LTE-A and backhaul
networks, considers the problems that
must be solved, and presents solutions that
are being proposed and developed. While
each section could easily be the subject of
a separate paper with deeper coverage, it
is the purpose of this paper to provide a
general overview of the subject.
Synchronization and UTC Traceability
Timing and synchronization are
fundamental to digital network operations.
Historically, relatively easy frequency
synchronization was all that was required.
LTE-TDD and LTE-A technologies add
requirements for phase and time. Figure 1
helps to understand the differences.
Timing and Synchronization for LTE-TDD
and LTE-Advanced Mobile Networks
Frequency Synchronization
A
B
T A=1/fA
```
TB=1/fB
```
```
fA =fB
```
```
fA =fB
```
t
t
Phase Synchronization
A
B
T A=1/fA
T A=1/f A
```
TB=1/fB
```
t
t
Time Synchronization
A
B
```
TB=1/fB
```
t
```
fA=fB
```
t
01:00:0001:00:10
01:00:0001:00:10
```
TA =1/fA
```
Leading edge of the pulses
are at same pace, but not
at the identical moment.
Leading edge of the pulses
are at identical moment.
Leading edge of the pulses
are at the identical moment
and identical time.
... Figure 1: Frequency, Phase and Time Synchronization
.. ...
Precise &accuratePrecise butnot accurate Accurate butnot precise
... Figure 2: Accuracy and Precision
WHITE PAPER
Page 2 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
calculates time from the satellite signals,
and the synchronization equipment then
uses it as a reference for network timing.
The best timing and sync equipment will
also use additional frequency inputs such
as Synchronous Ethernet or E1/T1 signals
which enable the solution to converge more
quickly on the precise and accurate time, and
improve holdover when the GNSS signals are
impaired or only available intermittently.
It is essential that the time and phase
reference in LTE-TDD and LTE-A networks
is traceable to Coordinated Universal Time
```
(UTC). ITU-T G.8272 defines requirements
```
```
for a Primary Reference Time Clock (PRTC);
```
a time and phase advancement compared
to the long established standards for
```
the Primary Reference Clocks (PRC) and
```
```
Primary Reference Sources (PRS) used
```
for frequency synchronization. Without
the common UTC time reference cell sites
cannot operate as intended. It must be
emphasized that SyncE is only a frequency
reference, and cannot be used by a PTP
```
clock (such as a Boundary Clock) as a
```
primary time reference.
Timing and Sync Requirements for LTE
2G, 3G and LTE-Frequency Division Duplex
mobile technologies require only frequency
synchronization with accuracy within 50
parts per billion at the radio interface. To
meet this requirement, 16 ppb is specified
at the base station interface to the backhaul
network. LTE-Time Division Duplex and LTE-
Advanced services have the same frequency
requirement as the earlier generations, but
also specify requirements for phase and
time. Figure 3 provides a summary of the
synchronization requirements.
LTE-Advanced requirements are a work-in-
progress in the standards bodies. Though
```
not consented at this time (mid-2013) it is
```
probable that the requirements will be ±1.5
```
μs or ±5 μs depending on the application;
```
though some of the discussion indicates that
```
500 nanoseconds (±.5 μs) may be required
```
for some service situations. LTE-A covers
multiple techniques rather than a single
technology. Not all features will be deployed
everywhere, leading to differences in real
world requirements. Figure 4 presents what
they may be when the standards are complete.
Residential and enterprise small cells, also
known as femtocells, are different in that they
use broadband Internet access service as
their backhaul. As such, they are not covered
in the solutions described in this paper
which address distributing synchronization
over mobile backhaul networks. These cells
typically use the less precise Network
```
Time Protocol (NTP), and require frequency
```
accuracy of 100-250 ppb for their air interface.
Impact of Failure
Investment in small cells and LTE networks
is made to increase capacity and coverage.
When synchronization fails, both objectives
are lost. Figure 5 presents a “cumulative”
look of what can go wrong.
... Figure 3: Frequency and Phase Synchronization Requirements
... Figure 5: Why Synchronization is Important.
Application Frequency Network /Air Phase Note
GSM, UMTS, WCDMA, LTE – FDD 16 ppb / 50 ppb -- --
CDMA2000 16 ppb / 50 ppb ± 3 μs to ± 10 μs --
LTE – TDD 16 ppb / 50 ppb ± 1.5 μs ≤ 3 km cell radius± 5 μs > 3 km cell radius
LTE MBMS
```
(LTE-FDD & LTE-TDD) 16 ppb / 50 ppb ± 10 μs
```
inter-cell timedifference
LTE- Advanced 16 ppb / 50 ppb ± 1.5 μs to ± 5 μs In discussion bymembers of the 3GPP
Application Need for compliance Impact of non-compliance
LTE -FDD Call initiation Call interference and dropped calls
LTE -FDD Time slot alignment Packet loss/collisions and spectral inefficiency
LTE-A MBSFN Proper time alignment of videosignal decoding from multiple BTSs Video broadcast interruption
LTE-A MIMO/
COMP
Coordination of signals to/frommultiple base stations Poor signal quality at edge of cells, LBSaccuracy
LTE-A eICIC Interference coordination Spectral inefficiency and service degradation
LTE-Advanced Type of Coordination Phase
eICIC enhanced Inter-cell Interference Coordination ± 1.5 to ± 5μs
CoMP Moderate to
tight
UL coordinated scheduling ± 5 μs
DL coordinated scheduling ± 5 μs
CoMP Very tight
DL coordinated beamforming ± 1.5 μs
DL non-coherent joint transmission ± 5 μs
UL joint processing ± 1.5 μs
UL selection combining ± 1.5 μs
UL joint reception ± 1.5 μs
... Figure 4: LTE-Advanced Synchronization Requirements
Needs and Impacts are cumulative, that is: “plus all of the above”.
WHITE PAPER
Page 3 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
Enhanced Intercell Interference
```
Coordination (eICIC) wholly depends on
```
the accuracy of distributed time. Out-of-
spec timing in networks that require only
frequency synchronization impacts only the
footprint of the failed NodeB. In LTE-TDD
and LTE-A networks, eICIC enables small
cells to operate in cooperation with each
other and with overlapping macro cells.
Should a cell transmit at the wrong time,
it will interfere with the signals at the
other base stations in the coverage area—
leading to overall spectral inefficiency and
broader service degradation.
Solutions for Stringent Time and Phase
Synchronization
There are three primary techniques
to meet the stringent phase and time
synchronization requirements of LTE-TDD
and LTE-A networks: “GNSS everywhere”,
PTP with “full on-path support”, and
PTP with “partial on-path support and/
or Edge Grandmaster”. Each solution has
advantages and disadvantages, and we will
look at each in turn.
GNSS Everywhere
A seemingly simple approach is to deploy
a GNSS receiver with every mobile base
station. The GNSS receiver can be a
standalone device or embedded into the
base station. A GNSS receiver can also
be integrated into a collocated or nearby
```
cell site router (CSR) or network interface
```
```
device (NID) if they also support sync
```
distribution to the base station, typically
using PTP. Though straight forward, this
approach is not economically or technically
feasible at every location, and it will also
leave the eNodeBs vulnerable to GNSS
signal interference.
Challenges to economic or technical
feasibility are most pronounced in the case of
public access small cells. These small cells
```
(also known as metro cells, microcells and
```
```
picocells) are planned for deployment where
```
either higher capacity or greater coverage
```
is needed. Many (perhaps most) of these
```
environments do not provide easy access
to GNSS signals. Cell sites may be indoors
such as in sports arenas, concert venues,
shopping malls or office buildings where
satellite signals do not reach and where it is
not feasible to connect to a remote antenna.
Many outdoor locations also present
problems. Urban canyons, where small
cells must be located near street level, offer
limited visibility to the upper atmosphere.
Deployed in the shadow of tall buildings, the
base stations cannot see or lock onto the
multiple satellite signals needed to make
precise time calculations. Additional problem
deployment areas include tunnels and
subways, and even city parks and tree lined
streets where dense foliage can attenuate
satellite signals below the level of receiver
sensitivity.
Though pricing models for small cell
base station equipment offerings are still
emerging, it is reasonable to assume there
will be a cost for an integrated GNSS receiver
and antenna—a cost that will be borne by
every small cell deployment that uses it.
Though smaller as a percentage of total site
costs, GNSS installation and maintenance
also figure in to the capital and operational
expense of macro sites as well. Figure
6 attempts to convey that, while GNSS
receivers and antennas are not expensive
individually, the large number of locations
and the on-going maintenance may prove
this alternative to be a poor economic choice.
The vulnerability of GNSS signals is of
growing concern. The signals are very
weak at the earth’s surface and easily
interfered with. Though usually discussed
in the context of positioning systems, such
things as GPS jammers and spoofers,
atmospheric interference, multi-path
from reflected signals, radiation from
malfunctioning electronics, or simply bad
weather damaging an antenna installation
are common causes for failure. These
vulnerabilities can be mitigated with a
...
. Figure 6: GNSS for Every Base Station, Cell Site Router or NID
AGGREGATIONCORE ACCESS
WHITE PAPER
Page 4 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
high quality holdover oscillator such as
a rubidium miniature atomic clock in
```
the base station; but, though feasible in
```
macro base stations, this solution is not
economically practical for small cells.
Carriers choosing “GNSS everywhere” still
need a solution for situations where it is
not feasible, and best practice also points
to the need for a backup timing source.
Consequently, the network distributed time
solutions described below will have an
important role for every carrier: either as the
primary timing solution, as an alternative
source where GNSS cannot be deployed, or
as a backup when GNSS is impaired.
The IEEE 1588 Precision Time Protocol
```
(PTP) was developed in response to
```
broad industry and government need to
enable accurate distribution of time and
frequency over packet-based networks.
IEEE 1588 employs a client/server
architecture to maintain precise
synchronization across all network
```
components. The server (PTP
```
```
Grandmaster Clock) is the primary
```
reference source for all of the PTP
clients within its network domain. It
continuously sends out sync, follow-up
and delay response messages to all of
its clients. Clients continuously send
delay request messages to the server
to maintain synchronization through the
packet-based network. Using the time
stamped packets, clients determine
frequency and calculate accurate
time that is traceable to the primary
reference of the Grandmaster.
The IEEE standard is designed broadly
to serve a great variety of applications.
To enable ease of deployment and
equipment interoperability while
meeting the requirements of specific
applications, IEEE 1588-2008
introduced the concept of profiles.
Profiles specify particular combinations
of PTP options and attribute values
to support a given application. For
example a profile may specify layer
2 or layer 3, unicast or multicast, the
message exchange rate, and whether
on-path support is required. The
```
“Telecom Profile” (recommendation
```
```
ITU-T G.8265.1) is intended to address
```
the application of PTP to the frequency
synchronization of telecommunication
systems, primarily cellular base stations.
ITU-T G.8275.1 and G.8275.2 are works-
in-progress to address time and phase
synchronization.
The PTP standard includes provisions
to maintain accuracy across a network
```
(refer also to the sidebar Packet Delay
```
```
Variation and Asymmetry). Boundary
```
Clocks are one option for this on-path
support. Usually embedded in network
elements, Boundary Clocks function as
a PTP client in the upstream direction
and as a grandmaster to other Boundary
Clocks and clients in the downstream
direction. By compensating for delays
in the switch and refreshing the PTP
packets, Boundary Clocks help to
maintain accuracy and are still traceable
to the original Grandmaster clock with a
primary UTC reference.
IEEE 1588 also defines Transparent
Clocks as a technique to support
accuracy across a network. Transparent
Clocks are not currently provided for in
the PTP profiles for telecom industry,
and need not be covered here.
Physical layer
Network protocolstack & OS
Physical layer
Network protocolstack & OS
Server Client
IEEE 1588 processor
t1
t4
t2
t3Sync detector &timestamp generator
Master clock sends:1. Sync message
2. Follow_up message4. Delay_resp. message
Master Network
Sync
delay_req.
follow_up
delay_resp.
Slave
Slave clock sends:3. Delay_ req. message
IEEE 1588 processor
Sync detector &timestamp generator
Ethernet/IP
Network
PTP, Profiles and Boundary Clocks
WHITE PAPER
Page 5 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
PTP Profile with Full On-path Support
```
(G.8275.1)
```
IEEE 1588-2008 Precision Time Protocol
is a proven technology for distributing
synchronization over packet-based
backhaul networks to mobile network
elements that require frequency
synchronization. There are hundreds of
networks successfully using this technology
today following the G.8265.1 standard PTP
profile or a pre-standard implementation. It
is typically deployed using a centralized PTP
```
Grandmaster (with GNSS primary reference
```
```
to meet G.8272 PRTC requirements), which
```
then interoperates with slave or client
software in the mobile network elements,
enabling the client to determine frequency
and calculate the time.
PTP, using the frequency profile as
deployed today, will likely not meet the
stringent time and phase accuracy
requirements of LTE-TDD and LTE-
Advanced networks. Consequently the ITU
is developing new standards, including new
profiles that take advantage of capabilities
provided for in IEEE 1588-2008.
ITU-T G.8275.1 is a work-in-progress for a
new PTP profile that enables the stringent
time and phase requirements at the base
station to be met over a network from a
centralized PTP Grandmaster many hops
away. Maintaining precision and accuracy
is achieved through deployment of “full
on-path support” of the PTP timing signals.
On-path support is provided by a Boundary
Clock function embedded in every
network element in the path between the
```
grandmaster and the client; including all
```
switches, routers, microwave radios, NIDs,
```
etc. Each Boundary Clock (BC) incorporates
```
a PTP client that interoperates with its
immediate upstream element to recover
time, and then acts as a PTP Grandmaster
to deliver time to connected downstream
Boundary Clocks or end device clients.
```
Synchronous Ethernet (SyncE) is covered
```
in the proposed standard as providing
frequency reference support for better
performance, but it is not a requirement.
Early experience indicates SyncE should be
included in the deployments. Figure 7 is a
simplified depiction of a network following
the G.8275.1 PTP profile.
Full on-path support will best fit
scenarios where new backhaul equipment
is being deployed at every location
```
(i.e.: Greenfields), but it has practical
```
disadvantages in other network scenarios.
Many mobile service providers do not
own or control their backhaul networks.
Independent, third party backhaul network
providers may not be willing to upgrade
their network elements for full on-path
support, or may only do so at increased
prices to the mobile network operator.
Even wireline networks owned by the
same company as the mobile operator
may resist the cost of a comprehensive
upgrade, retrofit or replacement. As
precise timing has become an essential, yet
more difficult, component for evolving LTE
networks, a “sync SLA” should be included
in the relationship between wireless and
backhaul operations, and monitoring and
reporting added to operational practices.
Pre-standard ITU-G.8275.1, in early
deployments, use layer 2 multicast.
While this may present no problem in
Greenfield scenarios, many carriers have
implemented network policies for MPLS
and IP networking at higher layers that
```
may have to be revised (and networks
```
```
re-engineered) to implement a multicast
```
network service at layer 2.
AGGREGATIONCORE ACCESS
Small CellAggregation
Metro Small Cells
Macro eNodeB
Rb
PTP GM
PTP GM
SyncESyncESyncE
SyncESyncESyncESyncES E
BC
SyncE
SyncE
~
~ ~ ~
~
S E
BC
S E
BC
SyncES E
BC
S E
BC
S E
BC
Macro eN
SyncES E
BC
mall Cell
SyncES E
BC
S E
BC
S E
BC
S E
BC
S E
BC
... Figure 7: Backhaul network using the ITU-T G.8275.1 profile for phase synchronization
WHITE PAPER
Page 6 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
Packet Delay Variation and Asymmetry
Another problem introduced by the
need for stringent phase and time
synchronization is the impact of packet
```
delay variation (PDV) or asymmetry as the
```
PTP packets travel back and forth across
the network. Boundary Clocks adjust the
timestamp to account for the time resident
in the network element, including packet
processing, buffering and queuing delays
that create packet delay variation which
would otherwise introduce errors in the
time calculation. However, Boundary
Clocks alone cannot compensate for path
asymmetry—differences in the upstream
and downstream paths between the
grandmaster and client. Network path
asymmetry can be severe enough to move
the time calculations of the client out of
spec, requiring the operator to manually
measure and enter time offset adjustments
to compensate, and then adjust when the
paths change.
Timing and synchronization, fundamental
in all mobile networks, is even more
critical as small cells are added and
networks evolve to LTE-TDD and
LTE-A technologies. Backhaul network
performance can dramatically impact
PTP timing accuracy, and thereby the
mobile network itself—affecting service
quality and customer satisfaction.
The problem is Packet Delay Variation
```
(PDV) which represents the change
```
in latency from packet to packet.
Packet delay itself has no effect on
the accuracy of the clock: constant
delay would allow an accurate time
offset calculation by the PTP client.
Variable delay, however, induces noise
in the PTP client’s perception of the
time at the master which can result in
variation in time calculations based on
the timestamps in the PTP packets.
Delay can vary as PTP packets are
processed, buffered and queued along
with the payload traffic through the
network switches and routers, and
it tends to be correlated to network
load which can be highly asymmetric in
nature. As the amount of traffic in the
network increases, the delay variation
is also likely to increase. Asymmetry is
also introduced by the physical topology
of the network as packets travel different
and changing paths in the upstream and
downstream directions.
Time accuracy is affected by both the
magnitude of the packet delay variation
and how effective the client is at
removing this noise. Synchronization
elements deployed in the network vary
in how effectively they filter this noise.
Embedded Boundary Clocks adjust only
for the switch delay variation in its host
```
switch; it cannot adjust for variations or
```
asymmetries in other network switches
and it cannot compensate at all for
network path asymmetry. Network
timing elements with a GNSS reference
can compensate for all variations,
including network path asymmetry.
Comparing a PTP input from a
centralized grandmaster and a local
```
GNSS reference; an Edge Grandmaster
```
can determine the typical offset and
apply it to provide superior accuracy
when the GNSS reference is not
available. Superior designs learn
multiple offset for different backhaul
network paths and continue to provide
accurate performance even through
backhaul network rearrangements.
Sources of Asymmetry
1. Switch delay variation:
- Switch transit: packet processing,
buffering and queuing
- Payload variation increases
variation in switch delay
2. Network path variation:
- Variation between upstream and
downstream paths in the network
- Path asymmetry alone can
cause timing performance to be
out of spec.
- An out-of-phase cell can impact
services on overlapping cells
WHITE PAPER
Page 7 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
reference to maintain high accuracy
timestamps to the next clients in the path.
Edge Grandmasters ensure accuracy
by deploying closer to the clients, and
thereby reducing the hops and putting
problem parts of the backhaul network
behind them. Edge Grandmasters include
a GNSS reference to meet G.8272 PRTC
requirements and perform much the like
centralized PTP Grandmaster equipment
commonly deployed today, except they are
scaled and cost optimized for deployment
closer to the network edge.
Figure 8 depicts some of the many network
scenarios that can be solved with partial
on-path support and/or Edge Grandmaster
deployment.
separately or in combination to provide the
best synchronization architecture for a wide
range of network scenarios.
“Partial on-path support” is deployment of
advanced boundary clocks at intermittent
locations through the network. In a
managed Ethernet network it may be
possible to locate an advanced boundary
clock at selected locations and maintain
timing within spec at the base stations.
Key to this approach is to limit the number
of hops and path asymmetry between the
grandmaster and the client. Advanced
boundary clocks have superior oscillators
and can leverage additional inputs such as
SyncE and E1/T1 circuits as a frequency
PTP Profile with Partial On-path Support
```
and/or Edge Grandmaster (G.8275.2)
```
Responding to the need for a phase
timing solution that is more feasible in
non-Greenfield, real-world scenarios,
```
another PTP profile (G.8275.2) has been
```
proposed to the ATIS/ITU standards
```
bodies: “a new profile to support time and
```
phase distribution over existing deployed
networks…compatible with the PTP
profile for frequency distribution defined
in G.8265.1”. This proposal will require
considerable more work before it becomes
a standard, but in practice, it can be
deployed in networks today.
In simple terms, this approach endorses
two solutions that can be employed
AGGREGATIONCORE ACCESS
PTP GM
Edge GM
High PDV or 3rd Party
Macro eNodeB
Boundary Clock
Edge GM
PTP GM
~~
~
~
~~
~
~
~
~
~
Boundary Clock
Microwave Edge GM
~
~
~
OLT ONU
PON
DSLDSLAM modem
... Figure 8: Partial on-path support and/or Edge Grandmaster deployment scenarios
WHITE PAPER
Page 8 of 9
Timing and Synchronization for LTE-TDD and
LTE-Advanced M obile Networks
this architecture, is that relatively nearby
Edge Grandmasters can backup each other
```
(shown in figure 10), as opposed to requiring
```
PTP clients to re-sync with a centralized
grandmaster that may be so many hops
away that accurate timing is not possible.
Timing and synchronization are a critical
component to LTE-TDD and LTE-Advanced
network operations, and therefore protecting
this function is more essential than ever.
Enhanced holdover is one protection
alternative. Another alternative, enabled by
Though outside the topic of the paper, it is
worth noting that the solution described
above and illustrated in figure 8 may also
be applied for frequency synchronization in
2G, 3G and LTE-FDD networks where many
of the same issues related to backhaul
network performance and control exist.
Edge Grandmasters may include a PTP
input capability, allowing PTP signal
exchanges with a centralized grandmaster
to continue as a precise time reference
should the GNSS reference be impaired.
During periods of normal operation the
Edge Grandmaster will track the time
offset between the GNSS calculation and
the calculation based on PTP with the
centralized grandmaster. When GNSS is
lost, the Edge Grandmaster can apply that
offset to the PTP calculation and continue
to provide a level of accurate timestamps
that the backhaul network alone could
not support.
Additional capabilities in both advanced
PTP Boundary Clocks and Edge
Grandmasters may include utilizing a
frequency input such as SyncE or E1/T1
as an additional reference, and providing
extended holdover for all connected clients
with a higher quality oscillator such as
a rubidium miniature atomic clock as
depicted in figure 9.
Edge GM or BCwith rubidium
oscillator
Rb
...
..Figure 9: A single rubidium oscillator providesextended holdover to multiple base stations.
... Figure 10: Edge Grandmasters provide backup to each other.
ACCESS
ACCESS
Edge GM
Edge GM
Edge GM
Edge GM
NORMAL OPERATION
SYNC AND TIMING PROTECTION
WHITE PAPER
Timing and Synchronization for LTE-TDD and
LTE-Advanced Mobile Networks
Timing and Synchronization for LTE-TDD and
LTE-Advanced Mobile Networks
2300 Orchard ParkwaySan Jose, California 95131-1017
```
tel: 408.433.0910 fax: 408.428.6960www.symmetricom.com
```
WP_TIMESYNCLTE/080313
© 2013 Symmetricom. Symmetricom and the Symmetricom logo are registered trademarksof Symmetricom, Inc. All specifications subject to change without notice.
Full on-path support is most feasible in
Greenfield situations where every new
switch and router can include SyncE and
Boundary Clock support. Network path
asymmetry and sync protection remain
as issues.
Edge Grandmasters deployments or
advance Boundary Clock offer the flexibility
to fit a wide range of network scenarios
and offer solutions for sync protection and
can compensate for all switch and path
asymmetry.
Symmetricom® is a leader in PTP
Grandmaster deployments for mobile
networks and stands ready to help analyze
and recommend the right solution for your
operation. Additional technical information,
test results, recommended best practices,
cost comparison aid, equipment
demonstration, lab test procedures
and network sync audit aids can all be
made available to help plan the best
synchronization distribution architecture
for your network. And, of course,
Symmetricom supplies and supports
best-in-class PTP Grandmaster, Edge
Grandmaster, and advanced Boundary
Clock equipment, to network operators
around the world.
```
Conclusion: Finding the Right Solution
```
for Your Network
The important and difficult question:
“How should I synchronize my LTE-TDD
and LTE-Advanced networks?” does not
have a single easy answer. The stringent
requirements for phase and time cannot
be met using the typical “frequency
synchronization distributed over the
backhaul network” techniques in
practice today, and so new solutions must
be adopted.
The right answer for your network is
driven by your service delivery network
```
fundamentals:
```
• The mobile network technology and
services determines the timing and
synchronization requirements: LTE-
TDD, LTE-A, eICIC requirements, CoMP
requirements, etc.
• Mobile network equipment selection and
```
cell site locations (particularly for small
```
```
cells) define what can and cannot be
```
done.
• Backhaul network technologies,
topologies, performance and control
drive decisions for synchronization
equipment and deployment locations.
Once the technical limits and possibilities
are understood, the solution alternatives
and their relative costs can be assessed.
Simply deploying GNSS receivers and
antennas everywhere is not economically
or technically feasible for all situations,
and GNSS alone exposes the base stations
to the vulnerabilities of the satellite signal
based systems. Network distributed
time, using the IEEE 1588 Precision Time
Protocol, will be part of virtually every
mobile network operator’s network.
Edge Grandmaster and/or partial on-path
support with advanced Boundary Clocks
provide many advantages:
• Tremendous flexibility to work in diverse
network scenarios provides network
planners with the tools for every situation
• Enables small cell deployments where
GNSS/GPS is not economically or
technically feasible
• Cost savings by avoiding backhaul
network upgrades for embedded
```
Boundary Clocks (and possibly also
```
```
upgrade for SyncE)
```
• Avoids issues related to high packet
delay variation, asymmetry and/or 3rd
party backhaul
• Timing and synchronization protection
techniques to maintain high mobile
network availability and performance
• Synchronization reliability is not
threatened by failure of one of many
```
embedded Boundary Clock (where failure
```
of one BC breaks the timing chain to the
```
downstream clocks)
```
• Makes extended holdover possible as
cost of a superior rubidium oscillator is
leveraged across multiple base stations
• Leverages existing investment in
centralized PTP grandmaster and SyncE,
preserves practices put in place for
frequency synchronization
• Preserves MPLS network and engineering
```
practices (operates at layer 3)
```