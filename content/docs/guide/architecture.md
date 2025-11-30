## Wireflow Architecture
The wireflow architecture is designed to provide a scalable and secure solution for managing WireGuard VPNs within Kubernetes environments. It consists of several key components that work together to deliver a seamless experience for users.

## Overview
At a high level, the wireflow architecture includes the following components:
- **Control Plane**: The central management component that provides a dashboard and APIs for configuring and monitoring WireGuard VPNs.
- **Wireflow Peers**: The Data Plane for wireflow, which are individual devices managed by the control plane,  Each device is a peer that configured with a unique WireGuard configuration file that allows it to securely communicate with other peers within the VPN network.
- **DRP Server**: A component responsible for relaying traffic between Wireflow Peers.
- **Management Service**: A service that for watching and managing the Wireflow Custom Resources within the Kubernetes cluster. When changed, push updates to the peers.
- **Wireflow-cli(wfctl)**: A command-line interface for interacting with the Wireflow Control Plane. Using wfctl you can configure and manage WireGuard VPNs.

![Wireflow Architecture](/images/wireflow-architecture.png)


## Next Steps
- [Install Control Plane](/docs/guide/install/): Learn how to install the Wireflow Control Plane & Wireflow Services on your Kubernetes cluster.
- [Install Data Plane](/docs/guide/install): Learn how to install the Wireflow Peers on your own devices.

