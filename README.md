The is an EKS demo to show the use of pods, services, and deployments. The application image is a voting app (demo-app) provided as an example from kodekloud.com. The files provided are how this application would work in Kubernetes.

The services expose the ports for the pods to talk to each other and the deployments are definitions for pods to be launched from.

Follow these steps to deploy the demo application on your EKS cluster:

1. Clone this repository to your local machine:

2. Navigate to the cloned directory:

cd eks-demo

3. Apply the Kubernetes configurations using kubectl:

kubectl apply -f deployments/
kubectl apply -f services/


4. Verify that the deployments and services are running:

kubectl get deployments
kubectl get services


5. Access the deployed application:

Get the external IP address of the service:

kubectl get services

Open a web browser and enter the external IP address in the address bar. You should see the application running.
