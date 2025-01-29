# OOP-assignment-1
A Flight and Passenger Management System
The Flight and Passenger Management System is designed to manage flight details and the
passengers who book these flights. This system supports functionalities for adding and
searching for passengers, upgrading ticket classes, and dynamically managing passenger
capacity.
Requirements:
1. Flight Management. To manage flights, you need to create a flight class that would
include the following flight info:
o The number of the flight, the flight’s destination, its departure time along with its
time zone, its seating capacity, the current number of booked seats, the seating
plan, and the list of passenger names. You need to choose the attribute types
appropriately.
o You also need to dynamically create a two-dimensional array for the seating plan
of that flight, based on the flight’s seating capacity. Such seating plan should

display the reserved/non-reserved seats within the flight, and should be updated
upon adding passengers to the flight, and upon removing passengers from the
flight. (Hint: Make your own assumptions about the number of seats per row
within the flights)
o Additionally, the list of passengers names needs to be a dynamically allocated
array of strings.

2. Furthermore, the flight class should provide member functions for each the following
functionalities:
o Adding passengers to a flight: The function should receive a number of
passengers to be added, along with an array with their passenger objects, and
would update the flight info accordingly. This function should trigger array
resizing if necessary.
o Search for a passenger by name, confirming whether he is present on the flight
or not
o Search for a specific seat number, within the seating plan, to confirm whether it is
booked or not.
o Display all of the flight details.
3. Additionally, the flight class should support the following features:
o A three-argument Constructor: Upon receiving the flight’s capacity, destination,
and number, initializes the remaining flight attributes and allocates memory for
the dynamic arrays appropriately.
o Friend operator<< Overloading: Allows for the easy printing of all of flight details
including its seating plan, and its passengers’ names.
o Operator++ overloading: Allows expanding the flight capacity by adding a new
row of seats to the flight. The ++ operator should be supported using the prefix
notation.
o Operator +=overloading: Allows adding a passenger to the flight. It would
receive a passenger object as an argument, and would extract the needed data
from that object to add the passenger to the flight, and properly update the flight
accordingly.
o Operator--overloading: Allows removing an existing passenger from the flight.
This should be the last added passenger. The -- operator should be supported
using the postfix notation.
o Operator -= that would take an integer argument and would remove the
equivalent number of passengers from the flight.
o An operation removePassenger(...) that would take a passenger object, and
would remove that specific from the flight.
o A copy constructor that allows deep copying of all of the flight’s information
from one flight object to another.
o Destructor: Cleans up dynamically allocated memory upon flight object
destruction.
o Note: All operations/functionality should reflect as appropriate within the system’s
state.

3. Passenger Management: To manage passengers, you need to create a Passenger
class that would include the following info: the name of the passenger, and the
passenger’s ID
4. Furthermore, the Passenger class should provide member functions for each the
following functionalities:
o Display passenger details.

o Maintain a count of total passengers across the system. A static function that
would return the total number of passengers currently present within the system
(even if across the different flights).
o Operator >> overloading to receive all the passenger info from
o A two-argument constructor that initializes the passenger with given passenger
info.
o Destructor: Updates the total number of passengers and outputs a message
upon passenger object destruction.

Write a main program that demonstrates all the above features. Enrich your classes and
your main program with comments to clarify how each of the above features map to your
source code. If a feature is not illustrated within your main program,
