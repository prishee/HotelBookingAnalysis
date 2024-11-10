# HotelBookingAnalysis

Problem Statement
Analyze booking patterns, guest preferences, and factors influencing cancellations. Use SQL and Excel to identify trends in booking sources and revenue. Develop a Power BI dashboard for tracking booking trends and optimizing hotel operations.

Dataset Description
This dataset contains information on hotel bookings, guest details, meal preferences, booking source, room details, and reservation status.

Table Explanations
Room_Details
The Room_Details table provides information related to room reservations and changes made to them. It is associated with the Booking_Details table via the booking identifier. This table includes details about the type of room initially reserved, the type of room eventually assigned, and the number of changes made to the booking. It offers insights into room allocation dynamics and booking modifications.

Reservation_Status*
The Reservation_Status table records the status of reservations over time. It is connected to the Booking_Details table through the booking identifier. This table captures the reservation's last status (e.g., Canceled, Check-Out) and the date on which this status was recorded. It is valuable for tracking the progression of reservations and understanding their final outcomes.

Booking_Details
The Booking_Details table contains essential details related to hotel reservations. It includes a unique booking identifier and information about the type of hotel (Resort Hotel or City Hotel). Additionally, it records the booking's cancellation status (0 for not canceled, 1 for canceled), lead time (number of days between booking and arrival), year, month, week number, and day of the month of arrival. The table also captures the number of weekend and weekday nights stayed.

Guest_Info
The Guest_Info table provides insights into the guests associated with each booking. It is linked to the Booking_Details table via the booking identifier. This table records the number of adults, children, and babies accompanying the booking, offering an understanding of the composition of guests for each reservation.

Meal_And_Stay_Details
The Meal_And_Stay_Details table complements the booking information by specifying meal-related and stay-related attributes. It connects to the Booking_Details table via the booking identifier. This table includes the type of meal booked (e.g., Bed & Breakfast, Half Board), the Average Daily Rate (ADR) for the stay, the number of required car parking spaces, and the total count of special requests made by the guest.

Booking_Source_and_History
The Booking_Source_and_History table is crucial for understanding the source of bookings and the historical behavior of guests. It is connected to the Booking_Details table via the booking identifier. This table encompasses information such as the market segment (e.g., Online Travel Agents, Direct Booking), distribution channel (e.g., Online Travel Agents, Direct Booking), and whether the guest is a repeated visitor (0 for not repeated, 1 for repeated). Additionally, it records the number of previous booking cancellations, previous bookings that were not canceled, the deposit type (e.g., No Deposit, Non-Refund), the booking agent's ID, the company's ID, the number of days a booking spent on the waiting list, and the customer type (e.g., Transient, Group).
