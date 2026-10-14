

## 89
FUJITSU Sci. Tech. J., Vol. 48, No. 1, pp. 89–94
(January
## 2012
## )
Inter-Cell Interference Coordination (ICIC)
## Technology
## 
## Dai Kimura
## 
## Hiroyuki Seki
Long Term Evolution (LTE) is a promising standard for next-generation cellular
systems targeted to have a peak downlink bit rate of 150 Mb/s.  However, as adjacent
cells use the same frequency, interference between adjacent cells may degrade
the bit rate at cell edges, preventing sufficient throughput from being obtained.
Inter-cell interference coordination (ICIC) is a promising technology for alleviating
this degradation and improving the bit rate at cell edges.  In the LTE standard,
an interface between adjacent base stations is specified for exchanging ICIC
information.  However, no methods or control algorithms have been specified for
using this interface, leaving it to base station vendors to develop them on their own.
This paper outlines ICIC technology in the LTE system, describes the original ICIC
algorithm we have developed, and discusses its evaluation.
## 1. Introduction
As  an  extension  of  the  third-generation
mobile communications system, the Long Term
Evolution  (LTE)  system  is  aimed  at  achieving
high  spectral  efficiency  through  the  use  of  a
one-cell-reuse  frequency  allocation  system  that
allocates  the  same  frequency  to  adjacent  cells,
the same as in the third-generation system.
note 1)

In  a  one-cell-reuse  system,  however,  there  is
much  interference  between  cells,  which  may
prevent   sufficient   throughput   from   being
obtained at cell edges.  The need was therefore
felt  for  making  further  improvements  in  LTE
spectral efficiency, and to this end, a throughput
at a cell edge throughput 2-3 times that of the
high  speed  downlink  packet  access/high  speed
uplink  packet  access  (HSDPA/HSUPA)  3.5th
generation   mobile   communications   system
was  established  as  a  target.
## 1)
In  light  of  the
above,  the  3rd  Generation  Partnership  Project
note 1)   In  a  mobile  communications  system,  “cell”
refers to a region in which radio signals from
a specific base station antenna dominate.
(3GPP)—the   LTE   standardization   body—
energetically discussed drawing up specifications
for inter-cell interference coordination (ICIC) as
a technology for reducing inter-cell interference
and improving throughput at cell edges.  These
discussions  resulted  in  the  specification  of  an
interface between base stations (the X2 interface)
for    exchanging    interference-coordination
information.
## 2)
However,  no  methods  or  control
algorithms have been specified by the 3GPP for
using  this  interface,  leaving  it  to  base  station
vendors to develop them on their own.
In  this  paper,  we  first  describe  the  basic
principle behind ICIC technology and outline the
interface between base stations specified in the
LTE  standard.    We  then  describe  the  original
ICIC algorithm that we developed to implement
ICIC  and  present  the  results  of  computer
simulations  that  we  performed  to  assess  the
effectiveness of this algorithm.
- ICIC operation principle
Figure  1  shows  different  frequency-

## 90
FUJITSU Sci. Tech. J., Vol. 48, No. 1
(January
## 2012
## )
D. Kimura et al.: Inter-Cell Interference Coordination (ICIC) Technology
usage  scenarios  when  one  base  station  is  used
to  configure  three  cells  (sectors).    Inter-cell
interference becomes a problem when the same
frequency  band  is  used  for  adjacent  cells,  as
shown in Figure 1(a).  This type of interference
can be reduced by allocating different frequency
bands  to  adjacent  cells  (frequency  reuse),  but
this narrows the band that can be used by each
cell,  which  reduces  throughput,  as  shown  in
Figure  1(b).    This  is  why  frequency  reuse  is
not  executed  in  normal  LTE  systems,  which
instead  use  only  one  frequency  in  a  method
called  “frequency-reuse  1.”    To  resolve  this
issue,  a  method  called  fractional  frequency
reuse (FFR) was developed.  As shown in Figure
1(c),  the  FFR  method  separates  the  frequency
bands allocated to the areas near a base station
where  no  signal  interference  from  adjacent
base  stations  occurs  from  the  frequency  bands
allocated to the areas far from the base station
where  signal  interference  from  an  adjacent
base station can occur.  The transmit power is
reduced and the frequency-reuse factor is set to
1 for the frequency band allocated to the cell area
where no signal interference from adjacent base
stations  occurs,  and  conversely,  the  transmit
power  is  increased  and  the  frequency-reuse
factor is set to 3 for the frequency band allocated
to the cell area where signal interference from an
adjacent base station can occur.  This improves
the signal to interference plus noise ratio (SINR)
and throughput for users located at the cell edge
without degrading spectral efficiency.
ICIC based on FFR is therefore considered
to  be  an  effective  method  for  use  in  the  LTE
downlink.    For  the  uplink,  a  method  based  on
this principle (shifting the bands used by users in
areas where signal interference from an adjacent
base station can occur) should also be effective.
- ICIC standardization
To  implement  FFR,  the  frequency  band
allocated  to  a  user  at  a  cell  edge  must  be
different from that allocated to another user in
the adjacent cell, as shown in Figure 1(c).  The
LTE  standard  specifies  an  inter-base-station
interface that enables adjacent base stations to
exchange information on bands generating large
interference in other cells and on bands that are
affected  by  large  interference  from  other  cells.
## Figure 1
Frequency allocation methods for cellular systems.
## Cell 1
## Cell 2
## Cell 3
Base station
## Cell 1
## Cell 2
## Cell 3
Base stationBase station
## Cell 1
## Cell 2
## Cell 3
## Frequency
Transmit power
## Cell 1
## Cell 2
## Cell 3
## Frequency
Transmit power
## Cell 1
## Cell 2
## Cell 3
## Frequency
Transmit power
## Cell 1
## Cell 2
## Cell 3
## (a) Frequency-reuse 1
## (b) Frequency-reuse 3
(c) Fractional frequency reuse (FFR)
Frequency-reuse 3 for cell-edge band

## 91
FUJITSU Sci. Tech. J., Vol. 48, No. 1
(January
## 2012
## )
D. Kimura et al.: Inter-Cell Interference Coordination (ICIC) Technology
The following describes interference-coordination
signals that can be used for implementing ICIC
in the downlink and uplink.
## 1)    Downlink
The signal used for interference coordination
in  the  downlink  is  called  relative  narrowband
transmit  power  (RNTP).    This  signal  can  take
a  value  of  0  or  1  and  is  sent  to  multiple  base
stations serving adjacent cells for each resource
block  (RB).
note  2)
Specifically,  this  value  is  set
to 0 if the ratio between the transmit power of
the downlink signal allocated to the RB and the
average transmit power of the system frequency
band  is  guaranteed  to  be  under  a  certain
threshold  and  to  1  otherwise.
## 3)
This  scheme
enables a base station to learn about an RB that
may be transmitting at high power in an adjacent
cell  and  to  reduce  interference  by  avoiding
allocating  that  RB  to  a  user  experiencing  poor
reception.  Increasing the transmit power above
the system average for a user experiencing poor
reception should also improve the quality of that
user’s reception.
## 2)    Uplink
There  are  two  types  of  signals  for
interference  coordination  in  the  uplink:  high
interference  indicator  (HII)  and  interference
overload indicator (OI).  The HII signal is used
by  a  base  station  to  notify  to  multiple  base
stations  serving  adjacent  cells  of  the  uplink
RB  it  has  allocated  to  a  cell-edge  user.    This
enables  cell-edge  users  in  adjacent  cells  to  be
allocated  different  bands,  the  same  as  in  the
downlink approach, which means that improved
throughput  can  be  expected  for  these  cell-edge
users.    The  OI  signal,  on  the  other  hand,  is
used by a base station to notify to multiple base
stations  serving  adjacent  cells  the  results  of
measuring  interference  power  for  each  RB  and
classifying  those  results  into  multiple  levels.
Thus,  the  base  station  of  a  cell  that  receives
notification  of  high  interference  power  from
note 2)   RB is a unit of allocation in the frequency
domain having a bandwidth of 180 kHz.
an adjacent cell can reduce the transmit power
of  its  users  and  thereby  reduce  the  amount  of
interference created in the adjacent cell.
- Proposal of original algorithm
4.1 Conventional interference-
coordination method and associated
problems
We  decided  to  investigate  the  control
signals  introduced  in  the  previous  section  for
achieving ICIC and algorithms for using them.
On  examining  techniques  proposed  at  3GPP
standardization  meetings,  we  found  that  a
method for changing the transmit power of the
cell-edge band on the basis of the RNTP from an
adjacent cell had been proposed,
## 4)
which we can
treat as a conventional interference-coordination
method.    In  this  method,  cell-edge  bands  are
uniformly  fixed,  as  in  Figure  1(c).    In  actual
cellular  mobile  communications,  however,  the
following several factors make cell shape complex
and difficult to predict.
1)    Radio  propagation  characteristics  differ  in
accordance with topography and buildings.
2)    Base  stations  with  different  transmit
powers and antenna heights coexist.
3)    Distances  between  base  stations  are  not
uniform  due  to  restrictions  on  where  they
can be installed.
4)    User distribution is non-uniform, generating
bias.
This makes it difficult to determine the cell-
edge band for each cell.  Moreover, the optimal
cell-edge band can be considered to change over
time.  Thus, if the method for allocating cell-edge
bands between adjacent cells is fixed, an optimal
ICIC effect may be difficult to obtain.
4.2 Interference-coordination method
considering user distribution
For ICIC based on FFR, it can be seen from
the above discussion that a mechanism is needed
to  automatically  determine  the  cell-edge  band
for  each  cell  under  various  conditions  such  as

## 92
FUJITSU Sci. Tech. J., Vol. 48, No. 1
(January
## 2012
## )
D. Kimura et al.: Inter-Cell Interference Coordination (ICIC) Technology
a biased user distribution and non-uniform cell
arrangement.    At  the  same  time,  a  variety  of
factors in actual cellular mobile communications
as  described  above  are  likely  to  affect  the
distribution of signal quality for users within a
cell.  In response to this situation, we developed
an original ICIC algorithm for LTE base station
equipment  to  automatically  optimize  cell-edge
bands  by  focusing  on  user  distribution  (in
particular,  receive-power  distribution).
## 5)
## We
outline the proposed algorithm below.
This  ICIC  algorithm  adaptively  selects
a  cell-edge  band  of  a  cell  on  the  basis  of
coordination information from adjacent cells and
notifies the base stations of the adjacent cells of
the band selected.  The base station of each cell
uses the received information and the following
equation to compute cell-edge-band metric A
k
for
each sub-band.
w
j
## X
j,k
## A
k
j  J
## Here, X
j,k
denotes  received  information  on
sub-band k from adjacent cell j.  It takes a value
of  1  for  a  cell-edge  area  and  0  otherwise  (this
information  can  be  exchanged  between  base
stations  using  the  RNTP  or  HII  signals).    The
symbol w
j
denotes weight with respect to adjacent
cell j,  that  is,  the  number  of  users  for  which
the  difference  between  the  power  of  the  signal
received from the serving cell and the power of
the signal received from the adjacent cell is less
than a threshold value (i.e., the number of users
near  the  cell  edge  in  the  service  cell).    In  the
example shown in Figure 2, a comparison of the
received-power values from cells 0 and 1 indicates
a  user  count  at  the  cell  edge  of  2,  resulting  in
weight w
## 1
=2.  Now, the sub-band for which cell-
edge-band  metric A
k
is  smallest  is  considered
to  be  the  band  that  would  be  least  affected  by
interference  from  another  cell.    This  area  is
selected as the cell-edge band of the serving cell,
and the base stations of the adjacent cells are so
advised.  Repeating this process across all cells
enables the allocation of frequency bands to cell-
edge areas to be optimized over the system and
to be adjusted with changes in user distribution.
In short, calculating weights that take user
distribution into account and using these weights
in the allocation of cell-edge bands can minimize
interference  between  adjacent  cell  edges.    A
flowchart for the above sequence of operations is
shown in Figure 3.
w
## 1
## 2
## Cell 1
## Cell 2
## Cell 3
w
## 2
## 4
w
## 3
## 3
## Cell 0
## Adjacent
cell
## Adjacent
cell
## Adjacent
cell
Connected cell
## Figure 2
Example of determination of cell weights.
## Adjacent
base station
## Terminal
## Connected
base station
Measure receive power
Reference signalReference signal
Measured receive power
Calculate weights
Cell-edge band information
## Calculate
cell-edge band metric
## Determine
cell-edge band
Cell-edge band information
Receive data
Allocation information
Transmitted data
Perform scheduling
## Figure 3
Flowchart for interference-coordination method
considering user distribution.

## 93
FUJITSU Sci. Tech. J., Vol. 48, No. 1
(January
## 2012
## )
D. Kimura et al.: Inter-Cell Interference Coordination (ICIC) Technology
- Computer simulation
We  evaluated  the  effectiveness  of  the
proposed  ICIC  algorithm  on  the  downlink
by  computer  simulation.   Table  1  lists  the
simulation conditions.  These conditions conform
to the general conditions described in the 3GPP
specifications:  a  configuration  consisting  of  19
base stations and 3 cells per base station for a
total of 57 cells with 10 users per cell.
## 6)
Users are
distributed randomly within a cell, and shielding
effects  (shadowing)  due  to  topography  and
buildings are taken into account, resulting in a
model  in  which  considerable  variance  exists  in
the distribution of signal quality for users within
each cell.  In the simulation, four methods were
compared:
1)    no ICIC
2)    ICIC (fixed bands, frequency-reuse 3 at cell
edge)
3)    ICIC  (proposed  method,  frequency-reuse  3
at cell edge)
4)    ICIC  (proposed  method,  frequency-reuse  4
at cell edge).
Method  2,  using  ICIC  with  fixed  bands,
divides  the  total  system  bandwidth  into  three
sub-bands, each of which is allocated as a cell-
edge  band  to  one  of  the  three  cells  configured
by a base station, as shown in Figure 1(c).  This
method is considered to be optimal for cell-edge
band  allocation  provided  that  signal  quality
distribution  is  uniform.    The  proposed  method
was  simulated  for  two  cases:  three  sub-bands
and  four  sub-bands.    Increasing  the  number
of  sub-bands  can  increase  the  frequency-reuse
factor  at  the  cell  edge  and  therefore  improve
the  quality  of  reception  for  users  allocated  a
cell-edge  band,  but  since  this  also  narrows  the
bandwidth at the cell edge, throughput may drop.
Increasing the frequency-reuse factor also makes
it more difficult to determine optimal frequency
allocation.
The  simulation  results  are  listed  in
Table 2.  Cell-average throughput is the average
throughput  across  the  57  cells,  while  cell-edge
throughput is taken as the throughput that 95%
of the users can receive.  It can be seen that using
ICIC  improves  cell-edge  throughput  without
significantly decreasing cell-average throughput.
Furthermore,  for  three  sub-bands  (frequency-
reuse 3 at cell edge), cell-edge throughput with
the proposed method is about the same as with
ideal  allocation  using  the  conventional  FFR
method.  For four sub-bands (frequency-reuse 4
at cell edge), cell-edge throughput is significantly
improved (about 1.5 times compared to without
ICIC).    These  results  show  that  the  algorithm
proposed  here  can  automatically  allocate  the
most  appropriate  cell-edge  bands  regardless  of
the frequency-reuse number at the cell edge.
For  the  uplink  as  well,  the  automatic
coordination  of  cell-edge  bands  should  improve
throughput for cell-edge users in the same way.
## Table 1
Simulation conditions.
ItemDescription
Cell layout
19 base stations, 57 cells
(3 cells/base station)
Center frequency, bandwidth2 GHz, 5 MHz
Antenna configuration
2-transmit, 2-receive MIMO
(Multiple input multiple output)
Base-station transmit power 46 dBm
No. of users10 users/cell
Cell radius0.5 km
Fading frequency1–200 Hz
SchedulingProportional Fairness
## 7)

Traffic modelFull buffer
Path modelExtended Pedestrian A
## 8)
## Table 2
Simulation results.
## Method
## Throughput (kb/s)
Cell averageCell edge
No ICIC554386
ICIC (fixed bands, 3 sub-bands)5387121
ICIC (proposed method, 3 sub-bands)5551121
ICIC (proposed method, 4 sub-bands)5623131

## 94
FUJITSU Sci. Tech. J., Vol. 48, No. 1
(January
## 2012
## )
D. Kimura et al.: Inter-Cell Interference Coordination (ICIC) Technology
## Dai Kimura
## Fujitsu Laboratories Ltd.
Mr. Kimura is engaged in the research
and development of LTE systems for
both domestic and overseas markets.
## Hiroyuki Seki
## Fujitsu Laboratories Ltd.
Mr. Seki is engaged in the research and
development of next-generation cellular
systems and base station equipment.
## 6. Conclusion
This  paper  provided  an  overview  of  inter-
cell  interference  coordination  technology  for
use with the Long Term Evolution system and
presented  an  original  ICIC  algorithm  focusing
on  the  distribution  of  users  in  a  cell.    The
proposed  algorithm  enables  stable  interference
coordination  under  various  conditions  and
improves downlink throughput for users at cell
edges  by  about  1.5  times  compared  to  without
## ICIC.
As  the  future  spread  of  LTE  services
makes  mobile  broadband  a  reality,  improving
transmission  speed  at  cell  edges  will  become
a  pressing  problem.    We  intend  to  solve
this  problem  and  to  contribute  to  the  future
expansion of mobile communications systems by
applying our ICIC algorithm to LTE base station
equipment.
## References
1)   Requirements for Evolved UTRA (E-UTRA) and
Evolved UTRAN (E-UTRAN), 3GPP TR25.913.
## 2)   Evolved  Universal  Terrestrial  Radio  Access
Network  (E-UTRAN);  X2  application  protocol
## (X2AP), 3GPP TS36.423.
## 3)   Evolved  Universal  Terrestrial  Radio  Access
(E-UTRA);  Physical  layer  procedures,  3GPP
## TS36.213.
4)   Nortel:  Discussion  on  the  DL  Interference
Coordination.    3GPP  RAN,  WG1,  Meeting  #51,
Jeju, Korea, November 2007 (R1-074641).
5)   D. Kimura et al.: De-Centralized Dynamic ICIC
Using X2 Interfaces for Downlink LTE Systems.
## 73rd  Vehicular  Technology  Conference,  May
2011, pp. 1–5.
6)   Physical  layer  aspects  for  evolved  Universal
Terrestrial   Radio   Access   (UTRA),   3GPP
## TR25.814.
7)   C.  Wengerter  et  al.:  Fairness  and  throughput
analysis   for   generalized   proportional   fair
frequency  scheduling  in  OFDMA.    Vehicular
Technology  Conference,  Vol.  3,  pp.  1903–1907
## (2005).
## 8)   Evolved  Universal  Terrestrial  Radio  Access
(E-UTRA); Base Station (BS) radio transmission
and reception, 3GPP TS36.104.