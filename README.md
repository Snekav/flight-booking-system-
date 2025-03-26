# 🛫 Flight & Hotel Booking System 🏨

The Flight & Hotel Booking System is a MySQL-based database project designed to manage flight and hotel reservations efficiently. It ensures seamless booking by incorporating stored procedures, functions, and triggers to automate tasks like booking validation, cost calculation, and preventing overbooking.

This system allows users to:

✅ Book flights and hotels in a single transaction.

✅ Calculate the total cost of a booking.

✅ Prevent overbooking by ensuring seat and room availability.



📂 Database Structure

Users - Stores user details (ID, name, contact details).

Flights - Stores flight details (ID, flight number, price, available seats).

Hotels - Stores hotel details (ID, hotel name, price per night, available rooms).

Bookings - Stores booking details (user ID, flight ID, hotel ID, booking date)
## Features

✅ Book a Trip - book_trip() (Stored Procedure)

Books a flight and hotel for a user.

Decreases the availability of flight seats and hotel rooms.

Ensures correct insertion of booking details.


✅ Calculate Total Cost - calculate_total_cost() (Function)

Returns the sum of the flight and hotel price for a booking.


✅ Prevent Overbooking - before_booking (Trigger)

Stops booking if no available seats or rooms exist.

Ensures proper constraints to prevent invalid bookings.

## Screenshots

![users](https://github.com/user-attachments/assets/29bdb1e9-4ddf-4b42-8686-6c625806b338)

![user bookin](https://github.com/user-attachments/assets/b3eedcdf-2721-4c42-b4d9-753140c1f022)

![flight](https://github.com/user-attachments/assets/522f5357-1609-4993-9d88-2132ce589455)

![hotel](https://github.com/user-attachments/assets/0d83d7f3-210c-4dd6-9b92-cff3fa2218b2)

![booking](https://github.com/user-attachments/assets/2444a07d-6757-476f-8a73-4bedd207034a)

![function](https://github.com/user-attachments/assets/847a4628-7414-48f3-a833-c901a49b5a43)

![procedure1](https://github.com/user-attachments/assets/45cef6d6-95d2-4d2c-894e-5057d8aece50)

![procedure 2](https://github.com/user-attachments/assets/96553709-7f76-411b-9b23-50316d272711)

![trigger](https://github.com/user-attachments/assets/1ca72661-09fd-4ff1-9e1a-6468fb27d241)



## Running Tests

🔧 How to Run the Project
Open MySQL Workbench or Command Line.

Run the project.sql file to create tables and insert sample data.

Execute stored procedures and functions to test bookings.

Example:
CALL book_trip(3, 2, 5);
SELECT calculate_total_cost(2, 5);


## Demo

https://github.com/user-attachments/assets/ed8f2ace-ee81-4141-b5b9-c6211bfd4e7e


