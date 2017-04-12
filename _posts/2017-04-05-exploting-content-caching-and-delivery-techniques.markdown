---
layout:     post
title:      "Caching in the Air"
subtitle:   "Exploiting content caching and delivery techniques for 5G systems"
date:       2017-04-05 12:00:00
author:     "Rene Midouin"
header-img: "img/caching.jpg"
---

> The demand for rich multimedia services over mobile networks has been soaring at a tremendous pace over recent years. However, due to the centralized architecture of current cellular networks, the wireless link capacity as well as the bandwidth of the radio access networks and the backhaul network cannot practically cope with the explosive growth in mobile traffic.

# Motivation of the research
Users are craving for contents and require the contents to be delivered as
fast as possible, faster before they can even say the word "momma".
# Existing approaches
When it comes to caching, all techinical issues falls in the following three
questions:
- ### Where to cache?
	- Evolve Packet Core (EPC)
		- URL Web-Based Web Caching
		- Prefix-Based Web Caching
		- Chunk-Level Redundancy Elimination
		- TCP-Level Redundancy Elimination
		- Packet-Level Redundancy Elimination
	- Radio Access Network (RAN)
		- Byte-caching

- ### What to cache?
	- Popular contents
		- Cat videos
			![image-title-here]({{ site.url }}/assets/imgs/cat.png){:class="img-responsive"}

- ### How to cache?
	- Least Frequently Used (LFU)
	- Least Recently Used (LRU)
	- First in First out (FIFO)

# New approach
Content Centric Networking (CCN) Based Caching:

In CCN, a user requests a particular content by issuing interest packets to neighbors. If the requested content can be retrieved in the caching store (CS) of any device, the content is directly delivered from the device. Otherwise, routers propagate interest towards appropriate content sources and store information for each forward- ed interest in the pending interest table (PIT).

# Performance evaluation
![image-title-here]({{ site.url }}/assets/imgs/caching-performance-evaluation.png){:class="img-responsive"}

# Conclusion and future work
- Device-2-Device
- Software Defined Network (SDN)

<br />
----
****

# Download Research Paper
<a href="http://ieeexplore.ieee.org/document/6736753/media" target="_blank">Cache in the air: exploiting content caching and delivery techniques for 5G systems</a>

# Class Presentation
<div class="responsive-wrap">
<iframe src="https://docs.google.com/presentation/d/14NaZ5CmBNt_MUU7dDTjW7qqtymfV3Rm8gA0D4gI6OP8/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</div>

