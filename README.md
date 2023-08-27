![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/126003fa-8094-4cc5-a040-d65d24c08f68)# Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System
In this repository, we delve into the implementation of narrowband and wideband channels. In the narrowband channel section, we implement the narrowband channel and by examining various modulations, we aim to reduce the error probability based on SNR. In another section, by designing an OFDM system, we are seeking to implement a wideband channel.

The purpose of performing this exercise is to become familiar with the effects of a channel on the received signal (fade effect) at the receiver and its impact on the system's error probability. To this end, various solutions used to mitigate these effects are examined in different parts of the project.

In the first part of the exercise, a narrowband channel is considered, where the effect of fading is noticeable at the system's output. Initially, we investigate the error probability in the normal state, and then various solutions to mitigate the fading effect in this channel are examined. These include Pulse Position Modulation, channel information estimation at the receiver and transmitter, time diversity, and trellis coding. In each subsection of this part, we analytically derive and simulate the error probability graph, and then compare it with other sections.

In the second part of the exercise, a wideband channel is taken into account, and we intend to utilize Orthogonal Frequency Division Multiplexing (OFDM) for data transmission and reception. First, we determine the required parameters of the OFDM system, and then we attempt to eliminate the channel effects by using methods such as Waterfilling, equalization, and space-time diversity. Additionally, we aim to investigate the impact of Clipping on the error probability of the OFDM system in the end.

**Part 1:** Narrow-Band Channel

We consider a wireless system. Let's assume that the channel is narrowband, and after sampling, the received signal at time instant "m" is given by the following equation:

$y[m]=h[m]x[m]+ω[m]$

$h[m \sim CN(0,1)$

$ω[m] \sim CN(0,N_0)$

1- Utilizing BPSK Modulation for Data Transmission

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/8ba3040f-6719-4359-a6e1-b5056ac6efd7)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/44f59f12-9814-4ea9-8c5e-944fecc83ea3)


2- Using Pulse Position Modulation for Data Transmission

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/a7b4edbc-5a8b-455f-97e6-686a875e4f38)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/759d3d3d-cf2d-4c98-94fd-31607bcb7ad0)

3- Using BPSK modulation for data transmission in the presence of available CSI

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/1fe0917e-59aa-40b0-916f-a918f87b9dbb)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/a6c7ab41-b66c-4e64-becc-7af5e5bc6aae)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/6726c193-cc08-4f31-b1dc-0f03c9285618)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/dbeae2e1-16b1-42fa-b3fc-71c01d0bc08c)

4- Using QPSK Modulation for Data Transmission

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/14f8b64c-1fd4-41cb-8ff0-4e928ae7d4e1)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/31742590-111a-4b46-9518-c5da646b44d7)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/217e7a71-10a8-4ae1-b5ff-76701fd618f6)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/4e18adbc-ed8e-4055-92bd-bdd13fd594cd)

5- Using Diversity in Time for Data Transmission

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/bdeea8b2-1b36-4238-85cf-241b27dbcba5)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/18e586a3-a4f0-48e3-9111-f033fb70e03b)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/740b28b9-f4bd-4cf4-bb05-e5abe970d81b)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/f6a3b9e8-799a-4525-9ad2-e59882b6c7d3)

6- Using Diversity in Location for Data Transmission

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/a44d2ec3-694b-4d3e-895d-2a26030bdacd)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/ac2d7096-18c5-4884-af58-cdac6195d3bd)

**Part 2:** Wide-Band Channel

1- Number of channel taps (L) and length of cyclic prefix (CP)

2- The number of subcarriers ($n_c$) in each OFDM block.

3- The number of OFDM blocks for transmitting the entire message

4- Block Diagram of the System in Transmitter and Receiver

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/7720ff09-74c7-4a86-8150-6b732f38123f)

5- Simulating System Question 4 and plotting error probability and channel capacity versus $SNR=P_max/(n_c N_0)$

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/8479ca69-0693-4566-9573-c6d573380e91)

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/93b013e0-f1e1-4990-a668-09b371322283)

6- Utilizing diversity method at the receiver location to compensate for fading in the receiver

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/1ab0fc8e-2171-4f8e-93f0-eae90edd3277)


7- Utilizing ZF and MMSE Equalizers at the Receiver to Compensate for Fading in the Receiver

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/8bd0d6e0-5eb6-45d0-8dcd-aa1ab5214866)


8- The impact of the Clipping effect on the error probability curve

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/14377da8-8883-4f75-a89d-637609b05051)

**Comparing:**

![image](https://github.com/ErfanPanahi/Implementation-of-Narrow-and-Wide-Band-Channels-Using-and-OFDM-System/assets/107314081/082f192c-f0b8-4f0c-b9e5-6ba202736b5e)
