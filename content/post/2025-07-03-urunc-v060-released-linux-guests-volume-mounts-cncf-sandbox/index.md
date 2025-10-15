---
title: "urunc v0.6.0 Released: Linux Guests, Volume Mounts & CNCF Sandbox"
date: 2025-07-03
draft: false
tags: ['news']
---

We are thrilled to announce the release of [`urunc` v0.6.0](https://github.com/urunc-dev/urunc/releases/tag/v0.6.0), a feature-packed
update that pushes unikernel-native infrastructure even closer to everyday
container workflows. 

This release marks a major milestone:
[`urunc`](https://github.com/urunc-dev/urunc) is now an official [CNCF Sandbox
Project](https://www.cncf.io/projects/urunc/), a strong signal of our
commitment to open collaboration, cloud-native principles, and production-grade
reliability.

<figure>
        <img src="/images/urunc-logo-light.svg#floatright" width="150px" alt="" />
</figure>

This release adds support for WASM **[Mewz
unikernels](https://github.com/mewz-dev)**, and significantly, for single-app, Linux-based 
containers by [transforming them](https://github.com/nubificus/bunny) into
minimal Linux VMs. You can now:

- Pivot and execute the monitor process from a freshly created root filesystem (`chroot`)
- Share the container’s root filesystem with the guest using 9pfs
- Mount volumes into the container's rootfs
- Boot single-application, Linux-based guests, not just unikernels
- Set CLI options at runtime
- Pass environment variables into the guest

It also enhances logging and error handling, introduces more intuitive CLI
semantics, and brings a polished documentation redesign, complete with a brand
new logo and improved usability.

#### Breaking Changes

- The `useDMBlock` annotation has been **replaced** with `mountRootfs`,
  offering a **unified way** to mount the container rootfs using block devices
  or shared filesystems.
- Unikraft CLI handling now reserves `argv[0]` for consistency with
  kraftkit's behavior.

#### CI/CD & Internals

- Moved entirely to GitHub-hosted runners
- Added automated docs publishing, better license checking, and spellchecks (code & docs)
- Improved isolation and test reproducibility by removing org-wide secret dependencies
- Refactored CI workflows to facilitate external (non-org) PRs

[Full Changelog](https://github.com/urunc-dev/urunc/compare/v0.5.0...v0.6.0)

#### Docs, Governance & Community

We're especially excited about the community-building steps in this release. In
addition to technical improvements, we’ve:

<figure>
        <img src="/images/cncf-color.svg#floatright" width="350px" alt="" />
</figure>

- Introduced clear project governance
- Published a dedicated security policy
- Refreshed the `README` with:
  - Roadmap links
  - Contribution guidelines
  - OpenSSF best practices badge
  - A public [Slack channel](https://cloud-native.slack.com/archives/C08V201G35J) to join the conversation

We invite developers, researchers, and users to collaborate, share feedback,
and help shape the future of Urunc.


#### CNCF Milestone

Becoming a [CNCF Sandbox Project](https://www.cncf.io/sandbox-projects/) marks
an important milestone for `urunc`. This recognition opens up new collaboration
opportunities and validates our vision: to bring secure, low-overhead,
unikernel-native execution to cloud-native environments through familiar
interfaces and open standards.

For more information, demos, tutorials, and contribution details, visit: **https://urunc.io**

#### Try it out

- [Run Urunc in Kubernetes](https://urunc.io/tutorials/How-to-urunc-on-k8s/)
- [Use Knative with Urunc](https://urunc.io/tutorials/knative/)
- [Boot OCI Containers as VMs](https://urunc.io/tutorials/existing-container-linux/)
- [Join the Slack & Get Involved](https://urunc.io/developer-guide/)


Contact
info@urunc.io  
GitHub: [github.com/urunc-dev/urunc](https://github.com/urunc-dev/urunc)