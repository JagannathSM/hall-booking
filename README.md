# TASK DETAILS 

<ul>
  <li>Create an Express Server</li>
  <li>Create end-points and write logics</li>
  <li>Can use local variable to store data</li>
  <li>Write API documentation in POSTMAN Docs</li>
</ul>

<b>RENDER URL :</b> https://hall-booking-xxjb.onrender.com

# TASK REQUIREMENTS

<ol>
  <li><b>Create a room with</b>
    <ul>
        <li>No. of seats available</li>
        <li>Amenities in the room</li>
        <li>Price for 1 hrs</li>
      </ul>
  </li>
  <li><b>Booking a room with</b>
    <ul>
        <li>Customer name</li>
        <li>Date</li>
        <li>Start Time</li>
        <li>End Time</li>
        <li>Room Name</li>
      </ul>
  </li>
  <li><b>List all rooms with booked data</b>
    <ul>
        <li>Room Name</li>
        <li>Booked status</li>
        <li>Customer name</li>
        <li>Date</li>
        <li>Start Time</li>
        <li>End Time</li>
      </ul>
  </li>
  <li><b>List all customer with booked data</b>
    <ul>
        <li>Customer name</li>
        <li>Room Name</li>
        <li>Date</li>
        <li>Start Time</li>
        <li>End Time</li>
      </ul>
  </li>
  <li><b>List how many times customer booked room with below details</b>
    <ul>
        <li>Customer name</li>
        <li>Room Name</li>
        <li>Date</li>
        <li>Start Time</li>
        <li>End Time</li>
        <li>Booking ID</li>
        <li>Booking Date</li>
        <li>Booking Status</li>
      </ul>
  </li>
</ol>

# END POINTS / DOCUMENTATION

1. GET METHOD :
   1. /get-rooms --> To collect all rooms details
   2. /all-booked-rooms --> To collect the all booked rooms details
   3. /all-customers --> To collect all customers details
   4. /booking-customer-data --> To get particular customer data (required customer_name from Query Params)

2. POST METHOD :
   1. /add-room --> To add more rooms.
     	<ul>
		<li>Data required in Query Params - room_name, seates_available, aminities, price. (all data required from user)</li>
		<li>Conditions :</li>
		<ul>
			<li>Should not add same room name again.</li>
		</ul>
	</ul>      
   2. /book-room --> To book room. [CONDITIONS : Should not book the already booked room for that time period]
	<ul>
		<li>Data required in Query Params - room_name, customer_name, date, start_time, end_time. (all data required from user)</li>
		<li>Conditions :</li>
		<ul>
			<li>date format should be Ex. 2024-12-24</li>
			<li>start_time & end_time format should be in 24-hrs Ex. start_time = 12:00 & end_time = 14:00 </li>
		</ul>
	</ul>
