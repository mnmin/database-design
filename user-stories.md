A local cinema wants to allow people to book tickets online to see movies that are being shown in its various screens. These tickets should be delivered to customers via email. The cinema wants to keep a record of their customers and the tickets they purchase, as well as offer a regularly updated list of movies for them to choose from. A single screen might show multiple movies a day, and even the same movie at multiple times. The cinema will expand its number of screens in the future, so the potential for growth needs to be accounted for.


- As a customer, so I can receive my tickets, I want to provide my contact information.
  - User & Profile
- As a customer, so I can decide which movie I want to watch, I want to see a list of movies.
  - Movies
- As a customer, I want to buy multiple tickets and choose specific seats
- Tickets, Movies
  
- As an admin, so I can manage the movies shown at the cinema, I want to update the list of movies.
  - User & Movies & Screens
- As an admin, I want to send via email to customers an updated lists of movies
  - User & User/Profile & Movies
- As a cinema, I want a list of customers and their purchase history
  - User & Profile
- A movie scheen must have multiple movie lists whith their titles and time of showing for each day
  - Screens & Movies
- The cinema should be able to add movie screens
  - Admin user & Screens

DB
-User
    -ID
    -Username
    -Password
    -createdAt
    -updatedAt
    -role VC (Admin)

-Profile/Contact
    -ID
    -User_ID
    -purchase history (tickets)
    -Email
    -Phone number
    -createdAt
    -updatedAt

-Movies
    -Name (ID)
    -Length
    -createdAt
    -Description
    -Duration
    -Rating (PG)
    -Movie Image
-Screens
    -Movie showings & time
    -Capacity
    -Seats available/booked
    -createdAt
    -Screen ID
-Screening
    -Id
    -Start_Time
    -Movie_Id
    -Screen_Id
    -Created_At
    -Updated_At
-Cinema
    -ID
    -Address
    -No of screen
-Tickets
    -ID
    -Screening_Id
    -User_Id
    -Type (adult/child)
    -createdAt
    -updatedAt
-Image
    -Cinema Image
    -Movie Images
    -Profile Images
