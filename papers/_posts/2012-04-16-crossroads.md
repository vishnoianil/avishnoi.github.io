---
layout: post
title: "CrossRoads: Seamless VM mobility across data centers through software defined networking"
date: "2012-04-16"
tags: "Online VM Migration, OpenFlow, SDN"
comments: true
permalink: 2012/04/crossroads
download: http://ieeexplore.ieee.org/document/6211886/
authors:
- Vijay Mann
- Anilkumar Vishnoi
- Kalapriya Kannan
- Shivkumar Kalyanaraman
type: Research Paper
conference: "IEEE NOMS 2012"
---

Most enterprises today run their applications on virtual machines (VMs). VM mobility - both live and offline, can provide enormous flexibility and also bring down OPEX (Operational Expenditure) costs. However, both live and offline migration of VMs is still limited to within a local network because of the complexities associated with cross subnet live and offline migration. These complexities mainly arise from the hierarchical addressing used by various layer 3 routing protocols. For cross data center VM mobility, virtualization vendors require that the network configuration of the new data center where a VM migrates must be similar to that of the old data center. This severely restricts wide spread use of VM migration across data center networks. For offline migration, the above limitations can be overcome by reconfiguring IP addresses for the migrated VMs. However, even this effort is non-trivial and time consuming as these IP addresses are embedded in various configuration files inside these VMs. As enterprises grow and new data centers emerge in different geographic locations, there is a need to interconnect these data centers in a way that allows seamless VM mobility.

In this context, we present CrossRoads - a network fabric that provides layer agnostic and seamless live and offline VM mobility across multiple data centers. We leverage software defined networking and implement an OpenFlow based prototype of CrossRoads. CrossRoads extends the idea of location independence based on pseudo addresses proposed in recent research to work with a control plane overlay of OpenFlow network controllers in various data centers. We evaluate CrossRoads on an innovative testbed that leverages nested virtualization to emulate two data centers. Our results confirm that CrossRoads has negligible performance overhead as compared to a Default layer 2 network - its average performance was no worse than 2.3% as compared to Default fabric across all experiments. In some experiments, it even outperformed the Default by up to 30%.
