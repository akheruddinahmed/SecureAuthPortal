# SecureAuthPortal

A comprehensive **Spring Boot** web application that implements secure user authentication with **registration and login** features, using **PostgreSQL**, **Spring Data JPA**, and **Thymeleaf** for the frontend.

---

## 🚀 Features

* ✅ User Registration with validation
* ✅ User Login authentication
* ✅ Session-based authentication (login/logout)
* ✅ Protected profile page
* ✅ PostgreSQL database integration
* ✅ Clean and responsive UI with Thymeleaf
* ✅ MVC architecture (Controller → Service → Repository)

---

## 🛠️ Tech Stack

* **Backend:** Spring Boot, Spring MVC
* **Database:** PostgreSQL
* **ORM:** Spring Data JPA / Hibernate
* **Frontend:** Thymeleaf, HTML, CSS
* **Build Tool:** Maven
* **Java Version:** Java 17

---

## 📁 Project Structure

```
SecureAuthPortal/
├── src/main/java/in/sp/
│   ├── controllers/
│   ├── entities/
│   ├── repositories/
│   └── services/
├── src/main/resources/
│   ├── templates/
│   ├── static/
│   └── application.properties
├── pom.xml
├── Dockerfile
└── README.md
```

---

## ⚙️ Configuration

Update your `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/reg_login_db
spring.datasource.username=postgres
spring.datasource.******

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/akheruddinahmed/SecureAuthPortal.git
cd SecureAuthPortal
```

2. Open in IDE (Spring Tool Suite / IntelliJ)

3. Create PostgreSQL database:

```sql
CREATE DATABASE reg_login_db;
```

4. Update `application.properties` with your database credentials

5. Run the application using Maven:

```bash
mvn spring-boot:run
```

Or run the main application class: `SecureAuthPortalApplication.java`

6. Open your browser and navigate to:

```
http://localhost:8080/
```

---

## 🐳 Docker Support

The project includes a `Dockerfile` for containerization. Build and run using:

```bash
docker build -t secure-auth-portal .
docker run -p 8080:8080 secure-auth-portal
```

---

## 🔐 Authentication Flow

1. Register a new user with email and password
2. Login with registered credentials
3. Session is created upon successful login
4. Access protected profile page
5. Logout invalidates the session

---

## 💡 Future Improvements

* 🔒 Password encryption (BCrypt)
* 🔑 Spring Security integration with JWT
* 🌐 REST API version
* 📱 Responsive mobile UI
* 🧪 Unit and integration tests
* 📧 Email verification for registration

---

## 👨‍💻 Author

**Akher Uddin Ahmed**  
Java Full Stack Developer

---

## ⭐ Support

If you find this project helpful, please consider giving it a ⭐ on GitHub!
