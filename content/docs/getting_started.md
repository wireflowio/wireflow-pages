---
title: Getting Started
weight: 1
---
# Introduction to Wireflow
Wireflow's goal is to make it easy for anyone to create and share own private network. It provides a simple and intuitive interface for managing WireGuard VPNs within Kubernetes environments.

# Getting Started with Wireflow
Welcome to Wireflow! This guide will help you get started with installing and using Wireflow on various platforms.

## Prerequisites
Before you begin, ensure you have the following prerequisites:
- A Kubernetes cluster (version 1.20 or higher) OR k3s cluster
- kubectl command-line tool installed
- Access to a terminal or command prompt

## Installation Steps
Follow these steps to starting using Wireflow:
1. **Install Control Plane**: You can install Wireflow using serval ways or by applying the provided YAML manifests. For Helm installation, run:
   ```bash
   helm repo add wireflow https://wireflowio.github.io/helm-charts
   helm install kubeflow wireflowio/wireflow
   ```
   For YAML installation, run:
   ```bash
   kubectl apply -f https://raw.githubusercontent.com/wireflow/wireflow/main/deploy/wireflow.yaml
   ```  
2. **Access the Wireflow Dashboard**: Once installed, you can access the Wireflow dashboard to manage your VPNs. Use port forwarding to access the dashboard:
   ```bash
   kubectl port-forward svc/wireflow-dashboard 8080:80
    ```
    Then, open your web browser and navigate to `http://localhost:8080`.
3. **Create a New VPN Network**: In the Wireflow dashboard, you can create a new VPN network by following the on-screen instructions. You can add peers, configure settings, and manage your VPN easily through the UI. or use the CLI tool:
   ```bash
   wireflow-cli create-network --name my-vpn
   ```
4. **Connect Peers**: Add peers to your VPN network by generating configuration files and distributing them to your devices. You can do this through the dashboard or using the CLI:
   ```bash
   wireflow-cli add-peer --network my-vpn --peer-name peer1
   ```
5. **Monitor and Manage**: Use the Wireflow dashboard to monitor the status of your VPN network, view connected peers, and manage configurations as needed.
6. **Documentation and Support**: For more detailed information, refer to the [Wireflow Documentation](https://wireflowio.com/docs). If you encounter any issues or have questions, feel free to reach out to the Wireflow community or support channels.
7. **Uninstallation**: If you need to uninstall Wireflow, you can do so by running:
   ```bash
   helm uninstall wireflow
   ```
   or if you used the YAML method:
   ```bash
   kubectl delete -f https://raw.githubusercontent.com/wireflow/wireflow/main/deploy/wireflow.yaml
   ```
Congratulations! You have successfully set up Wireflow Control Plane and created your first VPN network. 

## Install wireflow
Now you have the control plane running, you can install the `wireflow` CLI tool to manage your VPNs from the command line. Follow the instructions in the [CLI Installation Guide](https://wireflowio.com/docs/cli-installation) to download and set up the `wireflow` tool on your local machine.

## Building from Source
If you prefer to build Wireflow from source, follow these steps:
1. Clone the Wireflow repository:
   ```bash
   git clone https://github.com/wireflow/wireflow.git
   ```
2. Change into the Wireflow directory:
   ```bash
   cd wireflow
   ```
3. Build the project:
   ```bash
   make build
   ```
4. Install the Wireflow CLI tool:
   ```bash
   make install
   ```
5. Verify the installation:
   ```bash
   wireflow --version
   ```  

You are now ready to use Wireflow! For more information on advanced configurations and features, refer to the [Wireflow Documentation](https://wireflowio.com/docs).

## Using Wireflow
Once you have Wireflow installed which as data plane , now you can enjoy the benefits of a simplified VPN management experience. Use the Wireflow CLI tool to create, manage, and monitor your VPN networks directly from the command line.

For detailed usage instructions and examples, refer to the [Wireflow User Guide](https://wireflowio.com/docs/user-guide).

Happy networking with Wireflow!