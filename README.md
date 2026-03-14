# CST8915 – Lab 5  
## Containerizing the Algonquin Pet Store with Docker

**Course:** CST8915 – Full-stack Cloud-native Development  
**Lab:** Lab 5  
**Student:** Sara Mirzaei  


---

# Lab Overview

The purpose of this lab is to learn how to containerize microservices using Docker and manage them using Docker Compose.  

The Algonquin Pet Store application consists of multiple microservices including:

- Order Service (Node.js)
- Product Service (Python or Rust)
- Store Front (Vue.js)
- RabbitMQ (Message broker)

Each service is containerized using Docker and orchestrated together using Docker Compose.

---

# Lab Objectives

- Understand the fundamentals of Docker containers
- Containerize microservices using Dockerfiles
- Manage multi-container applications using Docker Compose
- Push Docker images to Docker Hub
- Run a full microservice application locally using containers

---

# Technologies Used

- Docker
- Docker Compose
- Node.js
- Python / Rust
- Vue.js
- RabbitMQ
- Nginx

---


## Demo Video

YouTube Demo Link:

[Youtube Video](https://youtu.be/Z5o6n2x6pJw)

---


## Docker Compose File

The Docker Compose file used for running the application with local images is available here:

[View docker-compose.yml](./docker-compose.yml) 

The Docker Compose file used for running the application with Docker Hub–hosted images is available here:

[View Docker-Hub yml file](./docker-compose1.yml)

## Docker File

The Docker files configuration used in this lab can be found here: 

**Order Servic Docker File:** [Order Service Dockerfile](https://github.com/saraMir26/order-service-L5/blob/main/Dockerfile)

**Store Front Docker File:** [Store Front Docker File](https://github.com/saraMir26/store-front-L5/blob/main/Dockerfile)

**Product Service Dockerfiles:**

- Rust Version   [Rust Dockerfile](https://github.com/saraMir26/product-service-rust-L5/blob/main/Dockerfile)

- Python Version   [Python Dockerfile](https://github.com/saraMir26/product-service-python-L5/blob/main/Dockerfile)



---
## Notes – Setup Challenges / Lessons Learned

During this lab I learned how to containerize multiple microservices and run them together using Docker Compose.

One challenge was ensuring that the services communicate correctly within the Docker network. 

Another challenge was building and pushing images to Docker Hub and making sure the correct image names were referenced in the docker-compose.yml file. Once the images were pushed successfully, Docker Compose was able to pull and run them correctly.
