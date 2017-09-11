# The Lion King Party

![King Lion picture](https://upload.wikimedia.org/wikipedia/en/2/23/LionKingCharacters.jpg)


Mufasa is organizing a party for all the animals from the forest. Everything is being managed by Rafiki and Zazu, who are now registering all the animals and their specific needs.

The entrance will be separated according to the animals needs. The ones who need to land will have an specific landing area, the ones arriving by the river or sea another area and the other ones will arrive by the main entrance.

Rafiki will be responsible for the Entrance control, while Zazu will be the DJ.

Every guest will have the right of recommending one song for the party.


## Use cases
* Mufasa may:
  * Add a new guest (Name, specie name, song)
  * Remove a guest
* Rafiki may:
  * Check if a guest is allowed by its name
  * Check which are the needs by animal name (e.g. Simba) or specie name (e.g. Lion)
* Zazu may:
  * Sort a song
  * Check which songs were already played


## Constraints
* All the strings should not be case sensitive, you can use [toUpperCase](http://docs.oracle.com/javaee/5/jstl/1.1/docs/tlddocs/fn/toUpperCase.fn.html) or [toLowerCase](http://docs.oracle.com/javaee/5/jstl/1.1/docs/tlddocs/fn/toLowerCase.fn.html) functions as you can also use [equalsIgnoreCase](https://docs.oracle.com/javase/7/docs/api/java/lang/String.html#equalsIgnoreCase(java.lang.String).
* The needs are particular for the specie and not for the particular animal, e.g. Turtles need a fresh tank of water for every now and then.
* The name of the animal is unique.
* The same menu is shown to all users, there is no need of implementing its use cases separated
* Exceptions need to be handled (e.g. when there is no more songs on the list and the user asks to sort a new one)
* According to the arrival mode, the animals have different needs:
  * Flying: The extension of its wings
  * Swimming: Where the animal will come from (sea or river)
  * Main entrance: Number of paws

* The system should have the following menu items:
  * Register guest (where you can register all the guest information)
  * Remove a guest (the system asks the name and deletes the user)
  * Sort a song (after sorted the song goes automatically for the list of played songs)
  * List played songs
  * Check if an animal is on the Guest list
  * List animal needs by animal name
  * List animal needs by specie name

## Grading:
  On a scale of 10  (yeap, 2 extra points)
  * Classes correctly implementing inheritance (3)
  * Guest adding and removing (2)    
  * List of played songs (2)
  * Working menu (2)
  * Song sorting (1)  
  * Song removing after sorting (1)
  * Verification of unique names before adding(1)

What makes you loose points:
  * Wrong OOP practices
  * Untreated exceptions
  * Wrong OOP practices
  * Not completed code
  * Wrong OOP practices
  * Wrong object or variable scope
  * Wrong OOP practices
  * Direct access to object variables
  * Wrong OOP practices


## Assignment Requirements
  * This is an individual assignment
  * In case of copied work, both students have zero grade
  * Indentation and readable code matters
  * It is requested to implement at least one inheritance
  * There is not a strict manner of implementation, use the Java Language capabilities on the best way you can.


## Recommendations

There is no need to follow it here, but here we will have some recommendations to make it easier.

* Implement Flying, Land and Swimming animals in different classes inheriting a generic class animal, where you define the general animal characteristics;

* Implement the menu inside a switch case implementation inside a do while loop;

* Put all the animals into an ArrayList
