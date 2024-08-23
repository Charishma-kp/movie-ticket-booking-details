ONLINE-TICKET-BOOKING-SYSTEM
1.INTRODUCTION TO ONLINE MOVIE TICKET BOOKING SYSTEM:

In today's digital age, the convenience of booking movie tickets online has revolutionized the way people experience entertainment. Online Movie Ticket Booking Systems provide a seamless platform for users to browse movies, select showtimes, choose seats, and make payments from the comfort of their homes or on the go using their smartphones. This introduction explores the key features and benefits of such a system. Online movie ticket booking systems have revolutionized the way audiences experience and interact with cinema. Traditionally reliant on physical box offices and manual ticketing processes, these systems now leverage digital platforms to offer seamless and efficient booking experiences

2.TECHNOLOGY STACK:

Frontend: Typically developed using web technologies (HTML, CSS, JavaScript) or desktop GUI frameworks like Tkinter (Python) for a native application.
Backend: Utilizes server-side languages (Python, PHP, etc.) and databases (MySQL, SQLite, etc.) to handle data storage, retrieval, and processing.
API Integration: Integrates with external APIs for movie data (e.g., movie details, showtimes) and payment gateways for secure transactions
3.ER DIAGRAM AND EXPLANATION :

image An Entity-Relationship (ER) diagram for an online movie ticket booking system provides a visual representation of the database schema, depicting entities (tables), attributes (columns), and relationships between entities. Here’s an explanation of the typical entities and relationships you might find in such a diagram.

ENTITIES:

User: o Attributes: UserID (Primary Key), Username, Password, Email, Phone, Address
Movie: o Attributes: MovieID (Primary Key), Title, Genre, Director, Duration, ReleaseDate, Rating
Cinema: o Attributes: CinemaID (Primary Key), Name, Location, Capacity
Showtime: o Attributes: ShowtimeID (Primary Key), MovieID (Foreign Key to Movie), CinemaID (Foreign Key to Cinema), StartTime, EndTime
Booking: o Attributes: BookingID (Primary Key), UserID (Foreign Key to User), ShowtimeID (Foreign Key to Showtime), BookingDate, Status
Payment: o Attributes: PaymentID (Primary Key), BookingID (Foreign Key to Booking), PaymentDate, Amount, PaymentMethod Relationships:
User - Booking (One-to-Many): o Each user can make multiple bookings, but each booking is made by exactly one user. o Direction: User (1) <---> (many) Booking
Movie - Showtime (One-to-Many): o Each movie can have multiple showtimes, but each showtime is associated with exactly one movie. o Direction: Movie (1) <---> (many) Showtime
Cinema - Showtime (One-to-Many): o Each cinema can host multiple showtimes, but each showtime occurs in exactly one cinema. o Direction: Cinema (1) <---> (many) Showtime
Booking - Payment (One-to-One): o Each booking is associated with exactly one payment, and each payment is made for exactly one booking. o Direction: Booking (1) <----> (1) Payment
Explanation:

• User Entity: Represents users of the system who register and book tickets. The User ID serves as the primary key, uniquely identifying each user. • Movie Entity: Stores information about movies available for booking, with Movie ID as the primary key. Attributes include details like title, genre, director, and release date. • Cinema Entity: Represents cinemas where movies are screened, identified uniquely by Cinema ID. Attributes include name, location, and seating capacity. • Showtime Entity: Contains details about specific showtimes for movies at cinemas. Showtime ID serves as the primary key, with attributes Start Time and End Time indicating the time window for each show. • Booking Entity: Records each booking made by users for specific showtimes. Booking ID uniquely identifies each booking, with attributes like Booking Date and Status (e.g., confirmed, cancelled). • Payment Entity: Stores payment information for each booking. Payment ID is the primary key, linked to a specific Booking ID, along with attributes like Payment Date, Amount, and Payment Method.

4.PERFORMING CRUD OPERATIONS:

image FIG 4.1: ADDING MOVIE DETAILS TO THE DATABASE

image FIG 4.2: OBTAINING MOVIE DETAILS THROUGH PRIMARY KEY MovieID

image FIG 4.3: DISPLAYING ALL THE DETAILS OF THE MOVIE ENTERED INTO DATABASE

image FIG 4.4: BEFORE UPDATING THE DETAILS OF MOVIEID 2

image FIG 4.5: AFTER UPDATING CAST DETAILS BY ADDING THE SANJAY DUTT IN MOVIEID2

This repository contains the source code for Online Movie Ticket Booking System, which was a Mini Project for Database Management System (DBMS).
