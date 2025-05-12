# alx-airbnb-database

# Entity and Relationships

The system has these  entities:
- User – Represents guests, hosts, and admins.
- Property – Houses listed by hosts.
- Booking – Tracks reservations between users and properties.
- Payment – Records transactions related to bookings.
- Review – Allows users to rate and comment on properties.
- Message – Facilitates communication between users.

Define Relationships
- A User can host multiple Properties (One-to-Many).
- A User can book multiple Properties, but a Booking belongs to only one User (Many-to-One).
- A Booking belongs to one Property, but a Property can have multiple bookings (One-to-Many).
- A Payment is linked to a Booking, ensuring a valid transaction.
- A User can write multiple Reviews, each belonging to a Property (One-to-Many).
- A User can send multiple Messages to another User (One-to-Many).

