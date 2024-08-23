# ONLINE-TICKET-BOOKING-SYSTEM  

1.INTRODUCTION TO ONLINE MOVIE TICKET BOOKING SYSTEM:

In today's digital age, the convenience of booking movie tickets online has
revolutionized the way people experience entertainment. Online Movie Ticket Booking
Systems provide a seamless platform for users to browse movies, select showtimes,
choose seats, and make payments from the comfort of their homes or on the go using
their smartphones. This introduction explores the key features and benefits of such a
system.
Online movie ticket booking systems have revolutionized the way audiences
experience and interact with cinema. Traditionally reliant on physical box offices and
manual ticketing processes, these systems now leverage digital platforms to offer
seamless and efficient booking experiences

2.TECHNOLOGY STACK:
* Frontend: Typically developed using web technologies (HTML, CSS, JavaScript)
or desktop GUI frameworks like Tkinter (Python) for a native application.
* Backend: Utilizes server-side languages (Python, PHP, etc.) and databases
(MySQL, SQLite, etc.) to handle data storage, retrieval, and processing.
* API Integration: Integrates with external APIs for movie data (e.g., movie details,
showtimes) and payment gateways for secure transactions

3.ER DIAGRAM AND EXPLANATION :

![image](https://github.com/user-attachments/assets/9f96f03c-af8b-4cf1-99b5-535ac0f52a82)
An Entity-Relationship (ER) diagram for an online movie ticket booking system provides a visual representation of the database schema, depicting entities (tables), attributes (columns), and relationships between entities. Here’s an explanation of the typical entities and relationships you might find in such a diagram.

ENTITIES:
1.	User:
o	Attributes: UserID (Primary Key), Username, Password, Email, Phone, Address
2.	Movie:
o	Attributes: MovieID (Primary Key), Title, Genre, Director, Duration, ReleaseDate, Rating
3.	Cinema:
o	Attributes: CinemaID (Primary Key), Name, Location, Capacity
4.	Showtime:
o	Attributes: ShowtimeID (Primary Key), MovieID (Foreign Key to Movie), CinemaID (Foreign Key to Cinema), StartTime, EndTime
5.	Booking:
o	Attributes: BookingID (Primary Key), UserID (Foreign Key to User), ShowtimeID (Foreign Key to Showtime), BookingDate, Status
6.	Payment:
o	Attributes: PaymentID (Primary Key), BookingID (Foreign Key to Booking), PaymentDate, Amount, PaymentMethod
Relationships:
1.	User - Booking (One-to-Many):
o	Each user can make multiple bookings, but each booking is made by exactly one user.
o	Direction: User (1) <---> (many) Booking
2.	Movie - Showtime (One-to-Many):
o	Each movie can have multiple showtimes, but each showtime is associated with exactly one movie.
o	Direction: Movie (1) <---> (many) Showtime
3.	Cinema - Showtime (One-to-Many):
o	Each cinema can host multiple showtimes, but each showtime occurs in exactly one cinema.
o	Direction: Cinema (1) <---> (many) Showtime
4.	Booking - Payment (One-to-One):
o	Each booking is associated with exactly one payment, and each payment is made for exactly one booking.
o	Direction: Booking (1) <----> (1) Payment

Explanation:

•	User Entity: Represents users of the system who register and book tickets. The User ID serves as the primary key, uniquely identifying each user.
•	Movie Entity: Stores information about movies available for booking, with Movie ID as the primary key. Attributes include details like title, genre, director, and release date.
•	Cinema Entity: Represents cinemas where movies are screened, identified uniquely by Cinema ID. Attributes include name, location, and seating capacity.
•	Showtime Entity: Contains details about specific showtimes for movies at cinemas. Showtime ID serves as the primary key, with attributes Start Time and End Time indicating the time window for each show.
•	Booking Entity: Records each booking made by users for specific showtimes. Booking ID uniquely identifies each booking, with attributes like Booking Date and Status (e.g., confirmed, cancelled).
•	Payment Entity: Stores payment information for each booking. Payment ID is the primary key, linked to a specific Booking ID, along with attributes like Payment Date, Amount, and Payment Method.

4.PERFORMING CRUD OPERATIONS:

![image](https://github.com/user-attachments/assets/ed1e0278-2086-4dd2-886f-b52a750dd5f0)
                              FIG 4.1: ADDING MOVIE DETAILS TO THE DATABASE

![image](https://github.com/user-attachments/assets/25e20185-c997-4e1f-b55c-1fbcc5e94a06)
                              FIG 4.2: OBTAINING MOVIE DETAILS THROUGH PRIMARY KEY MovieID

![image](https://github.com/user-attachments/assets/a0bc097c-37e1-452a-9423-327ff6d79e38)
                             FIG 4.3: DISPLAYING ALL THE DETAILS OF THE MOVIE ENTERED INTO DATABASE

![image](https://github.com/user-attachments/assets/5e75ecda-db43-448a-976f-647c29b96e67)
                             FIG 4.4: BEFORE UPDATING THE DETAILS OF MOVIEID 2 

![image](https://github.com/user-attachments/assets/113889a0-4f15-4190-8dd5-1f15f2c73b19)
                             FIG 4.5: AFTER UPDATING CAST DETAILS BY ADDING THE SANJAY DUTT IN  MOVIEID2
                             
                              

                              
                              









This repository contains the source code for Online Movie Ticket Booking System, which was a Mini Project for Database Management System (DBMS).
 
