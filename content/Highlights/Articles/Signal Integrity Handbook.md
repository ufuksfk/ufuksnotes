---
draft: true
description:
socialDescription:
title: Signal Integrity Handbook
tags:
  - highlight/articles
date: 2025-06-21
modified: 2025-08-21
---
author: [[eecosystem]]
url: https://www.theeecosystem.com/_files/ugd/3fb2d5_20dcd56d730d4fc9a321971c6ad36256.pdf
last highlighted date: [[2025-06#17]]

[[Signal Integrity]]
## Highlights
- Figure 2. In differential signaling, because the two signals propagate 180 degrees out of phase, they are resistant to the influence of noise, and the signal at the receiver matches the one from the sender.
- As Nyquist frequency increases to a higher data rate, loss and reflection become a challenge. A shift to four-level signaling (pulse amplitude modulation 4-level; PAM4) encodes data in the amplitude and doubles the data rate for signals operating at the same Nyquist frequency as PAM2.
- Each of the four voltage levels corresponds to one of four bit-sequences (00, 01, 10, 11), providing two bits on the space previously occupied by one, yet not increasing operating frequency.
- Unfortunately, PAM4 signaling is more sensitive to noise sources such as reflection and crosstalk (see Figure 3). This is due to the reduced signal amplitude (1/3 of NRZ), effectively reducing the signal-to-noise ratio. The highest speed standards operating at NRZ/PAM2 are 28 and 32 Gbps. Above this data rate, PAM4 is typically used, beginning at 56 and 64 Gbps and beyond.
- insertion loss (IL). In a two-port device under test (DUT), insertion loss is the magnitude of S21 in an S-parameter matrix and expressed in dB, where the nomenclature "21" (expressed as "two-one") refers to the signal observed at port 2 when stimulated at port 1.
- Insertion loss is expressed as a negative number for attenuation and as a positive number for gain. It is expressed in dB as the ratio of output to input.
- There are two types of crosstalk of concern in high-speed systems, near-end crosstalk (NEXT) and far-end crosstalk (FEXT) (see Figure 8). NEXT is the measure of crosstalk coupling from transmitting (Tx) lanes onto nearby receiving (Rx) lanes. NEXT is most critical when coupling sources (vias, connectors, etc.) occur near the transmitting source (where Tx signal levels are the highest and the Rx signal levels are the smallest).
  FEXT relates to signals traveling in the same direction. For example, FEXT is the noise that a transmitting lane experiences from other transmitting lanes. It is generally viewed in the context of the length and loss of the channel. With FEXT, both the crosstalk levels and signal levels are attenuating together before reaching the receiver.
- Another way of characterizing the effects of impedance mismatch in the frequency domain is voltage standing wave ratio (VSWR; pronounced “viz-wer”). Impedance discontinuities within a terminated cable connector and/or terminated PCB connector (terminated connector system) will cause partial reflections of a traveling wave.
- Impedance (Ω) is a measure of the behavior of the interconnect. It is influenced by signal conductor and reference conductor surface area, the gap between them, and the dielectric property of whatever is between them (air, plastic, etc). Impedance is a function of inductance and capacitance, and is highly influenced by conductor surface area. The impedance value affects return loss.
- At slow rise times, the device will appear to have an impedance value close to the reference or system impedance. But as rise times decrease (in other words, as edge rates get faster), the measured impedance values begin to move toward the true characteristic impedance of the component. At an infinitely short rise time, we would measure the true characteristic impedance of a device.
- Figure 12: Various simulation tools enable electrical model characterization, including 2.5D wave EM solvers (top left), 3D field solvers (top right), and system analysis tools (bottom)
