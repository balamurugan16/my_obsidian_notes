
## All API endpoints (Spring Boot API)

Base url : http://localhost:8080/ars/

#### Authentication
- Login : 	
	- POST `/auth/login`


- Register: 
	- POST `/auth/register`



#### Reservation
- showAvailableFlights 
	- POST `/reservation/showAvailableFlights`


- getTotalCost 
	- POST `/reservation/getTotalCost`


- reserveSeats 
	- POST `/reservation/reserveSeats`


- getMyReservations 
	- POST `/reservation/getMyReservations`



#### Cancellation
- showEligibleCancellations 
	- POST `/cancellation/show`

- cancelReservation
	- POST `/cancellation/cancel`



#### Test
- getPassenger
	- GET `/test/getPassenger/{id}`

- getFlightReservation
	- GET `/test/getFlightReservation/{id}`

- getFlight
	- GET `/test/getFlight/{id}`

- reserve
	- GET `/test/createReservation`