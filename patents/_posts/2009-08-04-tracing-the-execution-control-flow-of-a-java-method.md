---
layout: post
title: "Method and Appratus to trace the execution control flow of Java method"
date: "2009-08-04"
tags: "Java, Debugging, JVM, Control-flow-tracing"
comments: true
permalink: 2009/08/tracing-the-execution-control-flow-of-a-java-method
download: https://priorart.ip.com/IPCOM/000185977
inventors:
- Anilkumar Vishnoi
- Prashanth K Nageshappa
- Venkataraghavan Lakshminarayanachar,
type: Patent
grant-date: "2009-08-04"
publication-number: IPCOM000185977D (IP.com)
application-date:
application-number:
related-paper:
---

Applications comprise of methods which further comprise of control blocks (if else, while, switch etc.) that are taken or not taken at runtime depending on the runtime conditions. More often than not, while tracking specific entities like a structure variable or an Object instance, it becomes imperative to understand the following : 1) Methods which create and use the variable/instance 2) the actual Control Blocks within these methods that were traversed for creation or use of the object/variable. The above information is important to understand the specifics of what path was traversed to create and use the instance/variable - so that the debugging/diagnostics/profiling could concentrate on only those paths and narrow down the scope of analysis,thereby expediting the same.
