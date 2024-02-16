---
title: HTTP request terminated at 30 seconds in Google Kubernetes Engine
date: "2019-08-21T09:21:30Z"
template: "post"
draft: false
slug: "/posts/HTTP-request-termintaed-at-30sec/"
category: "Kubernetes"
tags:
  - "Kubernetes"
  - "Google Cloud"
description: "HTTP request to services hosted in Google Kubernetes Engine terminated by 30 seconds"
---

The main cause of this issue is [Google Load Balancer default timout](https://cloud.google.com/load-balancing/docs/https/#timeouts_and_retries) value 30. 
You can solve the problem by manually increasing timeout value, using steps given here.
<br>https://cloud.google.com/load-balancing/docs/backend-service#timeout-setting

However, the best solution is to use the Kubernetes Backend config file to set the timeout for our services. 
<br>https://cloud.google.com/kubernetes-engine/docs/how-to/configure-backend-service#creating_a_backendconfig