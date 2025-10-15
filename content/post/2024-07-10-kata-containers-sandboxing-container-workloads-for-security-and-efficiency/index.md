---
title: "Kata-containers: sandboxing container workloads for security and efficiency"
date: 2024-07-10
draft: false
tags: ['news']
---

<figure>
        <img src="/images/kata-logo.png#floatleft" width="70px" alt="" />
</figure>

Anastassios Nanos delivered an insightful
[presentation](https://youtu.be/2pNo8F3AMrw?t=10654) at [OpenInfra Days
Hungary](https://oideurope2024.openinfra.dev/hungary/), in Budapest, earlier
this June, highlighting the innovative capabilities of the [Kata
Containers](https://katacontainers.io) project. The talk focused on the
project's advancements, particularly the introduction and maturity of the Rust
runtimes, alongside the go version of the runtime, and demonstrated how the
Kata team is leveraging these technologies to enhance the performance and
security of serverless workloads. As a first time Architecture Committee member
since April 2024, Dr Nanos presented the current status of the project, and how
the team at Nubificus & Nubis is using kata-containers to sandbox serverless
workloads, while exposing hardware acceleration capabilities by integrating
vAccel to the container runtime.

##### Key Highlights of the Presentation

<figure>
        <img src="/images/oidh-photo2.png#center" height="180px" alt="" style="floatright" />
</figure>

_Kata Containers Project Overview_: Dr Nanos began by providing an overview of
the Kata Containers project, an open-source initiative that integrates
lightweight virtual machines (VMs) to enhance the security and isolation of
containerized applications. He explained how Kata Containers combine the speed
and flexibility of containers with the robust security features of VMs, making
them an ideal solution for modern cloud-native applications.

<figure>
        <img src="/images/oidh-photo1.jpg#floatleft" height="180px" alt="" style="floatleft;" />
</figure>

_Go and Rust Runtimes_: A significant portion of the presentation was dedicated
to the dual support for Go and Rust runtimes within Kata Containers. Dr Nanos
detailed the journey from the initial Go runtime to the introduction of the
Rust runtime, emphasizing the performance and safety benefits of Rust. He
discussed the efforts to achieve feature parity between the two runtimes,
enabling users to choose the runtime that best suits their needs without
sacrificing functionality or performance.

_Sandboxing Serverless Workloads_: Dr Nanos illustrated how Kata Containers are
being used to [sandbox serverless
workloads](https://dl.acm.org/doi/10.1145/3642977.3652096), a growing trend in
cloud computing.  He explained that by using Kata Containers, the team can
provide strong isolation for serverless functions, ensuring that workloads are
securely sandboxed and isolated from one another. This approach not only
enhances security but also improves the reliability and stability of serverless
environments.

<figure>
        <img src="/images/vaccel-logo_draft.svg#floatright" width="180px" alt="" style="floatleft;" />
</figure>

_vAccel Integration_: One of the standout points of the talk was the
integration of [vAccel](https://docs.vaccel.org) with Kata Containers. Dr Nanos
explained how vAccel allows the exposure of hardware acceleration
functionalities to sandboxed containers, significantly boosting the performance
of compute-intensive tasks.  This integration enables developers to take full
advantage of hardware acceleration within a secure and isolated environment,
paving the way for more efficient and powerful applications.

_Looking Ahead_: Dr Nanos concluded his presentation with a look ahead to the
future of Kata Containers, including the anticipated release of [Kata
Containers 4.0](https://github.com/orgs/kata-containers/projects/43). He
highlighted ongoing efforts to further unify the Go and Rust runtimes and to
expand the project’s capabilities to meet the evolving needs of the
cloud-native ecosystem.

The presentation at OpenInfra days Hungary underscored the Kata Containers
project's commitment to innovation and security in containerized environments.
With its robust feature set and continued development, Kata Containers is
poised to play a crucial role in the future of cloud-native infrastructure.

For more information about the Kata Containers project, visit
[katacontainers.io](https://katacontainers.io). All demos presented are available online at
[github](https://github.com/nubificus/openinfradayshu-demos).

Many thanks to the [OpenInfra Foundation](https://openinfra.dev/) for hosting Dr Nanos, as well as to
[DESIRE6G](https://desire6g.eu) and [MLSysOps](https://mlsysops.eu) for
supporting the development of most of the work presented.