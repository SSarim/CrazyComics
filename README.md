# CrazyComics

CrazyComics is a full-stack comic book reading platform designed to provide a seamless and engaging experience for comic enthusiasts. It enables users to browse, read, and manage their favorite comic books with ease, backed by robust and scalable architecture.

## Features
- **User-Friendly Interface:** Designed with HTML/CSS for a clean and intuitive user experience.
- **Secure Backend:** Built using Java to ensure robust data handling and seamless integration with the MySQL database.
- **Microservices Architecture:** REST APIs and KubeMQ integration for streamlined communication between services.
- **Real-Time Data Handling:** Leverages KubeMQ for efficient, real-time interactions between microservices.
- **Cloud Deployment:** Fully deployed on Google Cloud Platform (GCP) using Docker and Kubernetes for scalable and efficient orchestration.

## Technology Stack
- **Frontend:** HTML, CSS
- **Backend:** Java
- **Database:** MySQL
- **Messaging:** KubeMQ
- **Containerization:** Docker
- **Orchestration:** Kubernetes
- **Cloud Platform:** Google Cloud Platform (GCP)
- **Operating System:** Linux

## Architecture
The CrazyComics platform is built using a microservices architecture to ensure modularity, scalability, and reliability. Each service communicates through REST APIs, with KubeMQ managing message queues for real-time data exchange. Docker containers are used for deployment, and Kubernetes handles orchestration for efficient scaling.

## Setup and Installation
### Prerequisites
- Docker
- Kubernetes (kubectl and Minikube or any Kubernetes environment)
- Google Cloud Platform account
- Java JDK 11+
- MySQL Server
- Maven or Gradle (for Java project management)

### Installation Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/CrazyComics.git
   cd CrazyComics
   ```

2. **Set Up MySQL Database**
   - Install and configure MySQL server.
   - Import the database schema using the provided SQL file:
     ```bash
     mysql -u your_username -p < database/schema.sql
     ```

3. **Build the Backend**
   - Navigate to the backend directory and build the Java application:
     ```bash
     cd backend
     mvn clean install
     ```

4. **Configure Docker Containers**
   - Ensure Docker is installed and running.
   - Build the Docker images for each service:
     ```bash
     docker build -t crazycomics-service .
     ```

5. **Deploy on Kubernetes**
   - Apply Kubernetes configuration files:
     ```bash
     kubectl apply -f kubernetes/
     ```

6. **Access the Application**
   - Expose the application and get the external IP:
     ```bash
     kubectl get services
     ```
   - Open the application in your browser using the displayed IP address.

Project is temporality deploed on GCP via : http://35.203.53.221/FrontEnd/


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact
For inquiries or support, please reach out to:
- **Sarim Shahwar**  
  [LinkedIn](https://www.linkedin.com/in/sarimshahwar)  
  [Email](mailto:your-email@example.com)

---

Happy reading with CrazyComics! 📚
