### Tables
1. Flight Details (25 flights) Hardcoded

note: If admin portal is available, the date and time of departure and arrival can be edited by the admin for the future trips

- add pricing for business and economy class

![[Flights table schema.png]]
2. Passenger Details
 
- Add password
- Passenger id starts with 1000
- Login validation is done with email and password

![[Passenger table schema.png]]

```sql
CREATE TABLE passengers (
	passenger_id INTEGER PRIMARY KEY AUTO_INCREMENT,
	first_name VARCHAR(20) NOT NULL,
	last_name VARCHAR(20) NOT NULL.
	email VARCHAR(30) UNIQUE NOT NULL,
	phone_number VARCHAR(15) UNIQUE NOT NULL,
	address VARCHAR(50),
);
```
3. Flight Reservation

The insert operation in this table will only happen after the payment is done and a confirmation number will be generated.
![[Flight reservation table schema.png]]


Table entries
- Indian airlines only (7 airlines)
- Indian cities (12 cities)
- Flight code initials of the airlines + number
- Passeger id starts with 1000
- flight reservation confirmation number in JAVA



Airlines:
Air India (AI), Spice Jet (SJ), Vistara (VT),  IndiGo (IG), Go First (GF) 


Extra tables

- Airlines and their planes (Hardcoded)
- 