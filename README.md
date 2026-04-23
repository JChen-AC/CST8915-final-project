# CST8915 Final Project Documentation

## Studen information
**Student Name**: Joshua Chen

**Student ID**: 041280453

**Course**: CST8915 Full Stack Development

**Semester**: Winter 2026

## Project overview
This is a demo of a best buy website. That uses 9 microserives. 
1. Store-Front: Customer web app.
2. Store-Admin: Employee web app.
3. Order-Service: Order processing API.
4. Product-Service: Product management API.
5. Makeline-Service: Background worker for order processing.
6. Database: MongoDB (Stateful).
7. Blob Connect: handles uploading and downloading to the blob storage
8. Azure Service Bus : handles order request 
9. Azure Blob storage : stored Product images

## Deployment instructions
To deploy run the 
1. Set up and azure Kubernetes 
2. kubectl apply -f aps-all-in-one.yaml

### **Repository links**
| Service | GitHub | Docker Hub |
|---|---|---|
| Blob Connect | [GitHub](https://github.com/JChen-AC/cst8915-blobconnect-service-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-blob-connector) |
| Order Service | [GitHub](https://github.com/JChen-AC/cst8915-order-service-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-order-service) |
| Makeline Service | [GitHub](https://github.com/JChen-AC/cst8915-makeline-service-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-makeline-service/general) |
| Store Admin | [GitHub](https://github.com/JChen-AC/cst8915-store-admin-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-store-admin) |
| Store Front | [GitHub](https://github.com/JChen-AC/cst8915-store-front-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-store-front/general) |
| Product Service | [GitHub](https://github.com/JChen-AC/cst8915-product-service-final-project) | [Docker Hub](https://hub.docker.com/repository/docker/jchen1101/fp-product-service) |

## Demo Video
https://youtu.be/LoHTf25a_Eo

## Diagram
![architecture diagram ](./cst8915-fp3.drawio.png) 


## AI Disclosure 
AI was used extensively in this project and repository

### Simulation
ChatGPT and Claude were used in the following ways :
- used to help debug issues with setting up the cluster
- used to help set up azure service bus and blob storage. As well as how to handle authentication while dealing with kubernetes
- helped modify the order service messagequeue.js to connect to azure service bus
- debug a variety of coding issues
- helped extensively with debugging blob connector and ProductForm.vue
- helped determine microservice architecture for the blob connector
  
## References 
- https://learn.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-nodejs?tabs=managed-identity%2Croles-azure-portal%2Csign-in-azure-cli&pivots=blob-storage-quickstart-scratch




