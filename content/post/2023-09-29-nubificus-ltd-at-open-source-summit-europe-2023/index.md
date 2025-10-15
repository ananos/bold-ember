---
title: "Nubificus LTD at Open Source Summit Europe 2023"
date: 2023-09-29
draft: false
tags: ['news']
authors: ['']
---

<figure>
        <img src="images/oss2023.png#floatleft" alt="" style="border-radius: 10px"/>
</figure>

Sep 18th-21st we were in Bilbao, Spain for the [Open Source Summit Europe
2023](https://events.linuxfoundation.org/open-source-summit-europe/)!  We had
the opportunity to talk about open-source, meet friends, and make new ones! 

It was a pleasure for us to [present](https://osseu2023.sched.com/event/1OGgY)
our work on bringing unikernels closer to the cloud-native world! 
[Video](https://youtu.be/KokcFBRTGlM?t=12525)
[Slides](https://static.sched.com/hosted_files/osseu2023/56/OSS2023-NBFC-urunc.pdf)

In this session, we went through the options that users have to deploy
applications in Cloud & Edge environments. We talked about containers,
sandboxed containers, and unikernels, introduced our own container runtime
tailored to unikernels, and presented the integration effort we have undertaken
to allow unikernels to execute in k8s & Serverless Computing frameworks.
 
[urunc](https://github.com/nubificus/urunc) is an open-source, lightweight
container runtime that spawns unikernels as generic containers. To facilitate
the packaging of unikernels as OCI artifacts, we built
[bima](https://github.com/nubificus/bima), a tool that automates the process of
injecting unikernel binaries into container image layers and adds metadata that
are later used by urunc.

This work is supported by EU H2020 research and innovation programmes, under
Grant Agreements 101017168 (SERRANO) and 871900 (5G-COMPLETE).
