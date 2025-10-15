---
title: "urunc v0.5.0 Released: More Unikernel Power, Now K8s-Native!"
date: 2025-04-10
draft: false
tags: ['news']
authors: ['']
---

<figure>
        <img src="images/urunc-logo.png#floatright" alt="" />
        <img src="images/k8s-logo.png#floatright" alt="" />
</figure>

The `urunc` team is excited to announce the release of `urunc` v0.5.0, a major
step forward in our mission to make unikernel-based deployments seamless,
secure, and cloud-native. This release expands `urunc`’s capabilities across
containerized and orchestrated environments, with powerful new features,
enhanced monitor control, and expanded compatibility.

#### What’s New in v0.5.0

###### Namespace & Compatibility Enhancements
Full namespace support (except user namespaces) unlocks broader container and
runtime integrations. MirageOS support brings OCaml-based unikernels into the
fold, expanding Urunc’s reach across the unikernel ecosystem.

###### Kubernetes-First Deployments

`urunc_deploy` introduced for one-command installation and configuration in
existing Kubernetes clusters. Non-root monitor execution now supported,
enhancing security and compliance for enterprise-grade environments.

###### Smarter Monitor Interface

A revamped monitor interface introduces specialized CLI hooks:

- `MonitorBlockCli()` for block device options
- `MonitorNetCli()` for network-specific flags
- `MonitorCli()` for general monitor options

Monitors now spawn directly from the container’s root filesystem.


###### Cloud-Native Integrations 
Fixes for Knative readiness probes and improvements to devmapper/rootfs
handling ensure tighter integration with serverless platforms and container
runtimes.

###### CI/CD, Docs & Developer Experience

Go updated to v1.24.1, introduced End-to-end testing powered by Incus,
replacing legacy VM spawning.  CI enhancements include warning handling during
container ops and a cleanup workflow for stale issues/PRs.

###### Documentation improvements include:

Updated Kubernetes YAML examples, added new tutorials for EKS and Knative, and expanded examples on unikernel packaging

##### Read the Full Changelog
[View on GitHub](https://github.com/nubificus/urunc/compare/v0.4.0...v0.5.0)

##### Hands-on! 

- [`urunc` in k8s](https://urunc.io/tutorials/How-to-urunc-on-k8s)
- [Knative & `urunc`](https://urunc.io/tutorials/knative/)
- [`urunc` on EKS](https://urunc.io/tutorials/eks-tutorial)

`urunc` continues to push the boundaries of lightweight virtualization,
bringing the benefits of unikernels to modern cloud-native environments. With
v0.5.0, we're building the foundation for secure, performant, and flexible
infrastructure at scale.

For more information, tutorials, and community links, visit: [https://urunc.io](https://urunc.io)

Contact:

- info@urunc.io
- GitHub: [github.com/nubificus/urunc](https://github.com/nubificus/urunc)
