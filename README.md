# AWS-Scalable-WebApp-Architecture

A scalable and fault-tolerant web application architecture built on **AWS**, utilizing key services such as **Elastic Beanstalk**, **RDS**, **CloudFront**, **ElastiCache**, **RabbitMQ**, and more.  
This project demonstrates best practices for high availability, performance, and seamless deployment of Java Spring Boot applications.

![Architecture Diagram](diagrams/architecture.png)

---

## 🚀 Architecture Overview

This architecture includes the following key AWS services:

- **Amazon Route 53** – DNS routing
- **Amazon CloudFront** – Content Delivery Network (CDN)
- **Application Load Balancer (ALB)** – Distributes traffic across instances
- **Elastic Beanstalk** – Manages app deployment and scaling
- **Amazon RDS (MySQL)** – Backend relational database
- **Amazon ElastiCache (Memcached)** – Caching layer
- **Amazon MQ (RabbitMQ)** – Messaging queue
- **Amazon Elasticsearch** – Full-text search capabilities
- **Amazon CloudWatch** – Monitoring and logging
- **Amazon S3** – Storage for static files

---

## 🛠 Project Structure

Here’s the layout of the project:

```bash
AWS-Scalable-WebApp-Architecture/
├── diagrams/                 # Architecture diagrams (draw.io, svg, png)
├── src/                      # Java Spring Boot app with setup scripts
│   └── vprofile-project/
│       ├── src/              # Source code for the app
│       ├── pom.xml           # Maven configuration
│       ├── Jenkinsfile       # CI/CD pipeline configuration
│       └── ansible/          # Ansible provisioning scripts
├── README.md                 # Project documentation
└── .gitignore                # Git ignore file
```

---

## ⚙️ Getting Started

Follow these steps to set up the project locally.

### 1. Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/AWS-Scalable-WebApp-Architecture.git
cd AWS-Scalable-WebApp-Architecture
```

### 2. Setup Environment Variables

Create a `.env` file or export the following environment variables in your shell:

```env
DB_USERNAME=your-db-user
DB_PASSWORD=your-db-pass
RABBITMQ_USER=your-rabbitmq-user
RABBITMQ_PASS=your-rabbitmq-pass
```

Update the `src/main/resources/application.properties` file to use environment variables or secure configuration solutions like Spring Cloud Vault.

### 3. Build and Run

To build and run the project:

```bash
cd src/vprofile-project
mvn clean install
java -jar target/vprofile-project.jar
```

---

## 🚀 Deployment Options

You can deploy this architecture on AWS using the following tools:

- **Elastic Beanstalk** for app deployment
- **Ansible** for automated provisioning (check the `ansible/` directory)
- **Jenkins** for CI/CD pipeline management

---

## 🧠 Credits

This project is based on the [vprofile app](https://github.com/devopshydclub/vprofile-project), which inspired the design. This repository extends the original app into a scalable AWS architecture following modern best practices.

---

## 📄 License

This project is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).  
Feel free to use, modify, and contribute!

---

## 🙌 Contributing

We welcome contributions! If you’re planning to make significant changes, please open an issue first to discuss the changes you’d like to make.

---

## 📬 Contact

Have questions or feedback?  
Feel free to reach out via GitHub issues or email at `puspendrachawlax@gmail.com`.

---
