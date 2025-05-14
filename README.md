# 🎨 Colorful Java Web Application

This is a simple Java web application built using **JSP, Servlets, and Maven**, designed with a colorful front end. The application is packaged as a `.war` file and can be deployed on **Apache Tomcat**.

---

## 📌 Prerequisites

Before you begin, make sure you have the following installed:

- Java (JDK 8 or above)
- Maven
- Apache Tomcat (v9 or above)

---

## 📁 Project Structure
```bash
colorful-webapp/
├── pom.xml
├── src
│   └── main
│       ├── resources
│       └── webapp
│           ├── WEB-INF
│           │   └── web.xml
│           └── index.jsp
├── target
│   ├── classes
│   ├── colorful-webapp
│   │   ├── META-INF
│   │   ├── WEB-INF
│   │   │   ├── classes
│   │   │   └── web.xml
│   │   └── index.jsp
│   ├── colorful-webapp.war
│   └── maven-archiver
│       └── pom.properties
```

---

## ⚙️ How to Build the Project

1. **Clone the repository** (or create manually):
   ```bash
   git clone https://github.com/yourusername/colorful-webapp.git
   cd colorful-webapp

Run this command to build:-
  -->mvn clean install
This will creates:-
  -->target/colorful-webapp.war

Deploy the WAR File to Apache Tomcat
Copy the WAR to your Tomcat webapps/ directory:
sudo cp target/colorful-webapp.war  ~/apache-tomcat-10.1.41/webapps/
Restart Tomcat:
sudo systemctl restart tomcat
Access it at:
http://<your-server-ip>:8080/colorful-webapp
