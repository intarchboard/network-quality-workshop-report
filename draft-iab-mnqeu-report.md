---
title: "IAB workshop report: Measuring Network Quality for End-Users"
abbrev: title
docname: draft-iab-mnqeu-report-02
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
  RFC765:
    title: "FILE TRANSFER PROTOCOL"
    author:
      - ins: Jonathan B. Postel
    date: June 1980
    seriesinfo: https://datatracker.ietf.org/doc/html/rfc765
  RFC821:
    title: "SIMPLE MAIL TRANSFER PROTOCOL"
    author:
      - ins: Jonathan B. Postel
    date: August 1982
    seriesinfo: https://datatracker.ietf.org/doc/html/rfc821
  RFC977:
    title: "Network News Transfer Protocol"
    author:
      - ins: Brian Kantor
      - ins: Phil Lapsley
    date: February 1986
    seriesinfo: https://datatracker.ietf.org/doc/html/rfc977
  RFC1436:
    title: "Internet Gopher Protocol"
    author:
      - ins: M. McCahill
      - ins: P. Lindner
      - ins: D. Johnson
      - ins: B. Alberti
    date: March 1993
    seriesinfo: https://datatracker.ietf.org/doc/html/rfc1436
  RFC1945:
    title: "Hypertext Transfer Protocol -- HTTP/1.0"
    author:
      - ins: T. Berners-Lee
      - ins: R. Fielding
      - ins: H. Frystyk
    date: May 1996
    seriesinfo: https://datatracker.ietf.org/doc/html/rfc1945

  FCC_MBA:
    title: "Measuring Broadband America"
    seriesinfo: https://www.fcc.gov/general/measuring-broadband-america

  FCC_MBA_methodology:
    title: "Measuring Broadband America - Open Methodology"
    seriesinfo: https://www.fcc.gov/general/measuring-broadband-america-open-methodology

  Scuba:
    title: "Facebook Scuba"
    target: https://research.facebook.com/publications/scuba-diving-into-data-at-facebook/

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

  Speedtest:
     title: "Speedtest by Ookla"
     target: https://www.speedtest.net
  NetworkQuality:
     title: "Apple Network Quality"
     target: https://support.apple.com/en-us/HT212313
  samknows:
     title: "samknows"
     target: https://www.samknows.com/  

--- abstract

the measuring network quality for end-users workshop was held
virtually by the internet architecture board (iab) from september 14-16, 2021.
this report summarizes the workshop, the topics discussed, and some
preliminary conclusions drawn at the end of the workshop.

--- middle

# introduction

the internet architecture board (iab) holds occasional workshops designed to
consider long-term issues and strategies for the internet, and to suggest
future directions for the internet architecture.  this long-term planning
function of the iab is complementary to the ongoing engineering efforts
performed by working groups of the internet engineering task force (ietf).

the measuring network quality for end-users workshop {{workshop}} was held
virtually by the internet architecture board (iab) in september 14-16, 2021.
this report summarizes the workshop, the topics discussed, and some preliminary
conclusions drawn at the end of the workshop.

## problem space

the internet in 2021 is quite different from what it was 10 years ago. today, it
is a crucial part of everyone’s daily life. people use the internet for their
social life, for their daily jobs, for routine shopping, and for keeping up
with major events. an increasing number of people can access a gigabit
connection, which would be hard to imagine a decade ago. and, thanks to
improvements in security, people trust the internet for financial
banking transactions, purchasing goods and everyday bill payments.

at the same time, some aspects of end-user experience have not
improved as much.  many users have typical connection latencies that
remain at decade-old levels.  despite significant reliability
improvements in data center environments, end users also still often see
interruptions in service. despite algorithmic advances in the field of
control theory, one still finds that the queuing delays in the
last-mile equipment exceeds the accumulated transit delays. transport
improvements, such as quic, multipath tcp, and tcp fast open are still
not fully supported in some networks.
<!-- i'm not sure there is agreement about this next sentence - wes -->
likewise, various advances in
the security and privacy of user data are not widely supported, such
as encrypted dns to the local resolver.

some of the major factors behind this lack of progress is the popular
perception that throughput is the often sole measure of the quality of
internet connectivity. with such narrow focus, the measuring network
quality for end-users workshop aimed to discuss various questions:

- what is user latency under typical working conditions?
- how reliable is connectivity across longer time periods?
- do networks allow the use of a broad range of protocols?
- what services can be run by network clients?
- what kind of ipv4, nat, or ipv6 connectivity is offered, and are there
  firewalls?
- what security mechanisms are available for local services, such as dns?
- to what degree are the privacy, confidentiality, integrity, and authenticity
  of user communications guarded?
- improving these aspects of network quality will likely depend on
  measurement and exposing metrics in a meaningful way to all involved
  parties, including to end users. such measurement and exposure of
  the right metrics will allow service providers and network operators
  to concentrate focus on their users’ experience and will
  simultaneously empower users to choose the internet service
  providers that can deliver the best experience based on their needs.
- what are the fundamental properties of a network that contributes to
  a good user experience?
- what metrics quantify these properties, and how can we collect such metrics in a
  practical way?
- what are the best practices for interpreting those metrics, and incorporating
  those in a decision making process?
- what are the best ways to communicate these properties to service providers
  and network operators?
- how can these metrics be displayed to users in a meaningful way?

# workshop agenda

the measuring network quality for end-users workshop was divided into the
following main topic areas, further discussion in {{discussions}}:

- introduction overviews and a keynote by vint cerf
- metrics considerations
- cross-layer considerations
- synthesis
- group conclusions

# position papers {#positionpapers}

the following position papers were received for consideration by the
workshop attendees.  the workshop's web-page {{workshop}} contains
archives of the papers, presentations and recorded videos.

- ahmed aldabbagh. "regulatory perspective on measuring network quality for end users" {{aldabbagh2021}}
- al morton. "dream-pipe or pipe-dream: what do users want (and how can we assure it)?" {{morton2021}}
- alexander kozlov . "the 2021 national internet segment reliability research"
- anna brunstrom. "measuring newtork quality - the monroe experience"
- bob briscoe, greg white, vidhi goel and koen de schepper. "a single common metric to characterize varying packet delay" {{briscoe2021}}
- brandon schlinker. "internet’s performance from facebook’s edge" {{schlinker2019}}
- christoph paasch, kristen mcintyre, randall meyer, stuart cheshire, omer shapira. "an end-user approach to the internet score" {{mcintyre2021}}
- christoph paasch, randall meyer, stuart cheshire, omer shapira. "responsiveness under working conditions" {{paasch2021}}
- dave reed, levi perigo. "measuring isp performance in broadband america: a  study of latency under load" {{reed2021}}
- eve m. schooler, rick taylor. "non-traditional network metrics"
- gino dion. "focusing on latency, not throughput, to provide better internet  experience and network quality" {{dion2021}}
- gregory mirsky, xiao min, gyan mishra, liuyan han. "error performance measurement in packet-switched networks" {{mirsky2021}}
- jana iyengar. "the internet exists in its use" {{iyengar2021}}
- jari arkko, mirja kuehlewind. "observability is needed to improve network quality" {{arkko2021}}
- joachim fabini. "objective and subjective network quality" {{fabini2021}}
- jonathan foulkes. "metrics helpful in assessing internet quality" {{foulkes2021}}
- kalevi kilkki, benajamin finley. "in search of lost qos" {{kilkki2021}}
- karthik sundaresan, greg white, steve glennon . "latency measurement: what is latency and how do we measure it?"
- keith winstein. "five observations on measuring network quality for users of real-time media applications"
- ken kerpez, jinous shafiei, john cioffi, pete chow, djamel bousaber. "state of  wi-fi reporting" {{kerpez2021}}
- kenjiro cho. "access network quality as fitness for purpose"
- koen de schepper, olivier tilmans, gino dion. "challenges and opportunities of hardware support for low queuing latency without packet loss" {{deschepper2021}}
- kyle macmillian, nick feamster. "beyond speed test: measuring latency under  load across different speed tiers" {{macmillian2021}}
- lucas pardue, sreeni tellakula. "lower layer performance not indicative of upper layer success" {{pardue2021}}
- matt mathis. "preliminary longitudinal study of internet responsiveness" {{mathis2021}}
- michael welzl. "a case for long-term statistics" {{welzl2021}}
- mikhail liubogoshchev. "cross-layer cooperation for better network service" {{liubogoshchev2021}}
- mingrui zhang, vidhi goel, lisong xu. "user-perceived latency to measure ccas" {{zhang2021}}
- neil davies, peter thompson. "measuring network impact on application outcomes using quality attenuation" {{davies2021}}
- olivier bonaventure, francois michel. "packet delivery time as a tie-breaker for assessing wi-fi access points" {{michel2021}}
- pedro casas. "10 years of internet-qoe measurements. video, cloud,
  conferencing, web and apps. what do we need from the network side?" {{casas2021}}
- praveen balasubramanian. "transport layer statistics for network quality" {{balasubramanian2021}}
- rajat ghai. "measuring & improving qoe on the xfinity wi-fi network" {{ghai2021}}
- robin marx, joris herbots. "merge those metrics: towards holistic (protocol) logging" {{marx2021}}
- sandor laki, szilveszter nadas, balazs varga, luis m.
  contreras. "incentive-based traffic management and qos measurements" {{laki2021}}
- satadal sengupta, hyojoon kim, jennifer rexford. "fine-grained rtt monitoring inside the network" {{sengupta2021}}
- stuart cheshire. "the internet is a shared network" {{cheshire2021}}
- toerless eckert, alex clemm. "network-quality-eckert-clemm-00.4"
- vijay sivaraman, sharat madanapalli, himal kumar. "measuring network experience meaningfully, accurately, and scalably" {{sivaraman2021}}
- yaakov (j) stein. "the futility of qos" {{stein2021}}


# workshop topics and discussion {#discussions}

the agenda for the three day workshop was broken into four separate
sections that each played a role in framing the discussions. the
workshop started with a series of introduction and problem space
presentations {introduction-section}, followed by metrics considerations
{{discussion-metrics}}, cross layer considerations
{{discussions-cross-layer}} and a synthesis discussion {{synthesis}}.
after the four subsections concluded, a follow-on discussion was held
to draw conclusions that could be agreed upon by workshop participants
({{conclusions}}).

## introduction and overviews {#introduction-section}

the workshop started with a broad focus on the state of user quality
of service (qos) and quality of experience (qoe) on the internet today.
the goal of the introductory talks was to set the stage for the
workshop by describing both the problem space and the current
solutions in place and their limitations.

the introduction presentations provided views of existing qos and qoe
measurements and their effectiveness. also discussed was the
interaction between multiple users within the network, as well as the
interaction between multiple layers of the osi stack.  vint cerf
provided a key note describing the history and importance of the
topic.

### key points from the keynote by vint cerf {#dicsucssion-intro-keynote}

we may be operating in a networking space with dramatically different
parameters compared to 30 years ago. this differentiation justifies
re-considering not only the importance of one metric over the other,
but also re-considering the entire metaphor.

it is time for the experts to look at not only at adjusting tcp, but
also at exploring other protocols, such as quic has done lately. it's
important that we feel free to consider alternatives to tcp. tcp is
not a teddy bear, and one should not be afraid to replace it with a
transport later with better properties that better benefits its users.

a suggestion: we should consider exercises to identify desirable
properties. as we are looking at the parametric spaces, one can
identify “desirable properties”, as opposed to “fundamental
properties”, for example a low-latency property. an example coming
from arpa: you want to know where the missile is now, not where it
was. understanding drives particular parameter creation and selection
in the design space.

when parameter values are changed in extreme, such as connectiveness,
alternative designs will emerge. one case study of note is the
interplanetary protocol, where "ping" is no long indicative of
anything useful. while we look at responsiveness, we should not ignore
connectivity.

unfortunately, maintaining backward compatibility is painful. the work
on designing ipv6 so as to transition from ipv4 could have been done
better if the backward compatibility was considered. this is too late
for ipv6, but this problem space is not too late for the future laying
problems.

ipv6 is still not implemented fully everywhere.  it’s been a long road
to deployment since starting work in 1996, and we are still not
there. in 1996, the thinking was that it was quite easy to implement
ipv6, but that failed to hold true. in 1996 the dot-com boom began,
with lots of money was spent quickly, and the moment was not caught in
time while the market expanded exponentially. this should serve as a
cautionary tale.

one last point: consider performance across multiple hops in the
internet. we’ve not seen many end-to-end metrics, as successfully
developing end-to-end measurements across different network and
business boundaries is quite hard to achieve. a good question to ask
when developing new protocols is "will the new protocol work across
multiple network hops?"

multi-hop networks are being gradually replaced by humongous, flat
networks with sufficient connectivity between operators so that
systems become 1 hop or 2 hop at most away from each other
(e.g. google, facebook, amazon). the fundamental architecture of the
internet is changing.

### introductory talks  {#discussion-introductions}

the internet is a shared network, built on the ip protocols using
packet-switching to interconnect multiple autonomous networks. the
internet's departure from circuit-switching technologies allowed it to
scale beyond any other known network design. on the other hand, the
lack of in-network regulation made it difficult to ensure the best
experience for every user.

as internet use cases continue to expand, it becomes increasingly more
difficult to predict which network characteristics correlate with
better user experiences. different application classes, e.g., video
streaming and teleconferencing, can affect user experience in complex
and difficult to measure ways. internet utilization shifts rapidly
during the course of each day, week and year, which further
complicates identifying key metrics capable of predicting a good user
experience.

quality of service (qos) initiatives attempted to overcome these
difficulties by strictly prioritizing different types of
traffic. however, qos metrics do not always correlate with user
experience. the utility of the qos metric is further limited by the
difficulties in building solutions with the desired qos
characteristics.

quality of experience (qoe) initiatives attempted to integrate the
psychological aspects of how quality is perceived, and created
statistical models designed to optimize the user experience. despite
these high modeling efforts, the qoe approach proved beneficial in
certain application classes. unfortunately, generalizing the models
proved to be difficult, and the question of how different applications
affect each other when sharing the same network remains an open problem.

the industry's focus on giving the end-user more throughput/bandwidth
led to remarkable advances. in many places around the world, a home
user enjoys gigabit speeds to their internet service provider.  this
is so remarkable that it would have been brushed off as science
fiction a decade ago. however, the focus on increased capacity came at
the expense of neglecting another important core metric: latency. as
a result, end-users whose experience is negatively affected by high
latency were advised to upgrade their equipment to get more
throughput instead. {{macmillian2021}} showed that sometimes such an
upgrade can lead to latency improvements, due to the economical
reasons of overselling the "value-priced" data plans.

as the industry continued to give end users more throughput, while
mostly neglecting latency concerns, application designs started to
employ various latency and short service disruption hiding techniques.
for example, a user's experience of web browser performance is closely
tired to the content in the browser's local cache. while such
techniques can clearly improve the user experience when using stale
data is possible, this development further decouples user experience
from core metrics.

in the most recent 10 years, efforts by dave taht and the bufferbloat
society had led to significant progress updating queuing algorithms to
reduce latencies under load compared to simipler fifo
queues. unfortunately, the home router industry has yet to implement
these algorithms, mostly due to marketing and cost concerns. most home
router manufacturers depend on system on a chip (soc) acceleration to
create products with a desired throughput. soc manufacturers opt for
simpler algorithms and aggressive aggregation, reasoning that a
higher-throughput chip will have guaranteed demand. because consumers
are offered choices primarily among different high throughput devices,
the perception that a higher throughput leads to higher a quality of
service continues to strengthen.

the home router is not the only place that can benefit from clearer
indications of acceptable performance for users. since users perceive
the internet via the lens of applications, its important to appeal to
the application vendors that they should adopt solutions that stress
lower latencies. unfortunately, while bandwidth is straightforward to
measure, responsiveness is trickier. many applications have found a
set of metrics which are helpful to their realm, but do not generalize
well and cannot become universally applicable. furthermore, due to the
highly competitive application space, vendors may have economic
reasons to avoid sharing their most useful metrics.

<!-- incomplete: suggest we leave it out
finally, the internet infrastructure that connects the applictions to the users is yet another place where better measurements may help driving towards the better internet.
-->

### introductory talks - key points  {#discussion-introductions-summary}

1. measuring bandwidth is necessary, but is not alone sufficient.
2. in many cases, internet users don’t need more bandwidth, but rather
   need "better bandwidth" -- i.e., they need other connectivity improvements.
3. users perceive the quality of their internet connection based
   on the applications they use, which are affected by a combination
   of factors. there's little value in exposing a typical user to the
   entire spectrum of possible reasons for the poor performance
   perceived in their application-centric view.
4. many factors affecting user experience are outside the users'
   sphere of control. it's unclear whether exposing users to these
   other factors will help users understand the state of their network
   performance. in general, users prefer simple, categorical
   choices (e.g. "good", "better", and "best" options).
5. the internet content market is highly competitive, and many
   applications develop their own "secret sauce."

## metrics considerations {#discussion-metrics}

in the second agenda section, the workshop continued its discussion
about metrics that can be used instead of or in addition to available
bandwidth. several workshop attendees presented deep-dive studies on
measurement methodology.

### common performance metrics

losing internet access entirely is, of course, the worst user
experience. unfortunately, unless rebooting the home router restores
connectivity, there is little a user can do other than contacting
their service provider. nevertheless, there is value in the systematic
collection of availability metrics on the client side: these can help
the user's isp localize and resolve issues faster, while enabling
users to better choose between isps. one can measure availability
directly by simply attempting connections from the client-side to
distant locations of interest. for example, ookla's ({{speedtest}})
uses a large number of android devices to measure network and cellular
availability around the globe. ookla collects hundreds of millions of
data points per day, and uses these for accurate availability
reporting. an alternative approach is to derive availability from the
failure rates of other tests. for example, {{fcc_mba}}
{{fcc_mba_methodology}} uses thousands of off-the shelf routers,
called "whiteboxes", with measurement software developed by
{{samknows}}. these whiteboxes perform an array of network tests and
report availability based whether test connections were successful or
not.

measuring available capacity can be helpful to end-users, but it is
even more valuable for service providers and application
developers. high-definition video streaming requires significantly
more capacity than any other type of traffic. at the time of the
workshop, video traffic constituted 90% of overall internet traffic
and contributed to 95% of the revenues from monetization (via
subscriptions, fees, or ads). as a result, video streaming services,
such as netflix, need to continuously cope with rapid changes in
available capacity. the ability to measure available capacity in
real-time leverages the different adaptive bitrate (abr) compression
algorithms to ensure the best possible user experience. measuring
aggregated capacity demand allows internet service provider's to be
ready for traffic spikes. for example, during the end-of-year holiday
season, the global demand for capacity has been shown to be 5-7 times
higher than during other seasons.  for end-users, knowledge of their
capacity needs can help them select the best data plan given their
intended usage. in many cases, however, end-users have more than
enough capacity and adding more bandwidth will not improve their
experience -- after a point it is no longer the limiting factor in
user experience. finally, the ability to differentiate between the
"throughput" and the "goodput" can be helpful in identifying when the
network is saturated.

in measuring network quality, latency is defined as the time it takes
a packet to traverse a network path from one end to the other. at the
time of this report, users in many places worldwide can enjoy internet
access that has adequately high capacity and availability for their
current needs. for these users, latency improvements rather than
bandwidth improvements can lead to the most significant improvements
in quality of experience. the established latency metric is a
round-trip time (rtt), commonly measured in milliseconds. however,
users often find rtt values unintuitive since, unlike other
performance metrics, high rtt values indicate poor latency and users
typically understand higher scores to be better. to address this,
{{paasch2021}} and {{mathis2021}} presented an inverse metric, called
"round-trips per minute" (rpm).

there is an important distinction between "idle latency" and "latency
under working conditions." the former is measured when the network is
underused and reflects a best-case scenario. the latter is measured
when the network is under a typical workload. until recently, typical
tools reported a network's idle latency, which can be misleading. for
example, data presented at the workshop shows that idle latencies can
be up to 25 times lower than the latency under typical working
loads. because of this, it is essential to make a clear distinction
between the two when presenting latency to end-users.

data shows that rapid changes in capacity affect
latency. {{foulkes2021}} attempts to quantify how often a rapid change
in capacity can cause network connectivity to become "unstable" (i.e.,
having high latency with very little throughput). such changes in
capacity can be caused by infrastructure failures, but are much more
often caused by in-network phenomena, like changing traffic
engineering policies or rapid changes in cross-traffic.

data presented at the workshop shows that 36% of measured lines have
capacity metrics that vary by more than 10% throughout the day and
across multiple days. these differences are caused by many variables,
including local connectivity methods (wifi vs. ethernet), competing
lan traffic, device load/configuration, time of day and local
loop/backhaul capacity. these factor variations make measuring
capacity using only an end-user device or other end-network
measurement difficult. a network router seeing aggregated traffic from
multiple devices provides a better vantage point for capacity
measurements. such a test can account for the totality of local
traffic and perform an independent capacity test. however, various
factors might still limit the accuracy of such a test. accurate
capacity measurement requires multiple samples.

as users perceive the internet through the lens of applications, it
may be difficult to correlate changes in capacity and latency with the
quality of the end-user experience. for example, web browsers rely on
cached page versions to shorten page load times and mitigate
connectivity losses. in addition, social networking applications often
rely on pre-fetching their "feed" items. these techniques make the
core in-network metrics less indicative of the users' experience and
necessitates collecting data in-application.

it is helpful to distinguish between applications that operate on a
"fixed latency budget" from those that have more tolerance to latency
variance. cloud gaming serves as an example application that requires
a "fixed latency budget", as a sudden latency spike can decide the
"win/lose" ratio for a player. companies that compete in the lucrative
cloud gaming market make significant infrastructure investments, such
as buiding entire datacenters closer to their users. these data
centers highlight the economic benefits that lower numbers of latency
spikes outweighs the associated deployment costs. on the other hand,
applications that are more tolerant to latency spikes can continue to
operate reasonably well through short spikes. yet even those
applications can benefit from consistently low latency depending on
usage shifts. for example, video-on-demand (vod) apps can work
reasonably well when the video is consumed linearly, but once the user
tries to "switch a channel", or to "skip ahead", the user experience
suffers unless the latency is sufficiently low.

finally, as applications continue to evolve, in-application metrics
are gaining in importance. for example, vod applications can assess
the quality of experience by application-specific metrics such as
whether the video player is able to use the highest possible
resolution, identify when the video is smooth or freezing, or other
similar metrics. application developers can then effectively use these
metrics to prioritize future work. all popular video platforms
(youtube, instagram, netflix, and others) have developed frameworks to
collect and analyze vod metrics at scale. one example is the scuba
framework used by meta {{scuba}}.

unfortunately, the in-application metrics can be challenging to use
for comparative research purposes. firstly, different applications
often use different metrics to measure the same phenomena. for
example, application a may measure the smoothness of video via "mean
time to re-buffer", while application b may rely on the "probability
of re-buffering per second" for the same purpose. a different
challenge with in-application metrics is vod is a significant source
of revenue for companies such as youtube, facebook, and netflix,
placing a proprietary incentive against exchanging the in-application
data. a final concern centers on the privacy issues resulting from
in-application metrics that accurately describe the activities and
preferences of an individual end-user.

### availability metrics

availability is simply defined as whether or not a packet can be sent
and then received by its intended recipient.  availability is naively
thought to be the simplest to measure, but is more complex when
considering that continual, instantaneous measurements would be needed
to detect the smallest of outages.  also difficult is determining the
root cause of infallibility: was the user's line down, something in
the middle of the network or was it the service with which the user
was attempting to communicate.

### capacity metrics

if the network capacity does not meet user demands, their perceived
network quality will be impacted. once the capacity meets the demands,
increasing capacity won't lead to further quality improvements.

the actual network connection capacity is determined by the equipment
and the lines along the network path, and varies throughout a day
and across multiple days. studies involving dsl lines in north america
indicate that over 30% of the dsl lines have capacity metrics that
vary by more than 10% throughout the day and accross multiple days.

some factors that affect the actual capacity are:

1. presence of competing traffic, either in the lan or wan
   environments. in the lan setting, the competing traffic reflects
   the multiple devices that share an internet connection. in the wan
   setting, the competing traffic often originates from the unrelated
   network flows that happen to share the same network path.
2. capabilities of the equipment along a path of the network
   connection also affects the paths capacity, including the data
   transfer rate and the amount of memory used for buffering.
3. active traffic capacity management measures, such as traffic
   shapers and policers that are often used by the network providers,
   shape a paths capacity.

there are other factors that can also negatively affect the actual
line capacities.  user application demands of the traffic follow the
usage patterns and preferences of the particular users. for example,
large data transfers can use any available capacity, while the media
streaming applicaitons require limited capacity to function
correctly. video-conferencing applications typically need less
capacity than high-definition video streaming.

### latency metrics

end-to-end latency is the time that a particular packet takes to
traverse the network path from the user to their destination and back.
the end-to-end latency comprises several components:

1. the propagation delay, which reflects the path distance and the
   individual link technologies (e.g. fibre vs satellite).
   propagation delay doesn't depend on the utilization of the network,
   when the network path remains constant.
2. the buffering delay, which reflects the time segments spend in the
   memory of the network equipment that connect the individual network
   links, as well as in the memory of the transmitting endpoint.
   buffering delay does depend on the network utilization, as well as
   on the algorithms that govern the queued segments.
3. the transport protocol delays, which can be seen in the time spent
   in retransmission and reassembly, as well as the time spent when
   a transport is "head-of-line blocked."
4. some of the workshop sumbissions have explicitly called out the
   application delay, which reflects the inefficiencies in the
   application layer itself.

traditionally, end-to-end latency is measured when the network is
idle. results of these measurements reflect mostly only the
propagation delay. this report uses the term "idle latency" to refer
to results achieved under idle network conditions.

alternatively, if the latency is measured when the network is under
its typical working conditions, the results reflect multiple types of
delays. this report uses the term "working latency" to refer to such
results. other sources use the term "latency under load" (lul) as a
synonym.

data presented at the workshop reveals a substantial difference
between the idle latency and the working latency. depending on the
traffic direciton and the technology type, the working latency is
between 6 to 25 times higher than the idle latency:

| direction | technology type | working latency | idle latency | working - idle difference | working / idle ratio |
| downstream | ftth | 148 | 10 | 138 | 15 |
| dowstream | cable | 103 | 13 | 90 | 8 |
| downstream | dsl | 194 | 10 | 184 | 19 |
| upstream | ftth | 207 | 12 | 195 | 17 |
| upstream | cable | 176 | 27 | 149 | 6 |
| upstream | dsl | 686 | 27 | 659 | 25 |

while historically the tooling available for measuring latency focused
on measuring the idle latency, there is a trend in the industry to
start measuring the working latency as well,
e.g. apple's {{networkquality}}.

<!-- missing the rpm and goodput text from pr#8 - maybe here? -->

### measurement case studies

the participants have proposed several concrete methodologies for
measuring network quality for end users.

{{paasch2021}} introduced a methodology for measuring working latency
from an end-user's vantage point. the suggested method incrementally
adds network flows between a user device and a server endpoint until
a bottleneck capacity is reached. from these measurements, a round
trip latency is measured and reported to the end-user. the authors
chose to report results with the rpm metric. the methodology had been
implemented in apple monterey os.

{{mathis2021}} have applied the rpm metric to the results of more than
4 billion download tests that m-lab performed in 2010-2021. during
this time frame, the m-lab measurement platform underwent several
upgrades which allowed the research team to compare the effect of
different tcp Congestion Control Algorithms (CCAs) on the measured
end-to-end latency. the study showed that the use cubic cca leads to
increased working latency, which is attributed to its use of larger
queues.

{{schlinker2019}} presented a large-scale study that aimed to
establish a correlation between goodput and quality of experience on a
large social network. the authors performed the measurements at
multiple data centers from which video segments of set sizes were
streamed to a large number of end users. the authors used the goodput
and throughput metrics to determine whether particular paths were
congested.

{{Reed2021}} presented the analysis of working latency measurements
collected as part of the FCC's "Measuring Broadband America" (MBA)
program. The FCC does not include working latency in its yearly report,
but does offer it in the raw data files. The authors used a
subset of the raw data to identify important differences in the
working latencies across different ISPs.

{{MacMillian2021}} presented analysis of working latency across
multiple service tiers. They found that, unsurprisingly, "premium"
tier users experienced lower working latency compared to a "value"
tier. The data demonstrated that working latency varies significantly
within each tier; one possible explanation is the difference in
equipment deployed in the homes.

These studies have stressed the importance of measurement of working
latency. At the time of this report, many home router manufacturers
rely on hardware-accelerated routing which used FIFO queues. Focusing
on measuring the working latency measurements on these devices, and
making the consumer aware of the effect of chosing one manufacturer
vs. another, can help improving the home router situation. The ideal
test would be able to identify the working latency, and to pinpoint to
the source of delay (home router, ISP, server side, or some network
node in between).

Another source of high working latency comes from network routers
exposed to cross-traffic. As {{Schlinker2019}} indicated, these can
become saturated during the peak hours of the day. Systematic testing
of the working latency in routers under load can help improve both our
understanding of latency and the impact of deployed infrastructure.

### Metrics Key Points {#discussions-metrics-key-points}


The metrics for network quality can be roughly grouped into:

1. Availability metrics, which indicate whether the user can access
   the network at all.
2. Capacity metrics, which indicate whether the actual line capacity is
   sufficient to meet the user's demands.
3. Latency metrics, indicating if the user gets the data in a timely fashion.
4. Higher-order metrics, which include both the network metrics, such as
   inter-packet arrival time, and the applicaiton metrics, such as the mean
   time between rebuffering for video streaming.

The availabiltiy metrics can be seen as derivative of either the capacity (zero
capacity leading to zero availability) or the latency (infinite latency
leading to zero availability).

Key points from the presentations and discussions included:

1. Availability and capacity are "hygienic factors" - unless an
   application is capable of using extra capacity, end-users will see
   little benefit from using overprovisioned lines.
3. Working latency has stronger correlation with user experience
   than latency under an idle network load. Working latency can
   exceed the idle latency by order of magnitude.
4. The RPM metric is a stable metric, with positive values being
   better, that may be more effective when communicating latency to
   end-users.
5. The relationship between throughput and goodput can be effective in
   finding the saturation points, both in client-side {{Paasch2021}}
   and server-side {{Schlinker2019}} settings.
6. Working latency depends on algorithm choice for addressing endpoint
   congestion control and router queuing.

Finally, it was commonly agreed to that the best metrics are those
that are actionable.

## Cross-layer Considerations {#discussions-cross-layer}

In the Cross-layer segment of the workshop, participants presented
material on and discussed how to accurately measure exactly where
problems occur.  Discussion centered especially on the differences
between physically wired and wireless connections and the difficulties
of accurately determining problem spots when multiple different types
of network segments are responsible for the quality.  As an example,
{{Kerpez2021}} showed that limited bandwidth of 2.4Ghz wifi is the
most frequently the bottleneck. In comparison, the wider bandwidth of
the 5Ghz WiFi have only been the bottleneck in 20% of observations.

The participants agreed that no single component of a network
connection has all the data required to measure the effects of the
network performance on the quality of the end user experience.

- Applications that are running on the end-user devices have the best
  insight into their respective performance, but have limited
  visibility into the behavior of the network itself, and are unable
  to act based on their limited perspective.
- Internet service providers have good insight into QoS
  considerations, but are not able to infer the effect of the QoS
  metrics on the quality of end user experiences.
- Content providers have good insight into the aggregated behavior of
  the end users, but lack the insight on what aspects of network
  performance are leading indicators of user behavior.

The workshop had identified the need for a standard and extensible way
to exchange network performance characteristics. Such an exchange
standard should address (at least) the following:

- A scalable way to capture the performance of multiple (potentially
  thousands of) endpoints.
- The data exchange format should prevent data manipulation, so that
  the different participants won't be able to game the mechanisms.
- Preservation of end-user privacy. In particular, federated learning
  approaches should be preferred so no centralized entity has the
  access to the whole picture.
- A transparent model for giving the different actors on a network
  connection an incentive to share the performance data they collect.
- An accompanying set of tools to analyze the data is needed as well.

### Separation of Concerns

Commonly, there's a tight coupling between collecting performance
metrics, interpreting those metrics, and and acting upon the
interpretation.  Unfortunately, such model is not the best for
successfully exchanging cross-layer data as:

- Actors that are able to collect particular performance metrics
  (e.g. the TCP RTT) do not necessarily have the context necessary for
  a meaningful interpretation.
- The actors that have the context and the computational/storage
  capacity to interpret metrics do not necessarily have the ability to
  control the behavior of network / application.
- The actors that can control the behavior of networks and/or
  applications typically do not have access to complete measurement
  data.

The participants agreed that it is important to separate the above
three aspects, so that:

- The different actors that have the data but not the ability to
  interpret and/or act upon it should publish their measured data.
- The actors that have the expertise in interpreting and synthesizing
  performance data should publish the results of their interpretations.

### Security and Privacy Considerations

Preserving the privacy of Internet end users is a difficult
requirement to meet when addressing this problem space. There is an
intrinsic trade-off between collecting more data about user
activities, and infringing their privacy while doing so.
Participants agreed that observability across multiple layers is
necessary for an accurate measurement of the network quality, but
doing so in a way that minimizes privacy leakage is an open question.

### Metric Measurement Considerations

- The following TCP protocol metrics have been found to be effective
  and are available for passive measurement:
    - TCP connection latency measured using SACK/ACK timing, as well as
      the timing between TCP retransmission events, are good proxies for
      end-to-end RTT measurements.
    - On the Linux platform, the tcp_info structure is the de-facto
      standard for an application to inspect the performance of
      kernel-space networking. However, there is no equivalent
      de-facto standard for the user-space networking.
- The QUIC and MASQUE protocols make passive performance measurements
  more challenging.
    - An approach that uses federated measurement / hierarchical
      aggregation may be more valuable for these protocols.
    - The QLOG format seems to be the most mature candidate for such
      an exchange.

### Towards Improving Future Cross-layer Observability {#discussions-cross-observability}

The ownership of the Internet is spread across multiple administrative
domains, making measurement of end-to-end performance data
difficult. Furthermore, the immense scale of the Internet makes
aggregation and analysis of this difficult. {{Marx2021}} presented a
simple logging format that could potentially be used to collect and
aggregate data from different layers.

Another aspect of cross-layer collaboration hampering measurement is
that the majority of current algorithms do not explicitly provide
performance data that can be used in cross-layer analysis. The IETF
community could be more diligent in identifying each protocol's key
performance indicators, and exposing them as part of the protocol
specification.

Despite all these challenges, it should still be possible to perform
limited-scope studies in order to have a better understanding of how
user quality is affected by the interaction of the different
components that constitute the Internet. Furthermore, recent
development of federated learning algorithms suggests that it might be
possible to perform cross-layer performance measurements while
preserving user privacy.

### Efficient Collaboration Between Hardware and Transport Protocols {#discussions-cross-layer-hw-tp}

With the advent of the low latency, low loss and scalable throughput
(L4S) congestion notification and control, there is an even higher
need for the transport protocols and the underlying hardware to work
in unison.

At the time of the workshop, the typical home router uses a single
FIFO queue, large enough to allow amortizing the lower-layer header
overhead across multiple transport PDUs. These designs worked well
with the Cubic congestion control algorithm, yet the newer generation
of CCAs can operate on much smaller queues. To fully support latencies
less than 1ms, the home router needs to work efficiently on sequential
transmissions of just a few segments vs. being optimized for large
packet bursts.

Another design trait common in home routers is the use of packet
aggregation to further amortize the overhead added by the lower-layer
headers.  Specifically, multiple IP datagrams are combined into a
single, large tranfer frame. However, this aggregation can add up to
10ms to the packet sojourn delay.

Following the famous "you can't improve what you don't measure" adage,
it is important to expose these aggregation delays in a way that would
allow identifying the source of the bottlenecks, and making hardware
more suitable for the next generation transport protocols.

### Cross-Layer Key Points {#cross-layer-keypoints}

- Significant differences exist in the characteristics of metrics to
  measured and required optimizations needed in wireless vs wired
  networks.
- Identification of an issue's root-cause is hampered by the
  challenges in measuring multi-segment network paths.
- No single component of a network connection has all the data
  required to measure the effects of the complete network performance
  on the quality of the end user experience.
- Actionable results require both proper collection and interpretation.
- Coordination among network providers is important to successful
  improve measurement of end user experiences.
- Simultaneously providing accurate measurements while preserving
  end-user privacy is challenging.
- Passive measurements from protocol implementations may provide
  beneficial data.

## Synthesis {#synthesis}

Finally, in the Synthesis section presentations and discussions
concentrated on the next steps likely needed to make forward
progress. Of particular concern is how to bring forward measurements
that can make sense to end users trying to make subscription
decisions.

### Measurement and Metrics Considerations

One important consideration is how to make decisions and take actions
based on the metrics measured.  Measurements must be integrated with
applications in order to get true application views of congestion, as
measurements to different infrastructure or via other applications may
return incorrect results.  Congestion itself can be a temporary
problem, and mitigation strategies may need to be different depending
on whether it is expected to be a short-term or long-term phenomenon.
A significant challenge exists in measuring short-term problems,
driving the need for continuous measurements to ensure capture.  The
workshop participants debated whether an issue that goes away is a
problem or is a sign of a proper network that is self-recovering.

Important consideration must be taken when construction metrics in
order to understand the results.  Measurements can also affected by
individual packet characteristics -- different size packets have a
typically linear relationship with their delay. Resulting measurements
can be divided into a base geographical delay, a packet-size
serialization delay and a variable (noise) delay being a third delay.
Each of these sub-component delays can be different and individually
measured across each segment in a multi-hop path.  Variable delay can
also be significantly impacted by external factors, such as
bufferbloat, routing changes, network load sharing, and other local or
remote.  Network measurements, especially load-specific tests, must
also be run long enough to ensure capture of any problems associated
with buffering, queuing, etc.  Measurement technologies should also
distinguish between upsteam and downstream measurements, as well as
measure the difference between end-to-end path and subpath
measurements.

### End-User metrics presentation

Determining end-user needs requires informative measurements and
metrics.  How do we provide the users with the service they need or
want? Is it possible for users to even voice their desires
effectively?  Only high-level, simplistic answers like "reliability",
"capacity", and "service bundling" are typical answers given in
end-user surveys.  Technical requirements operators can consume, like
"low-latency" and "congestion avoidance", are not terms known to and
used by end-users.

Example metrics useful to end users might include the number of users
supported by a service, and the number of applications or streams that
a network can support.  An example solution to combat netwokring
issues include incentive-based traffic management strategies
(e.g. requesting lower latency may also mean accepting lower
bandwidth).  User perceived latency must be considered, not just
netwokr latency -- users experience in-application to in-server
latency, and measurements network to network measurements may only be
studying the lowest level latency.  Thus, picking the right protocol
to use in a measurement is critical in order to match user experience
(for example, users do not transmit data over ICMP).

In-application measurements should consider how to measure different
types of applications, such as video streaming, file sharing,
multi-user gaming, and real-time voice communications.  It may be that
asking users for what tradeoffs they are willing to accept would be a
helpful approach: would they rather have a network with low latency,
or a network with higher bandwidth.  Gamers may make different
decisions than home office or content producers, for example.

Furthermore, how can users make these trade-offs in a fair manner that
does not impact other users? There is a tension between solutions in
this space vs the cost associated with solving these solutions, and
which customers are willing to front these improvement costs.

Challenges in providing higher-priority traffic to users centers
around the ability for networks to be willing to listen to client
requests for higher incentives, when commercial interests may not flow
to them without a cost incentive.  Shared mediums in general are
subject to oversubscribing such that the number of users a network can
support is either accurate on an underutilized network, or may assume
an average bandwidth or other usage metric that fails to account for
utilization spikes.  Individual metrics are also affected by in-home
devices from cheap routers to microwaves and from (multi-)user
behaviors during tests.  Thus, a single metric alone or a single
reading without context may not be useful in assisting a user or
operator where the problem source actually is.

User comprehension of a network remains a challenging problem.
Multiple workshop participants argued for a single number (calculated
with weighted aggregation formual), or a small number of measurements
per expected usage (a "gaming" score vs a "content producer" score).
Many users may instead prefer to consume simplified or color-coded
ratings (good/better/best, red/yellow/green, or bronze/gold/platinum).

### Synthesis Key Points

- Some proposed metrics:
    - Round-trips Per Minute (RPMs)
    - Users per network
    - Latency
    - 99% latency and bandwidth
- Median and mean measurements are distractions from the real problems.
- Shared network usage greatly affect quality
- Long measurements are needed to capture all facets of potential
  network bottlenecks.
- Better funded research in all these areas is needed for progress
- End-users will best understand a simplified score or ranking system

# Conclusions {#conclusions}

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
    Jari Arkko
    Praveen Balasubramanian
    Olivier Bonaventure
    Djamel Bousaber
    Bob Briscoe
    Rich Brown
    Anna Brunstrom
    Pedro Casas
    Vint Cerf
    Stuart Cheshire
    Kenjiro Cho
    Steve Christianson
    John Cioffi
    Alexander Clemm
    Luis M. Contreras
    Sam Crawford
    Neil Davies
    Gino Dion
    Toerless Eckert
    Lars Eggert
    Joachim Fabini
    Gorry Fairhurst
    Nick Feamster
    Mat Ford
    Jonathan Foulkes
    Jim Gettys
    Rajat Ghai
    Vidhi Goel
    Wes Hardaker
    Joris Herbots
    Geoff Huston
    Toke Høiland-Jørgensen
    Jana Iyengar
    Cullen Jennings
    Ken Kerpez
    Evgeny Khorov
    Kalevi Kilkki
    Joon Kim
    Zhenbin Li
    Mikhail Liubogoshchev
    Jason Livingood
    Kyle MacMillan
    Sharat Madanapalli
    Vesna Manojlovic
    Robin Marx
    Matt Mathis
    Jared Mauch
    Kristen McIntyre
    Randall Meyer
    François Michel
    Greg Mirsky
    Cindy Morgan
    Al Morton
    Szilveszter Nadas
    Kathleen Nichols
    Lai Yi Ohlsen
    Christoph Paasch
    Lucas Pardue
    Tommy Pauly
    Levi Perigo
    David Reed
    Alvaro Retana
    Roberto
    Koen De Schepper
    David Schinazi
    Brandon Schlinker
    Eve Schooler
    Satadal Sengupta
    Jinous Shafiei
    Shapelez
    Omer Shapira
    Dan Siemon
    Vijay Sivaraman
    Karthik Sundaresan
    Dave Taht
    Rick Taylor
    Bjørn Ivar Teigen
    Nicolas Tessares
    Peter Thompson
    Balazs Varga
    Bren Tully Walsh
    Michael Welzl
    Greg White
    Russ White
    Keith Winstein
    Lisong Xu
    Jiankang Yao
    Gavin Young
    Mingrui Zhang

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

    Erik Auerswald
    Simon Leinen
    Brian Trammell

## Workshop Chairs

The workshop chairs consisted of:

    Wes Hardaker
    Evgeny Khorov
    Omer Shapira

## Program Committee

The program committee consisted of:

    Jari Arkko
    Olivier Bonaventure
    Vint Cerf
    Stuart Cheshire
    Sam Crowford
    Nick Feamster
    Jim Gettys
    Toke Hoiland-Jorgensen
    Geoff Huston
    Cullen Jennings
    Katarzyna Kosek-Szott
    Mirja Kuehlewind
    Jason Livingood
    Matt Mathis
    Randall Meyer
    Kathleen Nichols
    Christoph Paasch
    Tommy Pauly
    Greg White
    Keith Winstein

# Github Version of this document

While this document is under development, it can be viewed and tracked
here:

https://github.com/intarchboard/network-quality-workshop-report

