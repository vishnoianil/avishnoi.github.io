---
layout: post
title: "Providing replication and fail-over as a network service in data centers"
date: "2014-12-02"
tags: "Network-based-replication, service-replication, distributed-replication, OpenFlow, SDN"
comments: true
permalink: 2014/12/ncp-patent
download: https://docs.google.com/viewer?url=patentimages.storage.googleapis.com/pdfs/US8904224.pdf
inventors:
- Anilkumar Vishnoi
- Kalapriya Kannan
- Ravi Kothari
- Shivkumar Kalyanaraman
- Vijay Mann
type: Patent
grant-date: "2014-12-02"
publication-number: US8904224 B2
application-date:
application-number: US20140025986 A1
related-paper: "2013/05/crossroads"
---

Techniques for providing session level replication and fail-over as a network service include generating a replication rule that replicates network traffic destined for a primary server from an originating server to a network controller and installing said rule in a switch component, identifying flows from the originating server to the primary server, replicating each incoming data packet intended for the primary server to the network controller for replication and forwarding to replica servers, determining said primary server to be in a failed state based on a number of retransmissions of a packet, to selecting one of the replica servers as a fail-over target, and performing a connection level fail-over by installing a redirection flow in the switch component that redirects all packets destined to the primary server to the network controller, which forwards the packets to the replica server and forwards each response from the replica server to said originating server.
