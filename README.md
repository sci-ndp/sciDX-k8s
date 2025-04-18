# sciDX Kubernetes Resource

This repository contains Kubernetes manifests and supporting files for deploying and managing scidx services stack within a Kubernetes cluster.

## Basic Set up

1. **Deploy CKAN on VM**

    Please follow the link for instruction: [`ckan docker deployment`](https://github.com/sci-ndp/pop-ckan-docker/blob/master/README1.md)

2. **Install the Ingress Controller**:

    Navigate to the [`./nginx-ingress-controller`](./nginx-ingress-controller/) directory and follow the instructions to install the NGINX Ingress Controller in your cluster.

    > If you are using a MicroK8s cluster and have a DNS name for which you want HTTPS support with the NGINX Ingress Controller, refer to the [`./ssl-cert_microk8s`](./ssl-cert_microk8s/) directory for guidance.

3.  **Data Streaming Setup**: deploy Kafka cluster into your cluster

    Navigate to [`./apache-kafka`](./apache-kafka) and follow the provided instructions to deploy Kafka cluster into your cluster

4. **Deploy `NDP Endpoint(pointofpresence) API`**:

    Once the ingress controller is installed, navigate to either the [`./pointofpresense`](./pointofpresense) directory and follow the deployment instructions to deploy the respective applications.

