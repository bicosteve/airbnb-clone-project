# Airbnb Clone Project

## Team Roles

1. Bico Oloo - Backend Developer/Quality Assurance.
   **Backend Developer**

   - Designs high level architect of the software
   - Performs code reviews
   - Implements the core algorithms of the application and business logic.

   **Quality Assurance Engineer**

   - Makes sure the application performs according to the requirements
   - Spots functional and non-functional defects.
   - Verifies whether an application meets the requirements.

## Technology Stack

The technology stack to be used on this project are;

**1. Programming Language**

- Python : This is multipurpose object oriented programming language which can be used for both web developement and machine learning.

**2. Framework**

- Django : A high level Python web framework that encourages rapid development and clean, pragmatic design (www.djangoproject.com).

**3. Database Management**

- MySQL : This is an open source relational database management system that uses Structured Query Language to manage and query data.

**4. APIs**

- Django REST framework : a toolkit for building web APIs used in conjunction with Django web framework.

**5. GraphQL**

- An open source-data query and manipulation language for APIs, and a runtime for fullfilling queries with existing data (https://hygraph.com/learn/graphql).

## Database Design

These are the entities that will be used in this project schema.
**1. Users**

- This entity will contain user data in terms of usernames, passwords, and status
- The main fields in this entity will be user_id, username, email, and password.

**2. Properties**

- This entity will contain data in regards to properties available
- It will have fields like property_id, user_id, location, price.
- Properties entity will have a one-to-many relationship with Users and a many-to-many relationship with Bookings.

**3. Bookings**

- This entity will contain information pertaining to user bookings.
- The main fields in this entity will be booking_id, user_id, property_id
- It will have a one-to-many relationship with Properties and a one-to-many relationship with Users.

**4. Reviews**

- This entity will contain information pertaining to property reviews.
- The main fields in this entity will be review_id, user_id, property_id
- It will have a one-to-one relationship with Properties.

**4. Payments**

- This entity will contain information pertaining to property payments.
- The main fields in this entity will be payment_id, user_id, property_id, status
- It will have a one-to-many relationship with Properties and Users.
