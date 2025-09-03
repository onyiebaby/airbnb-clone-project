# airbnb-clone-project
A simple Airbnb clone project 
## Team Roles
- **Project Managers**: Oversees the project, ensures dadlines are met and supervises tasks.
-  **Frontend Developers**: Handles the UI/UX, builds user interfaces with HTML, CSS and JAVASCRIPT.
-  **Backend Develpers**: Manages the server, database and APIs
-  **DevOps Engineers**: Sets up deployment pipelines, manages hosting, and ensures scalability

## Technology Stack
- **Django**: Backend web framework used to build the core application logic, handle authentification and manage bookings.
- **PostgreSQL**: Relational database to store users, property listings, reservations, and reviews securely.
- **GraphQL**: API query language that allows flexible and efficient data fetching for the frontend
- **Dockers**: Containerization tool for consistent development and deployment environment.

  ## Database Design

- **Users**: id, name, email, password, role
- **Properties**: id, title, location, price, owner_id
- **Bookings**: id, user_id, property_id, check_in, check_out
- **Reviews**: id, user_id, property_id, rating, comment
- **Payments**: id, booking_id, amount, status, date

**Relationships**:
- A user can own multiple properties.
- A user can make multiple bookings.
- A booking belongs to one property and one user.
- A property can have many reviews.
- A payment is linked to a single booking.
