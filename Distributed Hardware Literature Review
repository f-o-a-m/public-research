# Distributed Hardware Literature Review  


   Raza, Usman, Parag Kulkarni, and Mahesh Sooriyabandara. **"Low power wide area networks: An overview."** *IEEE Communications Surveys & Tutorials* 19.2 (2017)

-**Low Power Wide Area Network (LPWAN)**


   > This review paper presents the design goals and the techniques, which differ- ent LPWA technologies exploit to offer wide-area coverage to low- power devices at the expense of low data rates. We survey several emerging LPWA technologies and the standardization activities carried out by different standards development organizations 


   > The success of LPWA technologies lies in their ability to offer low-power connectivity to massive number of devices distributed over large geographical areas at an unprecedented low-cost. This section describes the techniques LPWA tech- nologies used to achieve these often conflicting goals.

Properties of LPWAN:
-Long Range 
-Ultra low power operation
-Low Cost
-Scalability 

*****This paper has great technical comparison charts between the different chip types.*** 

----------


   Lavric, Alexandru, and Valentin Popa. "**LoRa Wide-Area Networks from an Internet of Things Perspective**. 


   > The main contribution of the paper is the performance evaluation of the LoRa technology considering the requirements of IoT. In the first part of this paper LoRa technology is summarized by reviewing some aspects regarding the architecture and the security of the technology, meanwhile in the second part of the paper are presented some simulation scenarios.


----------


   Adelantado, Ferran, et al. “**Understanding the limits of LoRaWAN**." *IEEE Communications Magazine* 55.9 (2017): 34-40.


----------


   Krizman, Kevin J., Thomas E. Biedka, and Theodore S. Rappaport. “**Wireless position location: fundamentals, implementation strategies, and sources of error.**" *Vehicular Technology Conference, 1997, IEEE 47th*. Vol. 2. IEEE, 1997.

Appears to be a canonical paper on the subject


----------


   Fargas, Bernat Carbonés, and Martin Nordal Petersen. "**GPS-free geolocation using LoRa in low-power WANs**." *Global Internet of Things Summit (GIoTS), 2017*. IEEE, 2017


   > This paper reports on a design and implementation of a LoRaWAN tracking system which is capable exploiting transmitted packages to calculate the current position **without the use of GPS or GSM. This is done using the low power technology LoRa where the geolocation is calculated applying a multilateration algorithm on the gateways timestamps from received packages.**

Uses LoRa for location without GPS using multilateration. 


   > The three most common methods used for performing the geolocation are **triangulation**, **trilateration** and **multilateration**.


   > **Triangulation** uses angles of incidence of the signal received from the transmitter. A triangle is defined with two of them and the end-node position is estimated applying trigonometric formulas.


   > **Trilateration** requires the distance between the transmitter and the receiver, which can be obtained from the time of arrival (TOA), the time of flight (TOF) or from the received signal strength indicator (RSSI). Therefore, it requires synchronization between the transmitter and the receiver. The position is the intersection of the three circles obtained from the different distances.


   > **Multilateration** is quite similar to trilateration; however, the main feature to compute the location is the time difference of arrival (TDOA). The transmitters are synchronized to each other, whereas the receiver does not need to be. Thus, the location in this technique is the intersection of at least two hyperbolas (three antennas required).


----------


   Sastry, Naveen, Umesh Shankar, and David Wagner. "**Secure verification of location claims.**" *Proceedings of the 2nd ACM workshop on Wireless security*. ACM, 2003.

Appears to be canonical. Need to closely revisit.


----------


   Chen, Liang, et al. "**Robustness, Security and Privacy in Location-Based Services for Future IoT: A Survey**." *IEEE Access* (2017).


   > Security and privacy threats related to positioning in IoT have not been sufficiently addressed so far. In this paper, we survey solutions for improving the robustness, security and privacy of location-based services in IoT systems. First, we provide an in- depth evaluation of the threats and solutions related to both Global Navigation Satellite System (GNSS) and non-GNSS based solutions. Secondly, we describe certain cryptographic solutions for security and privacy of positioning and location-based services in IoT.

*Has Block diagram of GNSS threats to IoT positioning

*NON-GNSS BASED LOCALIZATION TECHNOLOGIES AND THEIR SECURITY THREATS

*SUMMARY OF STANDARD CRYPTOGRAPHY FOR LOCATION INFORMATION

*Distance-bounding and secure localization*

good attack vectors here 


----------
    Capkun, Srdjan, and J-P. Hubaux. "**Secure positioning of wireless devices with application to sensor networks**." *INFOCOM 2005. 24th Annual Joint Conference of the IEEE Computer and Communications Societies. Proceedings IEEE*. Vol. 3. IEEE, 2005
    
   Capkun, Srdjan, and J-P. Hubaux. "**Secure positioning in wireless networks.**" *IEEE Journal on Selected Areas in Communications* 24.2 (2006): 221-232

These papers show an enormous amount of attack vectors, must revisit. Distance estimation v distance bounding? 


   > Verifiable Multilateration can also be performed with authenticated **distance estimation, instead of distance bounding.**


   > **If the nodes are tightly synchronized**, they can measure the signal time of flight to estimate their **mutual distance**. In the packets they send, nodes include timestamps of the times at which they sent the packets. Upon receiving a packet, each node registers the packet reception time, and estimates the distance based on the difference between the sending and the reception time.


----------

   Zeng, Yingpei, et al. "**Secure localization and location verification in wireless sensor networks: a survey.**" *The Journal of Supercomputing* (2013): 1-17.

Excellent survey, need to revisit. 


   > In this paper, we present a survey of current work on both secure localization and location verification. We first describe the attacks against localization and location verification, and then we clas- sify and describe existing solutions. We also implement typical secure localization algorithms of one popular category and study their performance by simulations.


   > **secure localization**=sensors themselves need to get their correct locations 
   > **location verification**=sensor nodes may be compromised and they may intentionally report false locations to the base. Thus, we need to verify the locations learnt from sensors. 


   > So for secure localization, it can be measured by received signal strength indicator (RSSI), time of arrival (ToA), or time difference of arrival (TDoA) 
    > 
    > For location verification, most of the solutions are about In-region solutions that try to verify that whether nodes (i.e., provers) are in- side given regions. 
    > These all use distance bounding protocols 

***Without synchronization can not get full geometry of network, why exactly though? Only one way?** 


----------


   Zhang, Pengfei, Sai Ganesh Nagarajan, and Ido Nevat. "**Secure Location of Things (SLOT): Mitigating Localization Spoofing Attacks in the Internet of Things.**" *IEEE Internet of Things Journal* (2017).


   > In this paper we developed new algorithms for Geo- Spatial tagging in the Internet of Things (IoT), which are robust against malicious attacks.

The algorithms developed here are for Ultra-Wideband (UWB) tech, not sure if they are applicable to LPWAN


----------

There is literature on Distance Bounding protocols, need to read more closely:


   Singelee, Dave, and Bart Preneel. "**Location verification using secure distance bounding protocols**." *Mobile Adhoc and Sensor Systems Conference, 2005. IEEE International Conference on*. IEEE, 2005


   Abu-Mahfouz, Adnan, and Gerhard P. Hancke. "**Distance bounding: A practical security solution for real-time location systems**." *IEEE transactions on industrial informatics* 9.1 (2013): 16-27
    


   > There are however some practical problems which limit the use of such protocols. There are three major attack scenarios: **distance fraud attacks, mafia fraud attacks and terrorist fraud attacks**


----------

Wifi Location


   Kotaru, Manikanta, et al. "**Spotfi: Decimeter level localization using wifi**." *ACM SIGCOMM Computer Communication Review*. Vol. 45. No. 4. ACM, 2015.
    
   Javali, Chitra, et al. **"I Am Alice, I Was in Wonderland: Secure Location Proof Generation and Verification Protocol."** *Local Computer Networks (LCN), 2016 IEEE 41st Conference on*. IEEE, 2016.

