Kubernetes Orchestration Using Yolo app
Description
This project utilizes Kubernetes to orchestrate the YOLO app on a cluster and expose it for access. YOLO application consists of a client and backend component. The project ensures seamless deployment and management of the app using Kubernetes.

Set up
To get started with Kubernetes Orchestration, follow the steps below:

Ensure that you have minikube and kubectl are installed on your local machine. This will allow you to run Kubernetes clusters locally for testing and development purposes.

Clone this repository to your local machine using git clone.

Start Minikube on your machine. You can use the following command to start Minikube: minikube start

Navigate to the client and backend directories in the cloned repository.

In each directory (client, backend and database), create the necessary Kubernetes manifests:

Deployment: Define the desired state and number of replicas for the client, backend and mongo components.
Service: Expose the client, backend and mongo components as Kubernetes services.
Secrets: Configure any environment-specific secrets or configuration required by the application as defined in the resctive directories secret files.
PVC (PersistentVolumeClaim): If applicable, set up persistent storage for the backend component. You can create the YAML files for these Kubernetes objects based on the requirements of your YOLO app.
Apply Kubernetes using the kubectl apply command.

Technology Used
The project is mainly built using YAML .

License MIT License
Copyright (c) 2023