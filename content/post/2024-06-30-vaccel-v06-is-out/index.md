---
title: "vAccel v0.6 is out!"
date: 2024-06-30
draft: false
tags: ['news']
authors: ['']
---

<figure>
        <img src="images/vaccel-logo_draft.svg#floatright" alt="" style="floatleft;" />
</figure>

Nubificus LTD proudly presents the latest release of the vAccel framework.
[vAccel v0.6.0](https://github.com/cloudkernels/vaccelrt/releases/tag/v0.6.0)
is available, as well as a [hot fix
followup](https://github.com/cloudkernels/vaccelrt/releases/tag/v0.6.1) for
`x86_64`, `aarch64`, and `armv7l` architectures, with the essential binaries
for users to get started.

<figure>
        <img src="images/pytorch-logo.png#floatright" alt="" />
</figure>

A major addition to our previous release is Torch support. Users are now able
to run inference on Torch models seamlessly, on local and remote targets
(CPU/GPU etc.). A short [screen cast](https://youtu.be/6VMguN9fuHA) is available
to check torch with vAccel in action!


vAccel v0.6 includes updated [helper
functions](https://github.com/cloudkernels/vaccelrt/blob/main/docs/vaccel_args.md)
for easier argument definition (`exec`), as well as enhanced CI and
[testing](https://blog.cloudkernels.net/posts/testing_post/) support.  

<figure>
        <img src="images/golang-logo.png#floatleft" height="50px" alt="" />
</figure>

A fun addition was native [`Golang` bindings](https://github.com/nubificus/go-vaccel)! Users can now natively interact with
Go programs and enjoy hardware acceleration from simple web services! `Golang`
bindings helped a lot with our Knative integration!

vAccel v0.6 offers updated API remoting functionality over generic sockets,
supporting `AF_VSOCK` and `AF_INET`, enabling local and remote
execution over the network. `AF_VSOCK` support is also updated with a streaming
optimization, to reduce the amount of memory allocated by the gRPC transport
layer.

This iteration's update also contains important bug fixes and performance
optimizations. For the list of changes, see the
[RELEASE](https://github.com/cloudkernels/vaccelrt/releases/tag/v0.6.0) notes.

The individual components are packaged as binary artifacts or `deb` packages
for users to install them directly. For a list of the binary components please
visit vAccel's [documentation page](https://docs.vaccel.org/binaries#binaries).
The core vAccel library is open-source, available on
[github](https://github.com/cloudkernels/vaccelrt).


The roadmap for v0.7 contains enhanced Torch support, `OpenCV`-native bindings, a
`C++`-based transport layer, the move to the `meson` build system, and more!


#### vAccel

vAccel enables workloads to enjoy hardware acceleration while running on
environments that do not have direct (physical) access to acceleration devices.
With a slim design and precise abstractions, [vAccel](https://vaccel.org)
semantically exposes hardware acceleration features to users with little to no
knowledge of software acceleration framework internals.

<figure>
        <img src="images/kata-logo.png#floatleft" alt="" />
</figure>

vAccel integrates with container runtimes such as
[kata-containers](https://katacontainers.io). v0.6 brings updated support for
kata-containers v3.X, both for the Go and rust runtimes, so deploying an
application that requires hardware acceleration in a sandboxed container in
[k8s](https://kubernetes.io) is now possible without complicated hardware
setups! 

Serverless computing workflows are now able to enjoy compute-offload mechanisms
to provide AI/ML services as functions, triggered thousands or millions of
times by events, on-demand, auto-scaling to multiple physical and virtual
nodes, without the need to directly attach a hardware device to the instance.
This functionality is enabled through vAccel's virtualization backends,
enabling the execution of hardware-accelerated functions on Virtual Machines.
Support for numerous hypervisors is available, including [AWS
Firecracker](https://firecracker-microvm.github.io/),
[QEMU/KVM](https://github.com/qemu/qemu), [Cloud
Hypervisor](https://www.cloudhypervisor.org/), and Dragonball, the stock
hypervisor of kata-containers! See the [relevant
documentation](https://docs.vaccel.org/vm-example) on how to run an example on
a VM.

End-users can get a sneak peek at what vAccel has to offer on the project's
[website](https://vaccel.org), on
[github](https://github.com/cloudkernels/vaccelrt), or by browsing through the available
[documentation](https://docs.vaccel.org). To get started, follow the
[Quick start guide](https://docs.vaccel.org/quickstart).
