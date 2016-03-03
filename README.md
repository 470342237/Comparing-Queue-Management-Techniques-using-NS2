# Comparing-Queue-Management-Techniques-using-NS2
Simulation of two Queue Management techniques – Tail Drop and RED, for a mesh network. The results obtained are analysed over 3 parameters: Throughput, End-2-End delay and Packet Loss/Drop.
The goal of the simulations performed using NS2, is to determine which Queueing mechanism, Taildrop or RED, is better for managing queues and thereby more effective for Congestion Control. These two mechanism are tried on a single network scheme and are compared on the basis of various performance parameters. RED came out as a queue management technique with the target to outperform the performance of Tail Drop.

**Schematic of the network simulated**
A Mesh network with 3 wireless nodes, 3 static and 3 mobile nodes.

**Description of the different flows/packets/protocols**
Routing protocol : AODV
Interface queue type : Droptail and RED
End to end link specs: 2Mb 10ms and 1.7Mb 20ms
End to End protocol: TCP and UDP

**Varying parameters**
- Congestion control protocol (Taildrop/RED)
- Sent Data Rate
- Packet size

For Observations, refer to the observation directory in the repository.
Overall Simulation Information:

**Drop Tail**
Simulation length in seconds: 9.77363029
Number of nodes: 7
Number of sending nodes: 7
Number of receiving nodes: 4
Number of generated packets: 640
Number of sent packets: 316
Number of forwarded packets: 289
Number of dropped packets: 326
Number of lost packets: 4
Minimal packet size: 32
Maximal packet size: 1040
Average packet size: 870.7948
Number of sent bytes: 246072
Number of forwarded bytes: 244808
Number of dropped bytes: 330808
Packets dropping nodes: 0  1  2  5

**RED**
Simulation length in seconds: 5.321942771
Number of nodes: 7
Number of sending nodes: 7
Number of receiving nodes: 4
Number of generated packets: 619
Number of sent packets: 285
Number of forwarded packets: 266
Number of dropped packets: 336
Number of lost packets: 1
Minimal packet size: 40
Maximal packet size: 1040
Average packet size: 875.2949
Number of sent bytes: 223204
Number of forwarded bytes: 222304
Number of dropped bytes: 339796
Packets dropping nodes: 0  1  2

**Results**
Results for the observed parameters as per our simulation are following:
- Throughput analysis: As we can see from the fig. (iii) and fig. (iv), throughput of both the protocols are almost the same. But RED seems to have a slight advantage over Tail Drop protocol.
- Packet Loss: From the overall simulation information, it is clear that Drop Tail suffered from the loss of 4 packets while RED suffered from the loss of just 1 packet.
- End to End Delay: From the fig. (i) belonging to Tail Drop and fig. (ii) belonging to RED, it is clear that the avg. delay time for data in case of RED is less than Tail Drop. So, RED seems to perform better in case of E2E delay as well.

**Conclusion**
Results shows that RED performs better than Tail Drop maintaining a low packet drop and higher throughput also maintaining a high packet delivery ratio(as clear from the overall information).
