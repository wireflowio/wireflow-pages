# wireflow Architecture
The wireflow architecture is designed to provide a scalable and secure solution for managing WireGuard VPNs within Kubernetes environments. It consists of several key components that work together to deliver a seamless experience for users.

## Overview
At a high level, the wireflow architecture includes the following components:
- **Control Plane**: The central management component that provides a dashboard and APIs for configuring and monitoring WireGuard VPNs.
- **Wireflow Peers**: The individual devices or nodes that connect to the VPN. Each peer is configured with a unique WireGuard configuration file that allows it to securely communicate with other peers within the VPN network.
- **DRP Server**: A component responsible for relaying traffic between Wireflow Peers.
- **Management Service**: A service that for watching and managing the Wireflow Custom Resources within the Kubernetes cluster. When changed, push updates to the peers.
- **

## Key Components
1. **Control Plane**: The Control Plane is the central management component of wireflow. It provides a user-friendly dashboard and APIs for configuring and monitoring WireGuard VPNs. The Control Plane leverages Kubernetes Custom Resource Definitions (CRDs) to define and manage VPN configurations.
2. **Wireflow Peers**: These are the individual devices or nodes that connect to the VPN. Each peer is configured with a unique WireGuard configuration file that allows it to securely communicate with other peers within the VPN network.
