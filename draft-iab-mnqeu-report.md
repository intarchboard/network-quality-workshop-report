---
title: "IAB workshop report: Measuring Network Quality for End-Users"
abbrev: title
docname: draft-iab-mnqeu-report-00
category: info
ipr: trust200902

stand_alone: yes
pi: [toc, sortrefs, symrefs, docmapping]

author:
  -
    ins: W. Hardaker
    name: Wes Hardaker
    org: USC/ISI
    email: ietf@hardakers.net
  -
    ins: O. Shapira
    name: Omer Shapira
    org: Apple
    email: omer_shapira@apple.com

normative:
  RFC2119:
  RFC5155:
  RFC4035:

informative:
  RFC1111:

  WORKSHOP:
    title: "IAB Workshop: Measuring Network Quality for End-Users, 2021"
    author:
      -
        ins: IAB
        name: IAB
    date: September, 2021

  Cheshire2021:
    title: "The Internet is a Shared Network"
    date: February 2021
    author:
      - ins: S. Cheshire
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/draft-cheshire-internet-is-shared-00b.pdf
  Iyengar2021:
    title: "The Internet Exists In Its Use"
    date: August 2021
    author:
      - ins: J. Iyengar
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/The-Internet-Exists-In-Its-Use.pdf
  Stein2021:
    title: "The Futility of QoS"
    date: August 2021
    author:
      - ins: J. Stein
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/QoS-futility.pdf
  Casas2021:
    title: "10 Years of Internet-QoE Measurements. Video, Cloud, Conferencing, Web and Apps. What do we need from the Network Side?"
    date: August 2021
    author:
      - ins: P. Casas
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/net_quality_internet_qoe_CASAS.pdf
  Pardue2021:
    title: "Lower-layer performance is not indicative of upper-layer success"
    date: February 2021
    author:
      - ins: L. Pardue
      - ins: S. Tellakula
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Lower-layer-performance-is-not-indicative-of-upper-layer-success-20210906-00-1.pdf
  Aldabbagh2021:
    title: "Regulatory perspective on measuring network quality for end users"
    date: September 2021
    author:
      - ins: A. Aldabbagh
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/2021-09-07-Aldabbagh-Ofcom-presentationt-to-IAB-1v00-1.pdf
  Welzl2021:
    title: "A Case for Long-Term Statistics"
    date: February 2021
    author:
      - ins: M. Welzl
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/iab-longtermstats_cameraready.docx-1.pdf
  Fabini2021:
    title: "Network Quality from an End User Perspective"
    date: February 2021
    author:
      - ins: J. Fabini
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Fabini-IAB-NetworkQuality.txt
  Mathis2021:
    title: "Preliminary Longitudinal Study of Internet Responsiveness"
    date: August 2021
    author:
      - ins: M. Mathis
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Preliminary-Longitudinal-Study-of-Internet-Responsiveness-1.pdf
  Schlinker2019:
    title: "Internet's performance from Facebook's edge"
    date: February 2019
    author:
      - ins: B. Schlinker
      - ins: I. Cunha
      - ins: Y. Chiu
      - ins: S. Sundaresan
      - ins: E. Katz-Basset
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Internet-Performance-from-Facebooks-Edge.pdf
  Foulkes2021:
    title: "Metrics helpful in assessing Internet Quality"
    date: September 2021
    author:
      - ins: J. Foulkes
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/IAB_Metrics_helpful_in_assessing_Internet_Quality.pdf
  Sivaraman2021:
    title: "Measuring Network Experience Meaningfully, Accurately, and Scalably"
    date: February 2021
    author:
      - ins: V. Sivaraman
      - ins: S. Madanapalli
      - ins: H. Kumar
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/CanopusPositionPaperCameraReady.pdf
  Reed2021:
    title: "Measuring IKSP Performance in Broadband America: A Study of Latency Under Load"
    date: February 2021
    author:
      - ins: D. P. Reed
      - ins: L. Perigo
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Camera_Ready_-Measuring-ISP-Performance-in-Broadband-America.pdf
  MacMillian2021:
    title: "Beyond Speed Test: Measuring Latency Under Load Across Different Speed Tiers"
    date: February 2021
    author:
      - ins: K. MacMillian
      - ins: N. Feamster
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/2021_nqw_lul.pdf
  Mirsky2021:
    title: "The Error Performance Metric in a Packet-Switched Network"
    date: February 2021
    author:
      - ins: G. Mirsky
      - ins: X. Min
      - ins: G. Mishra
      - ins: L. Han
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/IAB-worshop-Error-performance-measurement-in-packet-switched-networks.pdf
  Dion2021:
    title: "Focusing on latency, not throughput, to provide a better internet experience and network quality"
    date: August 2021
    author:
      - ins: G. Dion
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Nokia-IAB-Measuring-Network-Quality-Improving-and-focusing-on-latency-.pdf
  Balasubramanian2021:
    title: "Transport Layer Statistics for Network Quality"
    date: February 2021
    author:
      - ins: P. Balasubramanian
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/transportstatsquality.pdf
  Arkko2021:
    title: "Observability is needed to improve network quality"
    date: August 2021
    author:
      - ins: J. Arkko
      - ins: M. Kühlewind
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/iab-position-paper-observability.pdf
  Marx2021:
    title: "Merge Those Metrics: Towards Holistic (Protocol) Logging"
    date: February 2021
    author:
      - ins: R. Marx
      - ins: J. Herbots
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/MergeThoseMetrics_Marx_Jul2021.pdf
  Ghai2021:
    title: "Using TCP Connect Latency for Measuring CX and Network Optimization"
    date: February 2021
    author:
      - ins: R. Ghai
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/xfinity-wifi-ietf-iab-v2-1.pdf
  DeSchepper2021:
    title: "Challenges and opportunities of hardware support for Low Queuing Latency without Packet Loss"
    date: February 2021
    author:
      - ins: K. De Schepper
      - ins: O. Tilmans
      - ins: G. Dion
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Nokia-IAB-Measuring-Network-Quality-Low-Latency-measurement-workshop-20210802.pdf
  Michel2021:
    title: "Packet delivery time as a tie-breaker for assessing Wi-Fi access points"
    date: February 2021
    author:
      - ins: F. Michel
      - ins: O. Bonaventure
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/camera_ready_Packet_delivery_time_as_a_tie_breaker_for_assessing_Wi_Fi_access_points.pdf
  Kerpez2021:
    title: "Wi-Fi and Broadband Data"
    date: September 2021
    author:
      - ins: J. Shafiei
      - ins: K. Kerpez
      - ins: J. Cioffi
      - ins: P. Chow
      - ins: D. Bousaber
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Wi-Fi-Report-ASSIA.pdf
  Liubogoshchev2021:
    title: "Cross-layer cooperation for Better Network Service"
    date: February 2021
    author:
      - ins: M. Liubogoshchev
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Cross-layer-Cooperation-for-Better-Network-Service-2.pdf
  Laki2021:
    title: "Incentive-Based Traffic Management and QoS Measurements"
    date: February 2021
    author:
      - ins: S. Nadas
      - ins: B. Varga
      - ins: L. M. Contreras
      - ins: S. Laki
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/11/CamRdy-IAB_user_meas_WS_Nadas_et_al_IncentiveBasedTMwQoS.pdf
  Sengupta2021:
    title: "Fine-Grained RTT Monitoring Inside the Network"
    date: February 2021
    author:
      - ins: S. Sengupta
      - ins: H. Kim
      - ins: J. Rexford
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Camera_Ready__Fine-Grained_RTT_Monitoring_Inside_the_Network.pdf
  Morton2021:
    title: "Dream-Pipe or Pipe-Dream: What Do Users Want (and how can we assure it)?"
    date: September 2021
    author:
      - ins: A. Morton
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/draft-morton-ippm-pipe-dream-01.pdf
  Kilkki2021:
    title: "In Search of Lost QoS"
    date: February 2021
    author:
      - ins: K. Kilkki
      - ins: B. Finley
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Kilkki-In-Search-of-Lost-QoS.pdf
  Davies2021:
    title: "Measuring Network Impact on Application Outcomes using Quality Attenuation"
    date: September 2021
    author:
      - ins: N. Davies
      - ins: P. Thompson
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/PNSol-et-al-Submission-to-Measuring-Network-Quality-for-End-Users-1.pdf
  Zhang2021:
    title: "User-Perceived Latency to measure CCAs"
    date: September 2021
    author:
      - ins: M. Zhang
      - ins: V. Goel
      - ins: L. Xu
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/User_Perceived_Latency-1.pdf
  Paasch2021:
    title: "Responsiveness under Working Conditions"
    date: February 2021
    author:
      - ins: C. Paasch
      - ins: R. Meyer
      - ins: S. Cheshire
      - ins: O. Shapira
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/draft-cpaasch-ippm-responsiveness-1-1.pdf
  Briscoe2021:
    title: "A Single Common Metric to Characterize Varying Packet Delay"
    date: September 2021
    author:
      - ins: B. Briscoe
      - ins: G. White
      - ins: V. Goel
      - ins: K. De Schepper
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/single-delay-metric-1.pdf
  McIntyre2021:
    title: "An end-user approach to an Internet Score"
    date: September 2021
    author:
      - ins: C. Paasch
      - ins: K. McIntyre
      - ins: O. Shapira
      - ins: R. Meyer
      - ins: S. Cheshire
    seriesinfo: https://www.iab.org/wp-content/IAB-uploads/2021/09/Internet-Score-2.pdf

  tools.ookla_speedtest:
     title: "Speedtest by Ookla"
     target: https://www.speedtest.net
  tools.apple_networkQuality:
     title: "Apple Network Quality"
  tools.ping:
    title: "ping -- send ICMP ECHO_REQUEST packets to network hosts"

--- abstract

The Measuring Network Quality for End-Users workshop was held
virtually by the Internet Architecture Board (IAB) from September 14-16, 2021.
This report summarizes the workshop, the topics discussed, and some
preliminary conclusions drawn at the end of the workshop.

--- middle

# Introduction

The Internet Architecture Board (IAB) holds occasional workshops
designed to consider long-term issues and strategies for the
Internet, and to suggest future directions for the Internet
architecture.  This long-term planning function of the IAB is
complementary to the ongoing engineering efforts performed by working
groups of the Internet Engineering Task Force (IETF).

The Measuring Network Quality for End-Users workshop {{WORKSHOP}} was
held virtually by the Internet Architecture Board (IAB) in
September 14-16, 2021.  This report summarizes the workshop, the topics
discussed, and some preliminary conclusions drawn at the end of the
workshop.

## Problem space

The Internet in 2021 is quite different from what it was 10 years
ago. Today, it is a crucial part of everyone’s daily life. People use
the Internet for their social life, for their daily jobs, for routine
shopping, and for keeping up with major events. An increasing number
of people can access a Gigabit connection, which would be hard to
imagine a decade ago. And, thanks to improvements in security, people
trust the Internet for both planning their finances and for everyday
payments.

At the same time, some aspects of end-user experience have not
improved as much. Many users have typical connection latency that
remains at decade-old levels. Despite significant reliability
improvements in data center environments, end users often see
interruptions in service. Despite algorithmic advances in the field of
control theory, one can often find that the queuing delay in the
last-mile equipment exceeds the accumulated transit delay. Transport
improvements, such as QUIC, Multipath TCP, and TCP Fast Open are still
not fully supported in some networks. Likewise, various advances in
the security and privacy of user data are not widely supported, such
as encrypted DNS to the local resolver.

Some of the major factors behind this lack of progress is the popular
perception that throughput is the often sole measure of the quality of
Internet connectivity. With such narrow focus, the workshop aimed to
discuss various questions:

- What is the latency under typical working conditions?
- How reliable is the connectivity across longer time periods?
- Does the network allow the use of a broad range of protocols?
- What services can be run by clients of the network?
- What kind of IPv4, NAT, or IPv6 connectivity is offered, and are
  there firewalls?
- What security mechanisms are available for local services, such as
  DNS?
- To what degree are the privacy, confidentiality, integrity, and
  authenticity of user communications guarded?
- Improving these aspects of network quality will likely depend on
  measurement and exposing metrics to all involved parties, including
  to end users in a meaningful way. Such measurements and exposure of
  the right metrics will allow service providers and network operators
  to focus on the aspects that impacts the users’ experience most and
  at the same time empowers users to choose the Internet service that
  will give them the best experience.
- What are the fundamental properties of a network that contribute to good user experience?
- What metrics quantify these properties, and how to collect such metrics in a practical way?
- What are the best practices for interpreting those metrics, and incorporating those in a decision making process?
- What are the best ways to communicate these properties to service providers and network operators?
- How can these metrics be displayed to users in a meaningful way?

# Workshop Agenda

The Measuring Network Quality for End-Users workshop was divided into the
following main topic areas, further discussion in {{discussions}}:

- Introduction overviews and a keynote by Vint Cerf
- Metrics considerations
- Cross-layer considerations
- Synthesis
- Group conclusions

# Position Papers {#positionpapers}

The following position papers were received for consideration by the
workshop attendees.  The workshop's web-page {{WORKSHOP}} contains
archives of the papers, presentations and recorded videos.

- Ahmed Aldabbagh. "Regulatory perspective on measuring network quality for end users" {{Aldabbagh2021}}
- Al Morton. "Dream-Pipe or Pipe-Dream: What Do Users Want (and how can we assure it)?" {{Morton2021}}
- Alexander Kozlov . "The 2021 National Internet Segment Reliability Research"
- Anna Brunstrom. "Measuring newtork quality - the MONROE experience"
- Bob Briscoe, Greg White, Vidhi Goel and Koen De Schepper. "A single common metric to characterize varying packet delay" {{Briscoe2021}}
- Brandon Schlinker. "Internet’s performance from Facebook’s edge" {{Schlinker2019}}
- Christoph Paasch, Kristen McIntyre, Randall Meyer, Stuart Cheshire, Omer Shapira. "An end-user approach to the Internet Score" {{McIntyre2021}}
- Christoph Paasch, Randall Meyer, Stuart Cheshire, Omer Shapira. "Responsiveness under Working Conditions" {{Paasch2021}}
- Dave Reed, Levi Perigo. "Measuring ISP Performance in Broadband America: a Study of Latency Under Load" {{Reed2021}}
- Eve M. Schooler, Rick Taylor. "Non-traditional Network Metrics"
- Gino Dion. "Focusing on latency, not throughput, to provide better internet experience and network quality" {{Dion2021}}
- Gregory Mirsky, Xiao Min, Gyan Mishra, Liuyan Han. "Error Performance Measurement in Packet-Switched Networks" {{Mirsky2021}}
- Jana Iyengar. "The Internet Exists In Its Use" {{Iyengar2021}}
- Jari Arkko, Mirja Kuehlewind. "Observability is needed to improve network quality" {{Arkko2021}}
- Joachim Fabini. "Objective and subjective network quality" {{Fabini2021}}
- Jonathan Foulkes. "Metrics helpful in assessing Internet Quality" {{Foulkes2021}}
- Kalevi Kilkki, Benajamin Finley. "In Search of Lost QoS" {{Kilkki2021}}
- Karthik Sundaresan, Greg White, Steve Glennon . "Latency Measurement: What is latency and how do we measure it?"
- Keith Winstein. "Five Observations on Measuring Network Quality for Users of Real-Time Media Applications"
- Ken Kerpez, Jinous Shafiei, John Cioffi, Pete Chow, Djamel Bousaber. "State of Wi-Fi Reporting" {{Kerpez2021}}
- Kenjiro Cho. "Access Network Quality as Fitness for Purpose"
- Koen De Schepper, Olivier Tilmans, Gino Dion. "Challenges and opportunities of hardware support for Low Queuing Latency without Packet Loss" {{DeSchepper2021}}
- Kyle MacMillian, Nick Feamster. "Beyond Speed Test: Measuring Latency Under Load Across Different Speed Tiers" {{MacMillian2021}}
- Lucas Pardue, Sreeni Tellakula. "Lower layer performance not indicative of upper layer success" {{Pardue2021}}
- Matt Mathis. "Preliminary Longitudinal Study of Internet Responsiveness" {{Mathis2021}}
- Michael Welzl. "A Case for Long-Term Statistics" {{Welzl2021}}
- Mikhail Liubogoshchev. "Cross-layer Cooperation for Better Network Service" {{Liubogoshchev2021}}
- Mingrui Zhang, Vidhi Goel, Lisong Xu. "User-Perceived Latency to measure CCAs" {{Zhang2021}}
- Neil Davies, Peter Thompson. "Measuring Network Impact on Application Outcomes using Quality Attenuation" {{Davies2021}}
- Olivier Bonaventure, Francois Michel. "Packet delivery time as a tie-breaker for assessing Wi-Fi access points" {{Michel2021}}
- Pedro Casas. "10 Years of Internet-QoE Measurements. Video, Cloud, Conferencing, Web and Apps. What do we need from the Network Side?" {{Casas2021}}
- Praveen Balasubramanian. "Transport Layer Statistics for Network Quality" {{Balasubramanian2021}}
- Rajat Ghai. "Measuring & Improving QoE on the Xfinity Wi-Fi Network" {{Ghai2021}}
- Robin Marx, Joris Herbots. "Merge Those Metrics: Towards Holistic (Protocol) Logging" {{Marx2021}}
- Sandor Laki, Szilveszter Nadas, Balazs Varga, Luis M. Contreras. "Incentive-Based Traffic Management and QoS Measurements" {{Laki2021}}
- Satadal Sengupta, Hyojoon Kim, Jennifer Rexford. "Fine-Grained RTT Monitoring Inside the Network" {{Sengupta2021}}
- Stuart Cheshire. "The Internet is a Shared Network" {{Cheshire2021}}
- Toerless Eckert, Alex Clemm. "network-quality-eckert-clemm-00.4"
- Vijay Sivaraman, Sharat Madanapalli, Himal Kumar. "Measuring Network Experience Meaningfully, Accurately, and Scalably" {{Sivaraman2021}}
- Yaakov (J) Stein. "The Futility of QoS" {{Stein2021}}


# Discussions {#discussions}

The three day workshop was broken into four separate sections,
including introductory material and conclusions, that each played a
role in framing the discussions.

## Introduction and overviews

The Introduction section allowed participants to introduce and discuss
the problem space, existing mechanisms for QoS and QoE measurements.
Also discussed was the interaction between multiple users within the
Network, as well as the interaction between multiple layers of the OSI
stack.  Some existing measurement works were presented.  Vint Cerf
provided a key note describing the history and importance of
the topic.

## Metrics considerations

The Metrics section of the workshop concentrated on both defining new
and existing measures and how they might apply to different sections
of the Internet.  The need for improvements to latency and its
measurements was heavily discussed, especially for certain classes of
users such as live, collaborative content and gaming.

With the onset of COVID-19, the global population became more dependent on
vairous forms of collaboration and telepresence to get their work.

The metrics for network quality can be roughly grouped into:

1. Availability metrics, which indicate whether the user can access the network
   at all.
2. Capacity metrics, which indicate whether the actual line capacity is
   sufficient to meet the user demands.
3. Latency metrics, which indicate whether the user gets the data in time.
4. Higher-order metrics, which include both the network metrics, such as
   inter-packet arrival time, and the applicaiton metrics, such as the mean
   time between rebuffering for video streaming.

The availabiltiy metrics can be seen as derivative of either the capacity (zero
capacity leading to zero availability) or the latency (infinite latency
leading to zero availability).

Finally, the best metrics are those that are actionable.

### Availability metrics
TBD:

- Was the line down and for how long?
- Was the line unstable and for how long?

### Capacity metrics

If the network capacity does not meet the user demands, the network quality
will be impacted. Once the capacity meets the demands, increasing capacity
won't lead to further quality improvements.

The actual network connection capacity is determined by the equipment and the
lines along the network path, and it varies throughout the day and across
mutliple days. Studies involving DSL lines in North America indicate that over
30% of the DSL lines have capacity metrics that vary by more than 10%
throughout the day and accross multiple days.

Some factors that affect the actual capacity are:
1. Presence of a competing traffic, either in the LAN or in the WAN
   environments. In the LAN setting, the competing traffic reflects the
   multiple devices that share the Internet connection. In the WAN setting the
   competing traffic often originates from the unrelated network flows that
   happen to share the same network path.
2. Capabilities of the equipment along the path of the network connection,
   including the data transfer rate and the amount of memory used for
   buffering.
3. Active traffic management measures, such as traffic shapers and policers
   that are often used by the network providers.

There are other factors that can negatively affect the actual line capacities.

The user demands of the traffic follow the usage patterns and preferences of
the particular users. For example, large data transfers can use any available
capacity, while the media streaming applicaitons require limited capacity to
function correclty. Video-conferencing applications typically need less
capacity than high-definition video streaming.

### Latency metrics

End-to-end latency is the time it takes for a particular segment to traverse
the entire network path from the user to their destionation. The end-to-end
latency comprises several components:

1. The propagation delay, which reflects the path distance and the individual
   link technologies (e.g. fibre vs satellite). The propagation doesn't depend
   on the utilization of the network, to the extent that the network path
   remains constant.
2. The buffering delay, which reflects the time segments spend in the memory of
   the network equipment that connect the individual network links, as well as
   in the memory of the transmitting endpoint. The buffering delay depends on
   the network utilization, as well as on the algorithms that govern the queued segments.
3. The transport protocol delays, which reflects the time spent in
   retransmission and reassembly, as well as the time spent when the transport
   is "head-of-line blocked."
4. Some of the workshop sumbissions have explicitly called out the application
   delay, which reflects the inefficiencies in the application layer.

Tradionally, end-to-end latency is measured with tools such as {{tools.ping}}, as
well as with services such as {{tools.ookla_speedtest}}.
Such measurements are typically performed when the network is idle, and as a
result, such measurements reflect mostly the propagation delay.

A different way to measure the end-to-end latency is to perform the test when
the network is not idle, but in its typical working conditions.

The workshop participants used the term "Idle latency" when referring to the
subject of the former measurement methods, and "Working latency" when referring
to the latter.

While historically the tooling available for measuring latency focused on
measuring the idle latency, there is a trend in the industry to start measuring
the working latency as well, e.g. {{tools.apple_networkQuality}}.

### Measurement methodologies

The participants have proposed several concrete methodologies for measuring the
network quality for the end users.

{{Paasch2021}} introduced a new dimensionless metric, called RPM
(which stands for "round-trips per minute"), to communicate the quality of the
network to the end users. The metric represents the number of round trips a
segment can make within a minute when the network is under its typical working
conditions. The RPM metric reflects the combination of the propagation delay,
the buffering delay and the transport protocol delays. The RPM metric is designed
to be easy to explain to the general public - the higher values reflect better
network conditions, and the typical values are 3-4 digits.

{{Mathis2021}} have applied the RPM metric to the results of more than 4
billion download tests that were performed by M-Lab betwen 2010 and 2021.
During this timeframe, the measurement platform that M-Lab uses underwent
several upgrades, which allowed the research team to compare different versions
of the TCP CCAs. The study have demonstrated that the Cubic CCA have lowered
the responsiveness, which is attributed to the fact that Cubic uses large
network queues to maximize throughput.  A subsequent upgrade to the BBR CCA
have demonstrated increased responsivness (with the exception of several
locations such as NYC), which is consitent with the BBR design that makes
efforts to estimate the network capacity better, and relies on the capacity
estimations and pacing to maximize the throuhgput, vs. large queues.

The study have demonstrated that aside from the platform upgrades, the reported
RPM values are similar between the adjacent months, which suggests that the RPM
metric is stable. Changes in RPM metric that could not be attributed to changes
in the M-Lab platform were found to be consistent and lasting for several
months, which suggests that these were caused by ISPs upgrading their
equipment, or other events to the similar effect.

{{Schlinker2019}} presented a large scale study of the correlation between the
goodput and the quality of the experience of users of a large social network.

The authors performed the measurements at multiple datacenters from which video
segmetns of a set size were streamed to a large number of end users. The
authors used "the probability of transmitting vvideo segment of size S at
goodput G" as the metric. Goodput is highly dependent on the transport delays,
but is less sensitive to the latency. Further, the goodput is highly dependent
on the choice of the transport protocol (the authors used QUIC with BBRv1.)

Specifically, the authors suggested using the probabilty of
achieving desired goodput G when transmitting object of set size S.

TODO: insert formula

The choice of goodput and the logicistical metric were driven by the need to
assess the maximal quality of the content that can be effectively served by the
network. Specifically, the suggested metric has several properties that are
desireable for operators of large scale video streaming service:

1. The suggested metric is easy to aggregate, and therefore can be used to
   reflect the network quality across multiple connections - up to the scale of
   entire autonomous systems.
2. The suggested metric is directly applicable to the operators of streaming
   media services, since it allows to choose the most appropriate compression
   algorithms and bitrates to achieve the highest quality for a given network
   connection (or an aggregate, such as AS), without significant degradation of
   goodput.

The study have found that the short video clips, which constitute the majority
of the traffic, are typically consumed in a sequential way. Since the
sequential consumption of video is less sensitive to the buffering delays than
random-access consumption, the goodput metric may not be as sensitive to the
buffering delay as the RPM metric. It is, however, influenced by all types of
delay, and in particular is useful for identifying infrstructure nodes that are
shared by multiple forms of traffic.

As such, the suggested metric seems highly valuable to the operators of
streaming services, either when estimated the needed network capacity, or when
deciding what bitrate values to use in order to deliver the content at the
highest quality without stretching the capacity of the network.


{{Reed2021}} presents the results of FCC's "Measuring the Broadband America" (MBA) study.
### RPM metric considerations

The workshop participants have agreed that the RPM metric is an effective way
to communicate the network quality to the end users.

There's remaining work to be done before the RPM metric can be used as an
industry standard:

- The use of natural traffic vs. synthetic traffic.

The RPM metric, as defined in {{Paasch2021}}, relies on synthetic traffic to
bring the network into the working conditions.

There are pros and cons of the use of the synthetic traffic when compared to
the natural traffic that's generated by the applications which the end user
runs.

Using natural traffic to measure the responsiveness of the network is more
reflective of the interactions of users with the specific application.
Additionally, utilizing natural traffic to measure the network responsiveness
does not consume any additional resources beyond what is required by the
applications. Finally, using the natural traffic minimizes any potential impact
of the measurement on other applications.

Using the synthetic traffic to measure the responsiveness has the benefit of
reliably assessing the responsiveness when used by any particular applicaiton,
or by multiple applicaitons at once. The results of responsiveness
test that utilizes synthetic traffic allow comparing different
equipment or different locaitons in a fair way. Additionally, using a
synthetic traffic makes it easier to standardize the responsiveness
test - both the specific protocols that are used, as well as the test dynamics.
Finally, the use of active measurement alleviates the privacy concerns
that may arise if the users were not aware that their activities are used
to measure the quality of the network.

Work remains on making the RPM methodology more robust, as well as on
reconciling the two fundamental ways of measuring the network responsivenes.
This work had been taken to the IPPM working group within the IETF.

The workshop participants believe that it would be valuable to develop
methodology which could be used by the community to reconcile the RPM metric
with the goodput metric.

### Metrics considerations - conclusions

Through the course of the workshop, the following statements have emerged:

Both the goodput and the latency are important to measure. Today, users in many
locations around the world have access to gigabit throughput, and measuring the
latency is more important for these. Otehr users can not (yet) benefit from the
high-bandwidth network access. For these users, both throughput and latency
should be measured.

When measuring the latency, one should measure the latency under typical
working conditions, since the idle latency is not a good estimator of the user
experience. Data shows that there is dramatic difference between the idle
latency and the working latency. The RPM metric, described in {{Paasch2021}}
is one way to communicate the working latency to the users.

Most of existing tools today focus on measuring idle latency. It is important
to continue invsesting into a standard methodology (and a toolkit) to make
it possible for anyone to measure the working latency.


## Cross-layer considerations

In the Cross-layer section participants presented material and discussed
how accurately measuring exactly where problems occur is difficult
when many components of a network connection can affect the
measurement.  Discussion centered especially on the differences
between physically wired and wireless connections and the difficulties
of accurately determining problem spots when multiple different
network types are responsible for the quality.

## Synthesis

Finally, in the Synthesis section presentations and discussions
concentrated on the next steps likely needed to make forward
progress. Of particular concern is how to bring forward measurements
that can make sense to end users trying to make subscription
decisions.

# Conclusions

During the final hour of the workshop we gathered statements that the
group thought were summary statements from the 3 day event.  We later
discarded any that were in contention (listed further below for
completeness).  For this document, the editor took the original list
and divided it into rough categories, applied some suggested edits
discussed on the mailing list and further edited for clarity and to
provide context.

## General statements

1. Bandwidth is necessary but not alone sufficient.
2. In many cases, Internet users don’t need more bandwidth, but rather
   need "better bandwidth" -- i.e., they need other improvements to
   their connectivity.
3. We need both active and passive measurements – passive measurements
   can provide historical debugging.
4. We need passive measurements to be continuous and archivable and
   queriable – include reliability/connectivity measurements.
5. A really meaningful metric for users is whether their application
   will work properly or fail because of a lack of a network with
   sufficient characteristics.
6. A useful metric for goodness must actually incentive goodness --
   good metrics should be actionable to help drive industries toward
   improvement.
7. A lower latency Internet, however achieved would benefit all end
   users.

## Specific statements about detailed protocols/techniques

8. Round trips Per Minute (RPM) is a useful, consumable metric.
9. We need a usable tool that fills the current gap between network
   reachability, latency, and speed tests.
10. End-users that want to be involved in QoS decisions should be able
    to voice their needs and desires.
11. Applications are needed that can perform and report good quality
    measurements in order to identify insufficient points in
    network access.
12. Research done by regulators indicate that users/consumers prefer
    a simple metric per application, which frequently resolves to
    whether the application will work properly or not.
13. New measurements and QoS or QoE techniques should not rely only or
    depend on reading TCP headers.
10. It is clear from developers of interactive applications and from
    network operators that lower latency is a strong factor in user
    QoE.  However, metrics are lacking to support this statement
    directly.

## Problem statements and concerns

15. Latency mean and medians are distractions from better measurements.
16. It is frustrating to only measure network services without
    simultaneously improving those services.
17. Stakeholder incentives aren’t aligned for easy wins in this space.
    Incentives are needed to motivate improvements in public network
    access.  Measurements may be one step toward driving competitive
    market incentive.
18. For future-proof networking, it is important to measure the
    ecological impact of material and energy usage.
19. We do not have incontrovertible evidence that any one metric
    (e.g., latency or speed) is more important than others to persuade
    device vendors to concentrate on any one optimization.

## No-consensus reached statements

Additional statements were recorded that did not have consensus of the
group at the time, but we list them here for completeness about the fact
they were discussed:

1. We do not have incontrovertible evidence that buffer bloat is a
   prevalent problem.
2. The measurement needs to support reporting localization in order to
   find problems.  Specifically:
    - Detecting a problem is not sufficient if you can’t find the location.
    - Need more than just English – different localization concerns.
3. Stakeholder incentives aren’t aligned for easy wins in this space.

# Follow-on work

There was discussion during the workshop about where future work
should be performed.  The group agreed that some work could be done
more immediately within existing IETF working groups (e.g. IPPM,
DetNet and RAW), while other longer-term research may be needed in
IRTF groups.

# Security considerations

A few security relevant topics were discussed at the workshop,
including but not limited to:

- What prioritization techniques can work without invading the privacy
  of the communicating parties.
- How oversubscribed networks can essentially be viewed as a DDoS
  attack.

--- back

# Participants List

The following is a list of participants who attended the workshop over a remote connection:

    Ahmed Aldabbagh
    Al Morton
    Alexander Clemm
    Alvaro Retana
    Anna Brunstrom
    Balazs Varga
    Bjørn Ivar Teigen
    Bob Briscoe
    Brandon Schlinker
    Bren Tully Walsh
    Christoph Paasch
    Cindy Morgan
    Cullen Jennings
    Dan Siemon
    Dave Taht
    David Reed
    David Schinazi
    Djamel Bousaber
    Eve Schooler
    Evgeny Khorov
    François Michel
    Gavin Young
    Geoff Huston
    Gino Dion
    Gorry Fairhurst
    Greg Mirsky
    Greg White
    Jana Iyengar
    Jared Mauch
    Jari Arkko
    Jason Livingood
    Jiankang Yao
    Jim Gettys
    Jinous Shafiei
    Joachim Fabini
    John Cioffi
    Jonathan Foulkes
    Joon Kim
    Joris Herbots
    Kalevi Kilkki
    Karthik Sundaresan
    Kathleen Nichols
    Keith Winstein
    Ken Kerpez
    Kenjiro Cho
    Koen De Schepper
    Kristen McIntyre
    Kyle MacMillan
    Lai Yi Ohlsen
    Lars Eggert
    Levi Perigo
    Lisong Xu
    Lucas Pardue
    Luis M. Contreras
    Mat Ford
    Matt Mathis
    Michael Welzl
    Mikhail Liubogoshchev
    Mingrui Zhang
    Neil Davies
    Nick Feamster
    Nicolas (Tessares)
    Olivier Bonaventure
    Omer Shapira
    Pedro Casas
    Peter Thompson
    Praveen Balasubramanian
    Rajat Ghai
    Randall Meyer
    Rich Brown
    Rick Taylor
    Roberto
    Robin Marx
    Russ White
    Sam Crawford
    Satadal Sengupta
    Shapelez
    Sharat Madanapalli
    Steve Christianson
    Stuart Cheshire
    Szilveszter Nadas
    Toerless Eckert
    Toke Høiland-Jørgensen
    Tommy Pauly
    Vesna Manojlovic
    Vidhi Goel
    Vijay Sivaraman
    Vint Cerf
    Wes Hardaker
    Zhenbin Li


# IAB Members at the Time of Approval

Internet Architecture Board members at the time this document was
approved for publication were:

    Jari Arkko

    Deborah Brungard
    Ben Campbell
    Lars Eggert
    Wes Hardaker
    Cullen Jennings
    Mirja Kühlewind
    Zhenbin Li
    Jared Mauch
    Tommy Pauly
    Colin Perkins
    David Schinazi
    Russ White
    Jiankang Yao

# Acknowledgements

The authors would like to thank the workshop participants, the members
of the IAB, and the program committee for creating and participating
in many interesting discussions.

## Draft contributors

Thank you to the people that contributed edits to this draft:

    Brian Trammell
    Erik Auerswald
    Simon Leinen


## Workshop Chairs

The workshop chairs consisted of:

    Evgeny Khorov
    Omer Shapira
    Wes Hardaker

## Program Committee

The program committee consisted of:

    Christoph Paasch
    Cullen Jennings
    Geoff Huston
    Greg White
    Jari Arkko
    Jason Livingood
    Jim Gettys
    Katarzyna Kosek-Szott
    Kathleen Nichols
    Keith Winstein
    Matt Mathis
    Mirja Kuehlewind
    Nick Feamster
    Olivier Bonaventure
    Randall Meyer
    Sam Crowford
    Stuart Cheshire
    Toke Hoiland-Jorgensen
    Tommy Pauly
    Vint Cerf

# Github Version of this document

While this document is under development, it can be viewed and tracked
here:

https://github.com/intarchboard/network-quality-workshop-report

