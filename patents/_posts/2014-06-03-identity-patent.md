---
layout: post
title: "Enabling co-existence of hosts or virtual machines with identical addresses"
date: "2014-06-03"
tags: "VM-Migration-across-data-centers, co-existence-of-addresses, OpenFlow, Multi-tenancy, SDN"
comments: true
permalink: 2014/06/identity-patent
download: https://docs.google.com/viewer?url=patentimages.storage.googleapis.com/pdfs/US8745196.pdf
inventors:
- Anilkumar Vishnoi
- Kalapriya Kannan
- Shivkumar Kalyanaraman
- Vijay Mann
type: Patent
grant-date: "2014-06-03"
publication-number: US8745196 B2
application-date:
application-number: US20130145008 A1
related-paper: "2012/01/identity"
---

A method for enabling co-existence of multiple machines with identical addresses within a single data center network. The method includes assigning a unique pseudo identifier to each machine in the network that can be used for routing a packet to a destination machine, replacing a sender media access control address on an address resolution protocol request with a pseudo identifier of the sender at an edge network switch, retrieving a private network identifier from a mapping table based on the sender pseudo identifier and returning a pseudo identifier for the destination address based on the private network identifier, and replacing the pseudo identifier of the destination address with an actual identifier at a destination edge network switch for routing the packet to the destination machine.
