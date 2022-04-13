---
title:  "Find VIP of an application and DNS of server in windows"
categories:
  - Blog
date:   2022-04-13 14:25:00 -0500
author: Vignesh
tags: 
  - programming
  - infra
---

NSLookup in windows will not work right, particularly in scenarios where DNS refresh has taken place. To better identify DNS with TTL and other details, use the below commands.

`ipconfig /displaydns > output.log` (within the server box)

If you need only DNS details, use below:
`tracert esb.genpt.net` (within the server box)

To identif VIP of an application, use the below

`tracert example.com` (outside the server box)
