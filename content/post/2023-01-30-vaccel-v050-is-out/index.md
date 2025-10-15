---
title: "vAccel v0.5.0 is out!"
date: 2023-01-30
draft: false
tags: ['news']
authors: ['']
---

<figure>
        <img src="images/vaccel-logo_draft.svg#floatright" alt="" style="floatleft;" />
</figure>

Nubificus LTD proudly presents the latest release of the vAccel framework.
vAccel v0.5.0 is available as a [tar
bundle](https://github.com/cloudkernels/vaccel/releases/tag/v0.5.0) for `x86_64`
and `aarch64` architectures, with the essential binaries for users to get started.

Additionally, the individual components are packaged as binary artifacts or `deb`
packages for users to install them directly. For a list of the binary
components please visit vAccel's [documentation
page](https://docs.vaccel.org/binaries#binaries). The core vAccel library is
open-source, available on [github](https://github.com/cloudkernels/vaccelrt).

#### vAccel

vAccel enables workloads to enjoy hardware acceleration while running on
environments that do not have direct (physical) access to acceleration devices.
With a slim design and precise abstractions, [vAccel](https://vaccel.org)
semantically exposes hardware acceleration features to users with little to no
knoweldge of software acceleration framework internals.

<figure>
        <img src="images/kata-logo.png#floatleft" alt="" />
</figure>

vAccel integrates with container runtimes such as
[kata-containers](https://katacontainers.io). v0.5.0 brings updated support for
kata-containers v3.0, so deploying an application that requires hardware
acceleration in a sandboxed container in [k8s](https://kubernetes.io) is now
possible without complicated hardware setups! 

<figure>
        <img src="images/unikraft-u.svg#floatright" alt="" />
</figure>

A subset of vAccel's API is also integrated with Unikernel frameworks such as
[Unikraft](https://unikraft.org). See the [relevant
documentation](https://docs.vaccel.org/unikernels/unikernels) for more information on how
to get started!


Serverless computing workflows are now able to enjoy compute-offload mechanisms
to provide AI/ML services as functions, triggered thousands or millions of
times by events, on-demand, auto-scaling to multiple physical and virtual
nodes, without the need to directly attach a hardware device to the instance.
This functionality is enabled through vAccel's virtualization backends,
enabling the execution of hardware-accelerated functions on Virtual Machines.
Support for numerous hypervisors is available, including [AWS
Firecracker](https://firecracker-microvm.github.io/),
[QEMU/KVM](https://github.com/qemu/qemu), [Cloud
Hypervisor](https://www.cloudhypervisor.org/), etc.  See the [relevant
documentation](https://docs.vaccel.org/vm-example) on how to run an example on
a VM.

vAccel v0.5.0 offers enhanced API remoting functionality over generic sockets,
supporting `AF_VSOCK` and `AF_INET`, enabling local (intra-node) and remote
execution over the network. Optimized `AF_VSOCK` support is also offered using
the `virtio-vsock` backend on QEMU/KVM, AWS Firecracker, Cloud hypervisor,
Dragonball and any other hypervisor that supports `virtio-vsock`.

This iteration's update also contains important bug fixes and performance
optimizations.

The roadmap for v0.6.0 contains PyTorch support (currently under development).

End-users can get a sneak peek at what vAccel has to offer on the project's
[website](https://vaccel.org), on
[github](https://github.com/cloudkernels/vaccelrt), or by browsing through the available
[documentation](https://docs.vaccel.org). To get started, follow the
[Quickstart guide](https://docs.vaccel.org/quickstart).
