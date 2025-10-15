---
title: "FOSDEM 2024"
date: 2024-02-07
draft: false
tags: ['news']
---

<figure>
        <img src="/images/FOSDEM_venue.jpg#floatright" height="230px" alt="" style="border-radius: 10px"/>
</figure>

[FOSDEM 2024](https://fosdem.org) was a blast! Our team was there presenting
our work around unikernels, and their interaction with the cloud-native world.

The first presentation took place in the Containers devroom, where we described
the challenges of securing containers within VM or microVM sandboxes and the
complexities of resource optimization on physical nodes. We presented `urunc`, a
CRI-compatible container runtime spawning unikernels packaged in OCI images.
The talk highlighted `urunc`'s internals, covering hypervisor support, network
and storage handling, and integration with high-level orchestration frameworks
like Kubernetes, while also addressing network setup implications when
combining unikernels and generic containers in a k8s context.

In the Microkernel devroom, we continued our exploration of unikernels
with a focus on modularity. The team presented `bunny`, a novel build system
aimed at simplifying the Unikernel building process. `bunny` adopts a layered
approach, making use of the modular aspect of Unikernels. Each component
represents a distinct layer, eliminating the need for users to manually build
dependencies. This approach allows for the creation of minimal and specialized
Unikernel images tailored for individual applications. 

These presentations highlight our commitment to simplify and optimize
application delivery in diverse, heterogeneous infrastructure, providing
valuable insights into security and system optimization in the evolving
landscape of container technology.

Find below the slides and video recordings of the presentations, along with links to the devrooms full schedule.

- A Modular Approach to Effortless and Dependency-Aware Unikernel Building, Microkernel and Component-based OS devroom [session](https://fosdem.org/2024/schedule/event/fosdem-2024-3456-a-modular-approach-to-effortless-and-dependency-aware-unikernel-building/) [slides](https://fosdem.org/2024/events/attachments/fosdem-2024-3456-a-modular-approach-to-effortless-and-dependency-aware-unikernel-building/slides/22316/FOSDEM24-bunny_v1_Y1twYme.pdf) [video](https://live.fosdem.org/watch/ud2208) [devroom](https://fosdem.org/2024/schedule/track/microkernel/)
- From Containers to Unikernels: Navigating Integration Challenges in Cloud-Native Environments, Containers devroom [session](https://fosdem.org/2024/schedule/event/fosdem-2024-3402-from-containers-to-unikernels-navigating-integration-challenges-in-cloud-native-environments/) [slides](https://fosdem.org/2024/events/attachments/fosdem-2024-3402-from-containers-to-unikernels-navigating-integration-challenges-in-cloud-native-environments/slides/22484/FOSDEM24-urunc_8aePu2M.pdf) [video](https://live.fosdem.org/watch/ub2252a) [devroom](https://fosdem.org/2024/schedule/track/containers/)

**FOSDEM**
<figure>
        <img src="/images/FOSDEM_logo.svg.png#floatleft" height="230px" alt="" style="border-radius: 10px"/>
</figure>

FOSDEM stands for "Free and Open Source Software Developers' European Meeting."
It is one of the largest gatherings of open-source developers and enthusiasts
in the world. FOSDEM is an annual event that takes place in ULB Solbosch
Campus, Brussels, Belgium, typically in late January or early February.

The conference provides a platform for developers, contributors, and users of
free and open-source software to come together, share knowledge, collaborate on
projects, and discuss the latest developments in the open-source community.
FOSDEM is known for its diverse range of talks, developer rooms, and stands,
covering a wide array of topics related to open-source software, including
programming languages, operating systems, security, networking, and more.

FOSDEM is a free event, organized by volunteers, and it attracts participants
from around the globe. The conference aims to foster collaboration and promote
the principles of free and open-source software within the technology
community.

Although statistics are not out yet, this year, getting into the talks was
harder than ever. Rooms were filling up even 30' before the scheduled talks. As
an indication, almost 855 events are recorded and are being transcoded to be
available for online viewing. Our estimation is that there were almost 10000
people in ULB.