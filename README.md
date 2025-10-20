---

## 🚀 Two-Tier Flask Application with Docker Compose

This project is a **two-tier web application** built using **Docker** and **Docker Compose**. It includes a **Flask web application (frontend)** and a **MySQL database (backend)** running in separate containers.

With this application, users can **submit and view messages**. All messages are stored in the database, demonstrating the complete data flow of the system.

---

### 🛠️ Tech Stack & Tools

**Backend Framework:** **Flask (Python)**
A lightweight web framework that handles HTTP requests and renders HTML pages.

**Database:** **MySQL**
A powerful database used to permanently store all user messages.

**Containerization:** **Docker**
Used to package the application and database into isolated containers for consistency across environments.

**Orchestration:** **Docker Compose**
Used to run and connect multiple containers together seamlessly.

---

### ⚙️ Key Architectural Concepts

**Two-Tier Architecture:**
The application and database are divided into two separate layers, keeping the codebase clean and modular.

**Containerization:**
Both services run inside containers, providing a consistent environment everywhere.

**Environment Variables:**
Sensitive data (like database passwords) are stored securely in environment variables instead of hardcoding them.

**Service Health Checks:**
Docker Compose is configured so that the Flask app starts **only after** the MySQL database is fully ready.

---

### 🚀 How to Run the Project

Follow these simple steps to deploy and run the project.

#### **Prerequisites**

Make sure **Docker** and **Docker Compose** are installed on your system.

#### **Steps to Deploy**

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Fahad-developer/Docker-Two-Tier-Application.git
   cd Docker-Two-Tier-Application
   ```

2. **Build and Run the Containers:**
   This command will build and start both containers.

   ```bash
   docker-compose up --build -d
   ```

3. **Access the Application:**
   Once the containers are running, open the application in your browser:

   * **Local deployment:** [http://localhost:5000](http://localhost:5000)
   * **Cloud server (e.g., EC2):** `http://<server-ip>:5000`

---

### 🧹 Cleaning Up

To stop and remove the containers (including volumes), run:

```bash
docker-compose down -v
```

---
