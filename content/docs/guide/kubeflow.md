# What is Wireflow Control Plane?
Wireflow Control Plane is the central management component of Wireflow, a solution designed to simplify the deployment and management of WireGuard VPNs within Kubernetes environments. It provides a user-friendly interface and aPI for configuring and monitoring WireGuard VPNs, making it easier for users to create and manage secure private networks.

# Features of Wireflow Control Plane
  - **Kubernetes-Native CRDS**: Wireflow Control Plane leverages Kubernetes Custom Resource Definitions (CRDs) to define and manage WireGuard VPN configurations, allowing seamless integration with Kubernetes-native tools and workflows.
  - **User-Friendly Dashboard**: It includes a web-based dashboard that provides an intuitive interface
  - **Scalability**: Designed to handle multiple VPNs and peers, making it suitable for both small and large-scale deployments.
  - **Security**: Implements best practices for securing VPN configurations and communications.
  - **Extensibility**: Provides APIs and hooks for integrating with other systems and automating workflows.
# Installing Wireflow Control Plane
To install Wireflow Control Plane, follow these steps:
1. **Add the Helm Repository**: First, add the Wireflow Helm repository to your Helm client:
   ```bash  helm repo add wireflow https://wireflowio.github.io/helm-charts
   ```
2. **Update Helm Repositories**: Update your Helm repositories to ensure you have the latest charts:
   ```bash  helm repo update
   ```
3. **Install Wireflow Control Plane**: Use Helm to install the Wireflow Control Plane chart:
   ```bash  helm install wireflow wireflow/wireflow
   ```
4. **Verify Installation**: Check the status of the Wireflow Control Plane installation:
   ```bash  kubectl get pods -n wireflow-system
   ```
5. **Access the Dashboard**: Once the installation is complete, you can access the Wireflow dashboard by port-forwarding the service:
   ```bash  kubectl port-forward svc/wireflow-dashboard -n wireflow-system 8080:80
   ```
   Then, open your web browser and navigate to `http://localhost:8080` to access the dashboard.
# Conclusion
Wireflow Control Plane simplifies the management of WireGuard VPNs within Kubernetes environments. Using Kubernetes native decalared api design.