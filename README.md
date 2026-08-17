# AssessPro — Java Assessment Portal

A complete, responsive assessment portal starter built with Java Spring Boot, Thymeleaf, Spring Security, JPA, H2, Bootstrap 5, and vanilla JavaScript.

## Features
- Login/logout with roles: ADMIN, INSTRUCTOR, STUDENT
- Student dashboard with assessments, attempts, scores, progress and results
- Assessment instructions and timed assessment UI
- Multiple-choice questions with auto-save UI
- Automatic scoring for submitted assessments
- Professor assessment/question management
- Admin dashboard with platform statistics
- Responsive modern UI
- H2 database for easy local development
- Sample users and sample assessment data

## Demo accounts
- Student: student@assesspro.com / student123
- Professor: professor@assesspro.com / professor123
- Admin: admin@assesspro.com / admin123

## Requirements
- Java 17+ (Java 23 tested)
- Maven 3.9+

## Run
mvn spring-boot:run

Then open http://localhost:8080

The H2 console is available at /h2-console during development.
JDBC URL: jdbc:h2:mem:assesspro
Username: sa
Password: (empty)

## Structure
src/main/java/com/assesspro/portal
  config       security + seed data
  controller   MVC controllers
  model        JPA entities/enums
  repository   Spring Data repositories
  service      business logic
src/main/resources
  templates    Thymeleaf pages
  static       CSS and JavaScript

## Hackathon demo flow
1. Login as Student.
2. Open Java Programming Fundamentals.
3. Start the timed assessment.
4. Answer questions and submit.
5. Show the automatic result and attempt history.
6. Logout and login as Professor to show the management console.
7. Logout and login as Admin to show platform statistics.

## Important
Maven is required because the project intentionally uses a standard Spring Boot Maven build. The project does not require Lombok.
