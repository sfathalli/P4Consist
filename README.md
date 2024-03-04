**P4Consist: Toward Consistent P4 SDNs**

This is the main repository of the paper [**P4CONSIST**: Towards Consistent P4 SDNs](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9109655), published at the [IEEE Journal on Selected Areas in Communications](https://ieeexplore.ieee.org/xpl/tocresult.jsp?isnumber=9127210&punumber=49) (Volume: 38 Issue: 7).

Software-defined networking (SDN) functions on the principle that a centrally controlled system accurately reflects the current state of the network's data flow. However, issues such as bugs, misconfigurations, faults, or malicious attacks can lead to disparities between the control plane's directives and the actual behavior of the data plane, disrupting network operations.

In response to this challenge, we introduce P4Consist, a solution designed to identify inconsistencies between the control and data planes in P4-based SDNs. 
The tool employs active probe-based traffic generation, either continuously or periodically, to assess whether the data plane's actions align with the intended behavior dictated by the control plane. It collects separate reports from the control and data planes, which are then systematically compared to ensure alignment and detect any discrepancies.

P4Consist utilizes symbolic execution and graph traversal techniques to simulate packet forwarding throughout the control plane configuration. The data plane takes advantage of the Inband-Network Telemetry (INT), to collect telemetry data in real-time during network traversal.