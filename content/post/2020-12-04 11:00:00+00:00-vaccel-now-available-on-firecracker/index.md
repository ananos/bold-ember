---
title: "vAccel now available on Firecracker"
date: 2020-12-04 11:00:00+00:00
draft: false
tags: ['news']
authors: ['']
---

Today, Nubificus LTD introduced [vAccel][1] support on [AWS Firecracker][2],
opening the door for enabling hardware acceleration for serverless computing. 

With a slim design and precise abstractions, [vAccel][3] semantically exposes
hardware acceleration features to users with little to no knoweldge of software
acceleration framework internals.

Serverless computing workflows are now able to enjoy compute-offload mechanisms
to provide AI/ML services as functions, triggered thousands or millions of
times by events, on-demand, auto-scaling to multiple physical and virtual
nodes.                                     

The core of vAccel is the runtime system, essentially a library, that
translates complicated compute frameworks to meaningful functions that users
can directly call. These frameworks, commonly used on hardware accelerators,
such as TensorRT, Tensorflow, Jetson-inference, or even lower-level
abstractions such as CUDA, OpenCL, OpenACC, are now easily usable by the
end-user via vAccel. Moreover, vAccel offers a virtualization backend,
facilitating the execution of functions on Virtual Machines. Apart from support
for AWS Firecracker, [QEMU/KVM support][1] is also availabe.

End-users can get a sneak peek at what vAccel on AWS Firecracker has to offer
on the project's [website][4], on [github][5], or on-prem, by using the
distributed binaries, or just a container image. To get started, follow one of
the tutorials currently available at https://blog.cloudkernels.net

[1]: https://blog.cloudkernels.net/posts/vaccel
[2]: https://firecracker-microvm.github.io/
[3]: https://blog.cloudkernels.net/posts/vaccel
[4]: https://vaccel.org
[5]: https://github.com/cloudkernels/vaccelrt
