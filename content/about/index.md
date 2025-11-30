# About Wireflow

## Rethinking Networking in the Cloud-Native Era

The fundamental vision behind Wireflow is simple: Networking must be a first-class citizen in the Kubernetes ecosystem.

Traditional VPNs, network gateways, and manual key management scripts clash fundamentally with the core philosophy of Kubernetes—automation, reconciliation, and declarative state.

We built Wireflow to eliminate the complexity of secure inter-cluster and node-to-node communication, allowing you to manage your global overlay network using familiar Kubernetes APIs. With Wireflow, you don't configure steps; you declare your desired network state.

## Our Origin Story: Automating the Impossible

We chose to combine two industry-leading technologies to solve a persistent infrastructure pain point:

- WireGuard: For its minimalist, kernel-level implementation, offering superior performance, speed, and modern cryptography unmatched by older VPN protocols.

- Kubernetes Operator Pattern: For its ability to continuously observe and adjust reality to match the desired state, ensuring zero-drift in your network topology.

Wireflow is designed for SREs and Platform Engineers who demand automation and high security, especially in dynamic, multi-cloud, and edge computing environments.

## Core Philosophy: Zero-Trust and Performance
Our design philosophy centers on security, efficiency, and scale:

- Declarative Zero-Trust: Access is granted solely based on Kubernetes identity and labels. By automating key rotation and management entirely, Wireflow drastically shrinks the attack surface and enforces the principle of least privilege by default.

- Kernel-Speed Performance: Leveraging WireGuard's simplicity ensures our encrypted tunnels run with near-native throughput and minimal latency, even in demanding production environments.

- Edge-Ready Design: The Operator's lightweight footprint is purpose-built to thrive in resource-constrained environments like K3s and IoT clusters.


## Open Source Commitment
Wireflow is proudly an open source project released under the [Apache Liscense 2.0].

We believe the future of cloud infrastructure is built on open standards and community collaboration. We encourage developers, operators, and security researchers to explore the code, contribute to the roadmap, and help us make cloud-native networking truly effortless.

## Get Involved

- [Source Code](https://github.com/wireflowio/wireflow)
- [Documentation](https://wireflowio.github.io)
