# Green_Video_Control_Plane
Simulator used for submission to ITC 29

The main files to launch are in the srv_submissions folder, and start with srv_submission_* .

Motivation for our simulator choice:

In our concern of reproducible research, we have investigated the possible tools to make a simulator. In the ICN realm specifically, several tools are available (ccnSim, etc.) [1]. It however appears that constraining a client to be served by a
single source does not match the CCN concept where routing is content-based and not src/dst based. ICN simulators are therefore not adapted for our strategy based on a fine SDN control with continuous encoding (iProxy). Implementation in an SDN testbed or within a simulator such as ns-3 will require a cross-layer management, from optical up to DC. It would thus require deep modifications to available simulators. In order to get a first assessment, we therefore create a Matlab discrete-event simulator. However to consider reproducible research standards, we make our simulator publicly available
at here and are planning a full deployment within ns-3.

[1] M. Tortelli, D. Rossi, G. Boggia, L.A. Grieco, "ICN software tools: Survey and cross-comparison", Elsevier Simulation Modelling Practice and Theory, no. 63, pp. 23-46, 2016.


