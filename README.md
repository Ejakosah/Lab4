# Lab4

Task 1 
<img width="945" height="753" alt="image" src="https://github.com/user-attachments/assets/137b74d4-5dc8-41c9-b9d9-da6dd9605c31" />

<img width="942" height="804" alt="image" src="https://github.com/user-attachments/assets/95df0e2b-eb9f-4a36-84ef-6c9de7911e46" />

<img width="954" height="784" alt="image" src="https://github.com/user-attachments/assets/284981f1-33cf-4219-a1d2-0cd6bd37d171" />

<img width="650" height="421" alt="image" src="https://github.com/user-attachments/assets/32a82605-1295-42a0-8027-d3376e637e6c" />


I listed all available projects using the gcloud CLI and identified my project ID as dotted-saga-484500-n2 under My First Project. This confirmed that I was authenticated and had access to the correct Google Cloud project. I set the active project to dotted-saga-484500-n2. I set the default compute zone to us-east1-b. I enabled the Google Cloud services: Cloud Resource Manager API, Kubernetes Engine API, Artifact Registry API. This step was required to allow project management, cluster creation, and container image storage functionality. I created a GKE cluster named gke-cluster with 3 nodes Zone: us-east1-b. I listed all active and running Kubernetes clusters. Using kubectl get nodes, I verified that all three worker nodes were in the Ready state. 

Task 2 — Reuse Your Lab 3 Manifests and Deploy the Baseline System

<img width="949" height="591" alt="image" src="https://github.com/user-attachments/assets/bab65ac0-e64c-4623-ab4f-e9732bf00baf" />

<img width="939" height="319" alt="image" src="https://github.com/user-attachments/assets/13fcaf84-ff20-4c6c-900b-47ced18478b5" />

<img width="953" height="637" alt="image" src="https://github.com/user-attachments/assets/7c54d8e6-c5cc-431a-8ecf-61b266d38583" />

I navigated to the gke-microservices-manifests directory and verified my current path. I confirmed that all required Kubernetes manifest files were present for the products and orders microservices. I applied the Kubernetes manifests for the products microservice and this created: A Deployment to manage the product pods and a ClusterIP Service to expose the application internally within the cluster as the deployment was successfully created. I deployed the orders microservice using its manifest file and multiple replicas were made along with a corresponding ClusterIP Service successfully. I launched a temporary http-client pod using a curl container image. Initially, the pod showed a Pending status while Kubernetes scheduled it then it transitioned to running. I later rechecked the deployments and confirmed both products and orders were fully available with all replicas running. This verified that Kubernetes successfully scheduled and started all containers.


Task 3 — Create the Release Candidate Image (orders:v2 only)

<img width="1077" height="866" alt="image" src="https://github.com/user-attachments/assets/9e1d7617-0ddf-4e0c-a162-7cd1bdc26553" />

<img width="1091" height="871" alt="image" src="https://github.com/user-attachments/assets/2f68fd67-406c-421d-a2bb-93e48cf2eddf" />

<img width="827" height="876" alt="image" src="https://github.com/user-attachments/assets/82f17d4f-76fb-4ff9-a2ff-202319f08417" />

<img width="1068" height="807" alt="image" src="https://github.com/user-attachments/assets/b2b76ab6-2bef-4a53-b79b-9498908b44c4" />

<img width="856" height="146" alt="image" src="https://github.com/user-attachments/assets/ae7f97a6-4590-493c-ad0b-1637ae8efa16" />

<img width="1069" height="307" alt="image" src="https://github.com/user-attachments/assets/ff2a857a-f9de-4d92-8fc6-a5dc61883565" />

<img width="1069" height="678" alt="image" src="https://github.com/user-attachments/assets/62787358-ed4c-4077-8b1b-62110c83f49a" />

<img width="1074" height="500" alt="image" src="https://github.com/user-attachments/assets/8c5291f4-07e1-4403-a727-b09da3966fc9" />



Task 4 — Rolling Updates (Built-in Kubernetes Deployment Strategy)






Task 5 — Canary Release (Controlled Partial Rollout)






Task 6 — Blue-Green Deployment (Instant Cutover via Service Selector)





Task 7 — Reflection Questions (Conceptual Understanding)






Task 8 — Cleanup (Delete the Kubernetes Cluster)



