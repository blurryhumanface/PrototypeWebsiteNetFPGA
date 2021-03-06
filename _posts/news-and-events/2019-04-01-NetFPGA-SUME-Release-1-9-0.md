---
title: NetFPGA SUME Release 1.9.0
date: 2019-04-01
eventdate: 2019-04-01
eoldate: 2021-04-01
category: news
posttype: news-and-events
---

Greetings NetFPGA community,

We are pleased to announce today the next patch release (**1.9.0**) of the NetFPGA-SUME code base.

This release includes:

**Bug Fix:**
- nf_axis_converter_v1_0_0: Fix timing issue on the path between the nf_axis_converter and the tx_queue. The timing issue was causing the nf_axis_converter output to be incorrect, which in turn caused the MAC to reject packets of certain lengths. Added an AXIS pipeline stage on the output of the nf_axis_converter

<br>
**Contrb Projects:**
- lake: Layered Key-value store, a hardware-based implementation of memcached server
- reference_emu_dns: Implementation of a DNS server with the Emu framework and integrated into the SUME reference data path
- nic_v2: Reference NIC with the new DMA engine core

<br>
**Contrib Cores:**
- db_v1_0_1: A key-value cache which stores key-value pair on DRAM and BRAM
- div_v1_0_0: A packet distributer, based on UDP port number and this module acts as in-network computing on-demand controller
- emudns_output_port_lookup_v1_0_0: Output port lookup core generated by the Emu framework with DNS functionality
- input_arbiter_6in_v1_0_0: Provides support for an additional internal high-priority 50Gbps queue
- nf_naudit_dma_v1_0_0: New DMA engine
- nf_sume_pktgen_v1_0_0: Enables internal packet injection at full speed (~50Gbps)

<br>
{% include Update-close.md %}
