---
layout: post
title: "Living on the edge: Monitoring network flows at the edge in cloud data centers"
date: "2012-01-03"
tags: "Scalable-Flow-Monitoring, sFlow, NetFlow, SDN"
comments: true
permalink: 2013/01/living-on-the-edge
download: http://ieeexplore.ieee.org/document/6465540/
authors:
- Vijay Mann
- Kalapriya Kannan
- Sarvesh Bidkar
type: Research Paper
conference: "IEEE COMSNET 2013"
---

Scalable network wide flow monitoring has remained a distant dream because of the strain it puts on network router resources. Recent proposals have advocated the use of coordinated sampling or host based flow monitoring to enable a scalable network wide monitoring service. As most hosts in data centers get virtualized with the emergence of the cloud, the hypervisor on a virtualized host adds another network layer in the form of a vSwitch (virtual switch). The vSwitch now forms the new edge of the network.

In this paper, we explore the implications of enabling network wide flow monitoring inside virtual switches in the hosts. Monitoring of network flows inside the server vSwitch can enable scalability due to its distributed nature. However, assumptions that held true for flow monitoring inside a physical switch need to be revisited since vSwitches are usually not limited by the same level of resource constraints that exist for physical switches and routers. On the other hand, vSwitches do not implement flow monitoring in hardware, as it is done in some physical switches. We present the design and implementation of EMC2 - a scalable network wide monitoring service for cloud data centers. We also conduct an extensive evaluation of various switch based flow monitoring techniques and share our findings. Our results indicate that while layer-3 flow monitoring protocols such as NetFlow can give a very good network coverage without using too many resources, protocols that sample packet headers (such as sFlow) need to be carefully configured. A badly configured sFlow vSwitch can degrade application network throughput by up to 17% and can also choke the management network by generating monitoring data at a very high rate.
