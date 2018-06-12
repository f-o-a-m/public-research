# Clock Synchronization Literature Review
Vocabulary:

**Clock Drift**: in practice, the clock frequency varies unpredictably due to various physical effects, e.g., temperature and crystal aging. This is known as clock drifting. lower quality clocks, i.e., have a higher drift rate, that are more affordable. These clocks, however, need to be periodically resynchronized to account for their inherent drift and far more frequently than the atomic clocks.

**Resynchronization:** Due to inherent drift in local oscillators in the nodes, their clocks are bound to drift apart resulting in gradual degradation of synchrony, as a result, the nodes have to periodically resynchronize, referred to as the resynchronization process.

**Jitter:** Jitter is the timing variations of a set of signal edges from their ideal values. Jitters in clock signals are typically caused by noise or other disturbances in the system. Contributing factors include thermal noise, power supply variations, loading conditions, device noise, and interference coupled from nearby circuits. **Temporal** variations in consecutive clock edges • Mostly random

**skew: Spatial** variations in equivalent clock edges • Mostly deterministic. clock skew is the spatial variations of the arrival of the clock... it is due to delay in the clock path to various flops... it has serious effects on the design...like the setup and hold time violation... it is over come by using various routing techniques...a phenomenon in [synchronous](https://en.wikipedia.org/wiki/Synchronous_circuit) [digital circuit systems](https://en.wikipedia.org/wiki/Digital_electronics) in which the same sourced [clock signal](https://en.wikipedia.org/wiki/Clock_signal)arrives at different [components](https://en.wikipedia.org/wiki/Electronic_component) at different times i.e. the instantaneous difference between the readings of any two clocks is called their skew.


----------



      Malekpour, Mahyar R. "**A self-stabilizing Byzantine-fault-tolerant clock synchronization protocol.**" (2009).
      
      Malekpour, Mahyar. "**Achieving Agreement In Three Rounds With Bounded-Byzantine Faults.**" (2017).
      
      *******Malekpour, Mahyar R. “**An Autonomous Distributed Fault-Tolerant Local Positioning System**." (2017)

Malekpour has been working on this problem for over a decade, his most recent paper proposed two time synchronization algorithms that are Byzantine fault tolerant for wireless systems for local positioning. Highly recommended to read these three papers

    
    > We describe a **fault-tolerant, GPS-independent** (Global Positioning System) distributed autonomous positioning system for static/mobile objects and present solutions for providing highly-accurate geo-location data for the static/mobile objects in dynamic environments.
    
    > Existing distributed positioning systems either synchronize to a common external source like GPS or establish their own time synchrony using a scheme similar to a master-slave by designating a particular beacon as the master and other beacons synchronize to it, **resulting in a single point of failure.**
    
    > We solve this problem by first employing fault-tolerant distributed clock synchronization protocols to achieve the theoretical synchrony of one-clock tick across the distributed system of nodes (beacons) and, consequently, **determine the geometry of the network**, and then use **trilateration** to accurately determine the current location of the intended object.
    
    > **The geo-location and time-synchrony problems have a lot in common.**
    
    > prior knowledge of the exact locations of the beacons and their network geometry is not necessary; an autonomous distributed fault-tolerant local positioning system should be able to first determine its own geometry and then realign it to the world map…has to be able to autonomously and continually establish its time-synchrony and determine its geometry independent of an external source.
    
    > **The capability of a distributed network of beacons to autonomously self-synchronize and, subsequently, provide reliable signaling for proper geo- location, at the receivers and independent of GPS, is essential in reducing total reliance on an external source like GPS.**
    
    > We use the terms protocol and algorithm interchangeably. We also use the terms nodes and object generically as the protocols discussed in this paper are applicable to various applications. For geo-location applications, however, the terms nodes and object refer to beacons and vehicle (or target), respectively.


## More Notes: +An Autonomous Distributed Fault-Tolerant Local Positioning System 


----------


    Ramanathan, Parameswaran, Kang G. Shin, and Ricky W. Butler. **"Fault-tolerant clock synchronization in distributed systems."** *Computer* 23.10 (1990): 33-42.

An old and highly referenced piece of literature on the subject 


----------


    Djenouri, Djamel, and Miloud Bagaa. **"Synchronization protocols and implementation issues in wireless sensor networks: A review**." *IEEE Systems Journal* 10.2 (2016): 617-627.


    > Time synchronization in wireless sensor networks (WSNs) is a topic that has been attracting the research community in the last decade. Most performance evaluations of the proposed solutions have been limited to theoretical analysis and simulation. They consequently ignored several practical aspects, e.g., packet handling jitters, clock drifting, packet loss, and mote limitations, which affect real implementation on sensor motes.


    > **A taxonomy of the state-of-the-art implemented protocols has been given** before describing the protocols. Descriptions in this paper have been implementation centric, where the focus was on practical aspects related to the implementation and experimentation. Algorithmic description has been largely covered in the literature and is out of the scope of this paper.
    
----------
  
    Li, Chuanyou, Yun Wang, and Michel Hurfin. **"Clock synchronization in mobile Ad Hoc networks based on an iterative approximate byzantine consensus protocol."** *Advanced Information Networking and Applications (AINA), 2014 IEEE 28th International Conference on*. IEEE, 2014.

Appears to be a different approach than Malekpour, but noted that the focus is solely on time not location 


    > The clock synchronization strategy proposed in this paper is based on a solution to the approximate consensus problem
    > Our work is rather inspired by fault-tolerant techniques: we do not try to identify the malicious nodes but we synchronize the clocks in spite of them.


----------
    Medani, Khedidja, Makhlouf Aliouat, and Zibouda Aliouat**. "Fault tolerant time synchronization using offsets table robust broadcasting protocol for vehicular ad hoc networks."** *AEU-International Journal of Electronics and Communications* 81 (2017): 192-204


    > we propose “Offsets Table Robust Broadcasting” (OTRB) algorithm. In this algorithm, instead to each node communicates with its vicinity, a set of nodes is selected to spread the time information over the entire network. The proposed time synchronization protocol is well-adapted to random network topology changes, high nodal velocity while offering good precision and robustness against nodal failure and packet loss.

This paper includes a good overview of some time synchronization protocols. We should look a bit more into their proposed algorithm, but it seems to be focused only on moving nodes. 


----------
    Hussein, Sherif, Axel Krings, and Azad Azadmanesh. "**VANET clock synchronization for resilient DSRC safety applications**." *Resilience Week (RWS), 2017*. IEEE, 2017.


    > might be subjected to malicious attacks, s**uch as GPS time spoofing attacks, which attempt to prevent time synchronization between vehicles. Failure of the centralized GPS-based clock synchronization has the potential to cause safety applications to fail. Therefore, decentralized clock synchronization can be a valuable approach for augmenting GPS- based clock synchronization.**


    > 
----------
    Kinali, Attila, Florian Huemer, and Christoph Lenzen. **"Fault-tolerant Clock Synchronization with High Precision."** *VLSI (ISVLSI), 2016 IEEE Computer Society Annual Symposium on*. IEEE, 2016.


    > We present the first FPGA implementation of a distributed clock synchronization algorithm with sub-nanosecond skews that can tolerate arbitrary faults of individual components. Each of n nodes is equipped with its own quartz oscillator and the nodes broadcast their clock pulses to enable synchronization

Their algorithm seems specific to the oscillator type, so it may be hardware specific, lets investigate further. 

----------
    Tröger, Hans-Martin, et al. **"Synchronization of wireless sensor networks utilizing broadcast signal time stamps."** *Communications Workshops (ICC Workshops), 2017 IEEE International Conference on*. IEEE, 2017


    > The synchronization of wireless sensor networks is a crucial task, especially for wide area networks. In case of many applications state-of-the-art techniques such as GPS or network based timing protocols are not suitable. In this paper we present a new concept that allows for the efficient synchronization of sensor networks using the time stamps of so- called Signals of Opportunity.


----------





