---
title: Wireflow home
layout: hextra-home
---

{{< hextra/hero-badge >}}
  <div class="hx:w-2 hx:h-2 hx:rounded-full hx:bg-primary-400"></div>
  <span>Free, open source</span>
  {{< icon name="arrow-circle-right" attributes="height=14" >}}
{{< /hextra/hero-badge >}}

<div class="hx:mt-6 hx:mb-6">
{{< hextra/hero-headline >}}
  Kubernetes-Native WireGuard Orchestrator.&nbsp;<br class="hx:sm:block hx:hidden" />Zero-Touch Network Automation.
{{< /hextra/hero-headline >}}
</div>

<div class="hx:mb-12">
{{< hextra/hero-subtitle >}}
  Declare your network state, and eliminate manual configuration. <br class="hx:sm:block hx:hidden" />Let the Wireflow Operator handle the complexity for you.
{{< /hextra/hero-subtitle >}}
</div>


<div class="hx:mb-6">
{{< hextra/hero-button text="Get Started" link="docs" >}}
</div>


<!-- <div class="hx:mb-12">
{{< hextra/hero-subtitle >}}
  Wireflow's goal is to provide a seamless and automated way to manage WireGuard VPNs within Kubernetes environments. By leveraging Kubernetes' declarative nature, Wireflow allows users to define their desired network configurations using custom resource definitions (CRDs). The Wireflow operator then takes care of provisioning and managing the underlying WireGuard tunnels, ensuring secure and efficient connectivity between mutiple platforms. This approach simplifies the complexity of VPN management, enhances security through automation, and integrates natively with Kubernetes workflows.
{{< /hextra/hero-subtitle >}}
</div> -->

<div class="hx-mt-6 hx-mb-6">
{{< hextra/hero-section >}}
  Using Wireflow cases
{{< /hextra/hero-section >}}
</div>

<div class="hx:mb-12">
{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="Remote Workforces"
    subtitle="Enable secure remote access for employees, contractors, and partners with ease."
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-md:min-h-[340px]"
    image="images/remote-workforces.webp"
    imageClass="hx:top-[40%] hx:left-[24px] hx:w-[180%] hx:sm:w-[110%] hx:dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="IoT & Edge Networking"
    subtitle="Securely connect and manage IoT devices and edge locations across distributed environments."
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-lg:min-h-[340px]"
    image="images/hextra-markdown.webp"
    imageClass="hx:top-[40%] hx:left-[36px] hx:w-[180%] hx:sm:w-[110%] hx:dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(142,53,74,0.15),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Multi-Cluster Connectivity"
    subtitle="Seamlessly connect and manage multiple Kubernetes clusters with ease."
    class="hx:aspect-auto hx:md:aspect-[1.1/1] hx:max-md:min-h-[340px]"
    image="images/hextra-search.webp"
    imageClass="hx:top-[40%] hx:left-[36px] hx:w-[110%] hx:sm:w-[110%] hx:dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(221,210,59,0.15),hsla(0,0%,100%,0));"
  >}}
  
  
{{< /hextra/feature-grid >}}
</div>


<div class="hx-mt-6 hx-mb-6">
{{< hextra/hero-section >}}
  Features of Wireflow
{{< /hextra/hero-section >}}
</div>

<div class="hx:mb-12">
{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="Declarative Automation"
    subtitle="Zero-Touch Network Orchestration via Kubernetes CRDs，Eliminate the overhead of manual configuration and key management.Wireflow elevates your overlay networking to a true cloud-native level."
  >}}

    {{< hextra/feature-card
    title="K8s-Native Security"
    subtitle="Wireflow is built on the principle of **Zero-Trust**. It tightly integrates with the Kubernetes identity and label system to enforce fine-grained network policies across your clusters.This level of native integration allows you to Build a truly secure, identity-aware mesh network without the complexity"
  >}}

  {{< hextra/feature-card
    title="High-Performance Overlay"
    subtitle="Zero-Touch Network Orchestration via Kubernetes CRDs，Eliminate the overhead of manual configuration and key management.Wireflow elevates your overlay networking to a true cloud-native level."
  >}}

  {{< hextra/feature-card
    title="Declarative Automation"
    subtitle="Wireflow leverages the **minimalist and highly efficient WireGuard kernel implementation** to ensure your encrypted overlay network operates at maximum speed with minimal latency.Optimized for Kubernetes"
  >}}
  
{{< /hextra/feature-grid >}}
</div>