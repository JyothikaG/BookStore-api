📚 **BookStore API**

  A Spring Boot RESTful API for managing authors and books in a bookstore.
This project demonstrates CRUD operations, entity relationships, and service-layer abstraction using Spring Boot, JPA, and Hibernate.

🚀 **Features**

**Manage Authors**

- Create, update, delete, and fetch authors.
- Each author can have multiple books.

**Manage Books**

- Create, update, delete, and fetch books.
- Each book is linked to an author.
- RESTful APIs with clear endpoint mappings.
- Uses Spring Data JPA for database interaction.
- Follows a Service + Repository layered architecture.

🏗️ **Project Structure**

BookStore.api
 ┣ 📂 com.example.demo
 ┃ ┣ 📂 models
 ┃ ┃ ┣ Author.java        # Entity for Author
 ┃ ┃ ┗ Book.java          # Entity for Book
 ┃ ┣ 📂 repository
 ┃ ┃ ┗ AuthorRepository.java
 ┃ ┣ 📂 services
 ┃ ┃ ┗ AuthorService.java
 ┃ ┣ 📂 controllers
 ┃ ┃ ┣ AuthorController.java
 ┃ ┃ ┗ BookController.java
 ┃ ┗ DemoApplication.java # Main Spring Boot entry point
 ┣ 📜 pom.xml (Maven dependencies)
 ┗ 📜 README.md


⚙️ **Tech Stack**

- Java 17+
- Spring Boot 3+
- Spring Data JPA (Hibernate)
- H2 / MySQL (configurable)
- Maven

▶️ **Getting Started**

**Configure the database**

Edit src/main/resources/application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/bookstore

spring.datasource.username=root

spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update

spring.jpa.show-sql=true

**Run the application**

mvn spring-boot:run

**Access the API**

The application will start at:
http://localhost:8080

✅ **Future Enhancements**

- Add DTOs & ModelMapper for cleaner API responses.
- Implement pagination & sorting.
- Add unit & integration tests with JUnit and Mockito.
- API documentation with Swagger/OpenAPI.
