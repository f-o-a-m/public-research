# Clock Synchronization Literature Review^[[_add new research as noted in the style guidelines in the appendix._]()]
## FOAM Protocol Research links

## Vocabulary:

**Clock Drift**: in practice, the clock frequency varies unpredictably due to various physical effects, e.g., temperature and crystal aging. This is known as clock drifting. lower quality clocks, i.e., have a higher drift rate, that are more affordable. These clocks, however, need to be periodically resynchronized to account for their inherent drift and far more frequently than the atomic clocks.

**Resynchronization:** Due to inherent drift in local oscillators in the nodes, their clocks are bound to drift apart resulting in gradual degradation of synchrony, as a result, the nodes have to periodically resynchronize, referred to as the resynchronization process.

**Jitter:** Jitter is the timing variations of a set of signal edges from their ideal values. Jitters in clock signals are typically caused by noise or other disturbances in the system. Contributing factors include thermal noise, power supply variations, loading conditions, device noise, and interference coupled from nearby circuits. **Temporal** variations in consecutive clock edges • Mostly random

**skew: Spatial** variations in equivalent clock edges • Mostly deterministic. clock skew is the spatial variations of the arrival of the clock... it is due to delay in the clock path to various flops... it has serious effects on the design...like the setup and hold time violation... it is over come by using various routing techniques...a phenomenon in [synchronous](https://en.wikipedia.org/wiki/Synchronous_circuit) [digital circuit systems](https://en.wikipedia.org/wiki/Digital_electronics) in which the same sourced [clock signal](https://en.wikipedia.org/wiki/Clock_signal)arrives at different [components](https://en.wikipedia.org/wiki/Electronic_component) at different times i.e. the instantaneous difference between the readings of any two clocks is called their skew.

\clearpage

## Clock Synchronization Techniques for Distributed Systems^[[NASA Technology Transfer Program
](https://www.youtube.com/watch?v=oyXsiE9CuK8)]
_Mahyar R. Malekpour_

> Mahyar R. Malekpour introduces Agile Local Positioning System (ALPS) an autonomous distributed fault-tolerant local positioning system, in a NASA video.

## An Autonomous Distributed Fault-Tolerant Local Positioning System^[[AIAA SciTech 2018](https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20170007192.pdf)]
_Mahyar R. Malekpour_

> We describe a fault-tolerant, GPS-independent (Global Positioning System) distributed autonomous positioning system for static/mobile objects and present solutions for providing highly-accurate geo-location data for the static/mobile objects in dynamic environments. The reliability and accuracy of a positioning system fundamentally depends on two factors; its timeliness in broadcasting signals and the knowledge of its geometry, i.e., locations and distances of the beacons. 

## A Byzantine-fault tolerant self-stabilizing protocol for distributed clock synchronization systems^[[SSS'06 Proceedings of the 8th international conference on Stabilization, safety, and security of distributed systems Pages 411-427](https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20070000531.pdf)]
_Mahyar R. Malekpour_

> Embedded distributed systems have become an integral part of safety-critical computing applications, necessitating system designs that incorporate fault tolerant clock synchronization in order to achieve ultra-reliable assurance levels. Many efficient clock synchronization protocols do not, however, address Byzantine failures, and most protocols that do tolerate Byzantine failures do not self-stabilize. Of the Byzantine self-stabilizing clock synchronization algorithms that exist in the literature, they are based on either unjustifiably strong assumptions about initial synchrony of the nodes or on the existence of a common pulse at the nodes. The Byzantine self-stabilizing clock synchronization protocol presented here does not rely on any assumptions about the initial state of the clocks.

## Achieving Agreement In Three Rounds With Bounded-Byzantine Faults^[[AIAA Information Systems-AIAA Infotech @ Aerospace](https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20150017047.pdf)]
_Mahyar R. Malekpour_

FOAM Note: _Malekpour has been working on this problem for over a decade, his most recent paper proposed two time synchronization algorithms that are Byzantine fault tolerant for wireless systems for local positioning. Highly recommended to read these three papers._

 
 > We describe a **fault-tolerant, GPS-independent** (Global Positioning System) distributed autonomous positioning system for static/mobile objects and present solutions for providing highly-accurate geo-location data for the static/mobile objects in dynamic environments.
 
 > Existing distributed positioning systems either synchronize to a common external source like GPS or establish their own time synchrony using a scheme similar to a master-slave by designating a particular beacon as the master and other beacons synchronize to it, **resulting in a single point of failure.**
 
 > We solve this problem by first employing fault-tolerant distributed clock synchronization protocols to achieve the theoretical synchrony of one-clock tick across the distributed system of nodes (beacons) and, consequently, **determine the geometry of the network**, and then use **trilateration** to accurately determine the current location of the intended object.
 
 > **The geo-location and time-synchrony problems have a lot in common.**
 
 > prior knowledge of the exact locations of the beacons and their network geometry is not necessary; an autonomous distributed fault-tolerant local positioning system should be able to first determine its own geometry and then realign it to the world map…has to be able to autonomously and continually establish its time-synchrony and determine its geometry independent of an external source.
 
 > **The capability of a distributed network of beacons to autonomously self-synchronize and, subsequently, provide reliable signaling for proper geo-location, at the receivers and independent of GPS, is essential in reducing total reliance on an external source like GPS.**
 
 > We use the terms protocol and algorithm interchangeably. We also use the terms nodes and object generically as the protocols discussed in this paper are applicable to various applications. For geo-location applications, however, the terms nodes and object refer to beacons and vehicle (or target), respectively.

## List of Mahyar R. Malekpour Publications^[[shemesh.larc.nasa.gov](https://shemesh.larc.nasa.gov/people/mrm/publications.htm)]
_Mahyar R. Malekpour_

> The contents herein are mine and do not necessarily reflect the positions of my employer.
Last Updated: Sometime June 2018

\clearpage

## More Notes: +An Autonomous Distributed Fault-Tolerant Local Positioning System 

## Fault-tolerant clock synchronization in distributed systems^[[Computer ( Volume: 23 , Issue: 10 , Oct. 1990 )](https://ieeexplore.ieee.org/document/58235)]
_P. Ramanathan, K.G. Shin, R.W. Butler_

> Existing fault-tolerant clock synchronization algorithms are compared and contrasted. These include the following: software synchronization algorithms, such as convergence-averaging, convergence-nonaveraging, and consistency algorithms, as well as probabilistic synchronization; hardware synchronization algorithms; and hybrid synchronization. 

FOAM Note: _An old and highly referenced piece of literature on the subject._

## Synchronization Protocols and Implementation Issues in Wireless Sensor Networks: A Review^[[IEEE Systems Journal ( Volume: 10 , Issue: 2 , June 2016 )](https://ieeexplore.ieee.org/document/6922482)]
_Djenouri, Djamel, and Miloud Bagaa_

> Time synchronization in wireless sensor networks (WSNs) is a topic that has been attracting the research community in the last decade. Most performance evaluations of the proposed solutions have been limited to theoretical analysis and simulation. They consequently ignored several practical aspects, e.g., packet handling jitters, clock drifting, packet loss, and mote limitations, which affect real implementation on sensor motes.


> **A taxonomy of the state-of-the-art implemented protocols has been given** before describing the protocols. Descriptions in this paper have been implementation centric, where the focus was on practical aspects related to the implementation and experimentation. Algorithmic description has been largely covered in the literature and is out of the scope of this paper.
 

## Clock Synchronization in Mobile Ad Hoc Networks Based on an Iterative Approximate Byzantine Consensus Protocol^[[2014 IEEE 28th International Conference on Advanced Information Networking and Applications](https://ieeexplore.ieee.org/document/6838667)]
_Chuanyou Li, Yun Wang, Michel Hurfin_

> We consider the clock synchronization problem in wireless mobile ad hoc networks in the presence of Byzantine nodes. The communication topology is dynamic: nodes move randomly within a geographical area. We propose a clock synchronization protocol which is based on the linear approximate consensus method. Periodically each correct node broadcasts its current timestamp and gathers the timestamps provided by its current neighbors. To cope with the malicious nodes (and to improve the performance when the node density is low), each node keeps the collected timestamps in a local log.

> The clock synchronization strategy proposed in this paper is based on a solution to the approximate consensus problem.

> Our work is rather inspired by fault-tolerant techniques: we do not try to identify the malicious nodes but we synchronize the clocks in spite of them.

FOAM Note: _Appears to be a different approach than Malekpour, but noted that the focus is solely on time not location._

## Fault tolerant time synchronization using offsets table robust broadcasting protocol for vehicular ad hoc networks^[[AEU - International Journal of Electronics and Communications Volume 81, November 2017, Pages 192-204](https://www.sciencedirect.com/science/article/pii/S143484111730256X)]
_Khedidja Medani, Makhlouf Aliouat, Zibouda Aliouat_

> The requirement of time synchronization emerged in distributed systems remains one of the most significant issues that should be addressed to the extent of that systems evolve. As clock synchronization is important for any type of network, Vehicular Ad hoc networks (VANETs) are being considered for their basic communication platforms, but also for providing the ability to detect movement, location, proximity, and other network capabilities.
additional comments as needed.

> We propose “Offsets Table Robust Broadcasting” (OTRB) algorithm. In this algorithm, instead to each node communicates with its vicinity, a set of nodes is selected to spread the time information over the entire network. The proposed time synchronization protocol is well-adapted to random network topology changes, high nodal velocity while offering good precision and robustness against nodal failure and packet loss.

FOAM Note: _This paper includes a good overview of some time synchronization protocols. We should look a bit more into their proposed algorithm, but it seems to be focused only on moving nodes._


## VANET clock synchronization for resilient DSRC safety applications^[[2017 Resilience Week (RWS)](https://ieeexplore.ieee.org/document/8088648)]
_Sherif Hussein, Axel Krings, Azad Azadmanesh_

> Vehicular Ad Hoc Networks (VANET) are the fastchanging networks for connected vehicles, in which Vehicle- to-Vehicle and Vehicle-to-Infrastructure communication are the basis for technologies aiming at reducing accidents and improving operation. DSRC Safety Applications, **designed to assist drivers in order to avoid accidents, might be subjected to malicious attacks, such as GPS time spoofing attacks, which attempt to prevent time synchronization between vehicles.**


## Fault-Tolerant Clock Synchronization with High Precision^[[2016 IEEE Computer Society Annual Symposium on VLSI (ISVLSI)](https://ieeexplore.ieee.org/document/7560246)]
_Attila Kinali, Florian Huemer, Christoph Lenzen_

> We present the first FPGA implementation of a distributed clock synchronization algorithm with sub-nanosecond skews that can tolerate arbitrary faults of individual components. Each of n nodes is equipped with its own quartz oscillator and the nodes broadcast their clock pulses to enable synchronization. The algorithm provably maintains synchronization even if fewer than n/3 nodes exhibit arbitrary faulty behavior. 

FOAM Note: _Their algorithm seems specific to the oscillator type, so it may be hardware specific, lets investigate further._ 

## Synchronization of wireless sensor networks utilizing broadcast signal time stamps^[[2017 IEEE International Conference on Communications Workshops (ICC Workshops)](https://ieeexplore.ieee.org/document/7962831)]
_Hans-Martin Tröger, Florian Schmittner, Thorsten Nowak, Joerg Robert, Albert Heuberger_

> The synchronization of wireless sensor networks is a crucial task, especially for wide area networks. In case of many applications state-of-the-art techniques such as GPS or network based timing protocols are not suitable. In this paper we present a new concept that allows for the efficient synchronization of sensor networks using the time stamps of so-called Signals of Opportunity.

\clearpage

# Appendix

The following format may be used for referencing papers:

```
## title^[[published_location](url)]
_authors_

> Excerpt or abstract here.

FOAM Note: _additional comments as needed for relevance to FOAM._

```

# Make instructions for this document

Pandoc is a cross-platform application used for converting documents to other formats. The following will generate the pdf version of this document. Markdown is used for consistency, and ease of assembly.

```pandoc 'Clock-Synchronization-Literature-Review.md' --pdf-engine=xelatex -o 'Clock-Synchronization-Literature-Review.pdf'
```

# Glossary
> Words and their definitions should be included here alphabetically. Definitely include any domain specific words here, generic technical words may be included if this will improve readability of the document. Try to be succinct where possible.


## Attenuation
> the reduction of the amplitude of a signal, electric current, or other oscillation.

## Distance bounding
> are cryptographic protocols that enable a verifier V to establish an upper bound on the physical distance to a prover P. They are based on timing the delay between sending out challenge bits and receiving back the corresponding response bits. 

## GPS
> The Global Positioning System (GPS), originally Navstar GPS, is a satellite-based radio navigation system owned by the United States government and operated by the United States Air Force.

## LoRa
> LoRa (Long Range) is a patented digital wireless data communication technology developed by Cycleo of Grenoble, France, and acquired by Semtech in 2012.

## LoRaWAN
> LoRaWAN is the network on which LoRa operates, and can be used by IoT for remote and unconnected industries. LoRaWAN is a media access control (MAC) layer protocol but mainly is a network layer protocol for managing communication between LPWAN gateways and end-node devices as a routing protocol, maintained by the LoRa Alliance. Version 1.0 of the LoRaWAN specification was released in June 2015.[5] In basic terms, one can consider LoRaWAN to be a new WiFi to connect new IoT devices across every industry.

## LPWAN
> A low-power wide-area network (LPWAN) or low-power wide-area (LPWA) network or low-power network (LPN) is a type of wireless telecommunication wide area network designed to allow long range communications at a low bit rate among things (connected objects), such as sensors operated on a battery.

## Multilateration (MLAT) 
> is the measurement of the difference in distance to two stations at known locations by broadcast signals at known times.

## Wi-Fi
> Wi-Fi is technology for radio wireless local area networking of devices based on the IEEE 802.11 standards. Wi‑Fi is a trademark of the Wi-Fi Alliance, which restricts the use of the term Wi-Fi Certified to products that successfully complete interoperability certification testing.





