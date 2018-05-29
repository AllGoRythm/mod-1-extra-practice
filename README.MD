
##Passenger
###Attributes
* Name
* Age (integer)
* Destination

###Methods
* Passenger.all
	- should return all of the passenger instances
* Passenger.find_by_name(name)
	- given a string of a full name, returns the first passenger whose full name matches
* Passenger.find_all_by_destination(destination)
	- given a string of a destination, returns an array containing all passengers with that destination
* Passenger.all_ages
	- should return an array of all of the passenger ages
* Passenger.youngest_passenger
	- should return the youngest passenger
* Passenger.eldest_passenger
	- should return the eldest passenger
* Passenger#add_carriage(donkey, speed)
	- given a donkey object and carriage speed (as an integer), creates a new carriage and associates it with that passenger and donkey. A Carriage belongs to a Passenger and belongs to a Donkey

##Carriage
###Attributes
* Passenger
* Donkey
* Speed (integer)

###Methods
* Carriage.all
  * returns all of the carriages
* Carriage#passenger
  * returns the passenger object for that given carriage
* Carriage#donkey
  * returns the donkey object for that given carriage
* Carriage#fastest_carriage
  * returns the fasted carriage

##Donkey
* Name
* Weight (integer)
* Friendly (boolean)

###Methods
* Donkey.all
  * returns an array of all donkeys
* Donkey.find_by_name(name)
  * given a string of donkey name, returns the first donkey that matches
* Donkey#carriages
  * returns an array of all carriages for that donkey
* Donkey#friendly_donkeys
  * returns an array of friendly donkeys
* Donkey#heaviest_donkey
  * returns the heaviest donkey instance
* Donkey#passengers
  * returns all of passengers who have written carriages of that donkey. A `Donkey` has many `Passengers` and a `Passenger` has many `Donkeys`
