---
title: Choosing the right VM for microservices in the Cloud
date: "2019-08-02T09:25:06Z"
template: "post"
draft: false
slug: "/posts/choosing-right-vm-type-for-deployment/"
category: "Microservice"
tags:
  - "Kubernetes"
  - "Google Cloud"
  - "Microservices"
  - "Deployment"
description: "This article describes how to choose cloud Virtual Machines(VM) type for microservices"
---

For cloud hosting, there are lots of vendors available and each provides a similar set of offerings with different names. To name a few Azure, AWS, Google Cloud, IBM cloud, etc., but the core concept of resources offered among the vendors are the same. Apart from CPU core counts, RAM size, storage; you also need to decide the type of machine going to use. Choosing the right type of machine involves assessing what you're deploying in the VM. For example, 
* An in-memory database can use a memory-optimized VM
* A web service that does a lot of computations like cryptography, image editing can use a VM optimized for computation.

Refer the guidelines and example use-cases given by each vendor for more details
* [Google Cloud](https://cloud.google.com/compute/docs/machine-types#determining_a_machine_type_for_your_workload)
* [Azure](https://azure.microsoft.com/en-in/pricing/details/virtual-machines/series/)
* [Amazon](https://aws.amazon.com/ec2/instance-types/)