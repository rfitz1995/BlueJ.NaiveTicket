# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

First you need to FORK this repo into your account, then you need to CLONE that foreked repo, the one in your account. 
When you are finished with your code, be sure to ADD/COMMIT and PUSH your code to your repo.

Use the URL from your repo as the submission to the portal. 

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket?
	* the balance is zero

### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior?
		* it adds all the money up that you have previously entered and it continues to add money on top of what was previously entered
	* What happens if you insert too much money into the machine – do you receive any refund?
		* nothing, you do not receive a refund and the money is just extra 
	* What happens if you do not insert enough and then try to print a ticket?
		* nothing happens

### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine.
	* Does the printed ticket look different?
		* no it looks the same just with different numbers 	

### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part.
	* public class Student {
	 }
	* public class LabClass{
	}
### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class?
	* yes the order matters

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram?
		* yes it went from solid to crossing lines on the class diagram
	* What error message do you get when you now press the compile button?
		* it says illegal start of expression
	* Do you think this message clearly explains what is wrong?
		* not really, it tells me that the expression cannot be started that way but does not tell me what I could change it to 

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class.
	* yes it is possible and the code still compiles 

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
	* Hint: There is only one constructor in the class.
		* fields - price, balance, total, ticketNumber
		* constructors - TicketMachine(Integer ticketCost)
		* methods - getPrice, getBalance, insertMoney, printTicket, getTicketNumber
### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class?
	* the constructor has the same name as the class as which is 

### Exercise 2.11
* What do you think is the type of each of the following fields?
	* int, string, string 
```java
private int count;
private Student representative;
private Server host;
```

### Exercise 2.12
* What are the names of the following fields?
	* alive, tutor, game
```java
private boolean alive;
private Person tutor;
private Game game;
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in?
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible?
	* Check by pressing the compile button to see if there is an error message.
	* Make sure that you reinstantiate the original version after your experiments!
		* the code will not compile if it is in any other order besides the one listed above. You will receive an error message.

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration?
* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.
	* yes it is always necessary to have a semicolon at the end of a field declaration because this is how java ends a certain portion of code. Without the semicolon the program would not know where certain code ends and others begin, since whitespace is irrelevant. 


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.
	* private int status 

### Exercise 2.16
* To what class does the following constructor belong?
	* Student 
```
public Student(String name)
```

### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
	* it has two parameters: title and price 
	* their types are string and double
```
public Book(String title, double price)
```

### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be?
* Can you assume anything about the names of its fields?
	*  string type for author or int for date published
	*  depending on the info given for each class field you may be able to determine wheter the book was purchased or even borrowed from a library if the interger is a price or a date to return

READ upto and INCLUDING section 2.15 of this chapter.
