# “From Waves to Packets: A Mini-Study of Signal Processing in Computer Networks”

**Goal:** show how physical signal principles (sampling, reflections, aliasing) map into network phenomena (collisions, ARP broadcasts, TCP handshake delays).

## Abstract
This project bridges physical signal processing with data communication protocols, showing how wave properties (aliasing, reflections, noise) map to network behavior (collisions, ARP, TCP timing).

## Objectives
- Demonstrate Nyquist–Shannon theorem and anti-alias filtering.
- Simulate transmission line reflections.
- Capture ARP broadcasts/unicasts.
- Model CSMA/CD collision handling.
- Analyze TCP 3-way handshake timing.
- Visualize application-layer packet scope.

## Method
- Tools: Python (NumPy, SciPy, matplotlib, pyshark), Wireshark.
- Data: synthetic waveforms + packet captures.
- Approach: each exercise documented in Jupyter notebooks.

## Results (per notebook)
- **NyquistLab:** alias observed at 500 Hz, suppressed −30 dB after LPF.
- **WireScope:** open load reflection Γ=+1, standing waves observed.
- **ARP:** local ping → target MAC; remote ping → gateway MAC.
- **CSMA/CD:** throughput peaked at ~0.36 channel capacity (matches theory).
- **TCP:** RTT ~22 ms, detected retransmit when ACK lost.
- **App Scope Map:** clear differences in packet visibility.

## Discussion
- How physical constraints limit network layers.
- Comparison between theory and experimental captures.
- Reflections on lab feasibility for EASV curriculum.

## Conclusion
Signal processing is not abstract—it shapes the limits of digital communication, from aliasing in sampling to congestion in Ethernet.

---
