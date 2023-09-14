# Week 4 Assessment

### Setup
* Fork and clone this repository
* Open your forked repo in Visual Studio.
* Complete the two exercises and the questions

## Exercise 1: Inheritance and Dependency Injection (8 points)

Open up `Program.cs` and run your program. It should run with no errors, if you get an error reach out to your instructor.

This exercise involves some refactoring and some new features.

**Step 1:** Currently there are two classess `Student` and `Teacher` that have a lot of repeated code between them. Create a new class `Person` that will be the base class. Then update `Student` and `Teacher` to be derived from `Person`. Include as much in your `Person` class as you can to keep your code DRY (Don't Repeat Yourself). 

**Testing Step 1:** Uncomment the code under "Step 1:" in the Main method. That code should now run without error.

**Step 2:** Implement a new class called `School` that uses dependency injection and takes in a list of people as a dependency. Implement a method called `ListBirthdays` in your school class that calls the `GetBirthday` method and prints to the console each student and teacher's birthday.

**Testing Step 2:** Uncomment the code under "Step 2:" in the Main method. That code should now run without error and output a bunch of names and birthdays.

Ungraded extra challenge: If you have time, improve the way the birthdays are output. Can you group them by month or by Student/Teacher?

### Exercise 2: Interfaces (4 points)
Open up `InterfacePractice.cs`. You should not need to run this file, you will just edit it.

**Step 1:** Take a look at the two classes `Car` and `Bicycle`. They both implement an interface called `InterfaceNameHere`. Replace all three uses of `InterfaceNameHere` with a fitting name for this interface.

**Step 2:** The interface has already been created for you on line 5. Fill in the details for any methods and/or properties that make sense based on the two classes implementing this interface.

## Questions (8 points)

Edit this file with your answers.

1. What are some of the benefits of using inheritance? (1 point)
    * Inheritance is useful for many reasons. One of the biggest reasons being the ability to reuse code such as properties and
	methods in different classes. It also serves as a tool to extend functionality of existing classes to new ones.
2. What might be some of the disadvantages of using inheritance? (1 point)
    * If changes were to be made to the base class, it would affect all of the derived classes. It can also become very complex 
	if mulitple levels of child classes are being created.

3. How would you describe the difference between the base class and the derived class when working with inheritance? (1 point)
	* A base class holds attributes and methods that will be inherited by other classes. A derived class inherits attributes 
	and methods from a base class.

4.  What happens if you define the same method in the parent class and the child class? (1 point)
	*  Defining the same method in a child class that's in the parent class is method overriding. If a method already exists in
	a parent class and is defined in a derived class, the method will be overwritten and have a new use in that class.

5. In your own words, how would you define an Interface? (1 point)
    * An interface is a contract that holds attributes without a value and methods without a behavior. 
	The attributes and methods are given values and behaviors when a class implements the interface.

6. Does a class implementing an interface need to implement all of the methods in that interface? Why or why not? (1 point)
    * A class is required to implement all of the methods defined in an interface. This is because an interface does not provide values
	or behaviors for its members.

7. Both Inheritance and Interfaces use the `:` symbol after a class name. If you're looking at a class, what's one thing that can help you determine if the class is implementing an interface of extending a base class? (1 point)
	*  It is convention to name an interface with an I at the beginning to identify whether it is an interface or not.

8. If asked in an interview, how would you describe the purpose of the IOC container in a .NET application? (1 point)
	* The IoC container automatically injects dependencies. 


## Rubric

This assessment has a total of 20 points.  A score of 15 or higher is a pass.

As a reminder, this assessment is for students and instructors to determine if there are any areas that need additional reinforcement!
