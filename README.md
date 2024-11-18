Network Simulation: Go-Back-N Method

Overview

This project demonstrates a basic network simulation where one device sends data packets to another using the Go-Back-N ARQ (Automatic Repeat Request) protocol. It showcases how packet transmission, acknowledgment, and retransmission work in a simulated network environment.

Features

Simulated Packet Transmission: Data packets are sent from a sender to a receiver in sequence.
Go-Back-N Protocol: Enables sending multiple packets at a time without waiting for individual acknowledgments.
Error Handling: Lost or delayed packets trigger a timer, prompting the sender to retransmit the required packets.
Multithreading: Sending and receiving processes run concurrently, emulating real-world network behavior.
How to Use

Open the Notebook
Access the project via the Google Colab link.
View Outputs
You can directly view the results and outputs within the notebook without requiring additional setup.
Technical Explanation

The Go-Back-N method allows the sender to send multiple packets simultaneously without waiting for individual acknowledgments. If an issue occurs (e.g., a lost or delayed packet), the following steps are executed:

Timer Activation: A timer detects errors or delays in acknowledgment.
Retransmission: The sender retransmits the required packets starting from the erroneous packet.
Concurrent Processing: Threads handle the sending and receiving processes simultaneously, similar to how separate processes operate in real networks.
This simulation provides an understanding of how network protocols manage data reliability and efficiency.

Requirements

Google Colab (no local installation required).
