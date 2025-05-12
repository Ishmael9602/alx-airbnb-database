
# Entity Relationship Diagram (ERD) Requirements

## Entities & Attributes

### User
- id (PK)
- name
- email
- password
- phone_number
- created_at

### Property
- id (PK)
- owner_id (FK to User)
- title
- description
- location
- price_per_night

### Booking
- id (PK)
- user_id (FK to User)
- property_id (FK to Property)
- start_date
- end_date
- total_cost

### Review
- id (PK)
- user_id (FK to User)
- property_id (FK to Property)
- rating
- comment

### Payment
- id (PK)
- booking_id (FK to Booking)
- amount
- payment_date
- status

## Relationships
- A User can own many Properties
- A User can make many Bookings
- A User can leave many Reviews
- A Property can have many Bookings
- A Property can have many Reviews
- A Booking has one Payment

