# Role-Based Access Control (RBAC) Using React + Spring Boot

The back-end server uses Spring Boot with Spring Security for JWT authentication and The front-end will be created with React.

## Features
- **User Signup**: New users can create an account with their username, email, and password.
- **User Login**: Existing users can log in using their username and password.
- **Role-Based Authorization**: Users are assigned one of the following roles:
  - **`ROLE_USER`**
  - **`ROLE_MODERATOR`**
  - **`ROLE_ADMIN`**

  Authorization is handled by these roles, ensuring different levels of access for users based on their role.

## Frontend Features
- There are Login/Logout and Signup pages.
- Form data will be validated by the front-end before being sent to the back-end.
- Depending on the user’s roles (admin, moderator, user), the Navigation Bar changes its items automatically.

## Database Setup

To set up the database, run the following SQL statements to insert roles:

```sql
-- Insert roles into the 'roles' table
INSERT INTO roles(name) VALUES('ROLE_USER');
INSERT INTO roles(name) VALUES('ROLE_MODERATOR');
INSERT INTO roles(name) VALUES('ROLE_ADMIN');



