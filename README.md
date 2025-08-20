# Airbnb Clone Project  

## 🚀 Objective  
Build a scalable Airbnb-like platform for property listings, bookings, and payments.  

## 🏆 Goals  
- User authentication & profile management  
- Property listing & booking system  
- Secure payment integration  
- Scalable backend with APIs  

## ⚙️ Tech Stack  
- **Backend**: Django  
- **Database**: PostgreSQL  
- **API**: GraphQL & REST  
- **Deployment**: Docker, CI/CD  


## 👥 Team Roles  

- **Backend Developer**:  
  Responsible for building the server-side logic of the application. This includes developing APIs, implementing business logic, and integrating third-party services to ensure smooth communication between the client and the server.

- **Database Administrator (DBA)**:  
  Designs and maintains the project’s databases. Ensures data integrity, implements indexing for performance optimization, and manages backups, migrations, and database security.

- **DevOps Engineer**:  
  Handles deployment, automation, and infrastructure management. Sets up and monitors CI/CD pipelines, manages cloud resources, and ensures scalability, reliability, and smooth delivery of updates.

- **QA Engineer**:  
  Ensures the quality of the software through testing. This includes writing and running test cases, identifying bugs, verifying security, and validating that all features meet requirements before release.


## Technology Stack
- **Django**: Python web framework to build REST APIs.
- **Django REST Framework**: API tools for CRUD operations.
- **PostgreSQL**: Relational database for structured storage.
- **GraphQL**: Flexible query language for efficient data retrieval.
- **Celery + Redis**: Asynchronous tasks & caching.
- **Docker**: Containerization for consistent deployments.
- **GitHub Actions**: Automating CI/CD pipeline.


## Database Design
### Entities:
- **Users**
  - id, name, email, password, role
- **Properties**
  - id, title, description, price, host_id
- **Bookings**
  - id, user_id, property_id, check_in, check_out, status
- **Payments**
  - id, booking_id, amount, status, timestamp
- **Reviews**
  - id, user_id, property_id, rating, comment

### Relationships:
- A **user** can list many **properties**.
- A **booking** belongs to one **property** and one **user**.
- A **payment** belongs to a **booking**.
- A **review** is written by a **user** for a **property**.

## Feature Breakdown
- **User Management**: Register/login, manage profiles, authentication.
- **Property Management**: Hosts create/update/delete property listings.
- **Booking System**: Guests book properties, manage check-in/out.
- **Payments**: Secure handling of booking payments.
- **Reviews**: Guests leave ratings & reviews for properties.

## API Security
- **Authentication**: JWT tokens to secure user sessions.
- **Authorization**: Role-based access (hosts vs guests).
- **Rate Limiting**: Prevent abuse of API calls.
- **Data Protection**: Secure sensitive data (e.g., passwords, payment info).
- **Why Important**: Protects user privacy, prevents fraud, ensures trust.

## CI/CD Pipeline
- **Definition**: CI/CD automates testing, building, and deployment of code.
- **Importance**: Ensures quick, reliable updates with minimal errors.
- **Tools**:
  - **GitHub Actions**: Run automated tests & deployments.
  - **Docker**: Containerize the app for consistent environments.
  - **Heroku/AWS**: Deployment platforms for scaling the app.



