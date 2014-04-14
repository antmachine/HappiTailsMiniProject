#Title: HappiTails

###Type:
- Mini-Project

###Prerequisites:
- Ruby
  - Objects/Classes
  - Initializer
  - Accessors
  - gets.chomp
  - Multi-file projects ('require')

###Objectives:
- Practice creating objects

###Activity:
- Work on this lab in pairs
- There is a spec folder containing tests on each model. 
  - Make sure these tests pass before moving on.

###Explanation
- You are the manager at HappiTails animal shelter. You need to manage your
shelter by storing and manipulating information about clients and animals.
- Make git commits as you finish each phase, so you can see the history

###Starter Code

- You are given some code and and files to get yourself started
  - **main.rb**
    - This is the file you will use to run your program with `ruby main.rb`
    - This is the file that will be responsible for prompting users, and taking input
  - **data.rb**
    - You do not need to write or change any code in this file but you may want to look at it
    - Once you have created your classes this file will seed your program with data
  - **animal.rb, client.rb, shelter.rb**
    - These files are for your classes
    - animal.rb has some code started for you, but the other classes you'll have to create from scratch
  - **spec**
    - These are your rspec tests to help ensure your program is working properly
    - To run all your specs run `rspec` in your teminal
    - To run a specific set of specs run `rspec spec/<filename>` in your terminal, i.e. `rspec spec/animal_spec.rb`

###Specification:
#####Objects:
- Animal:
	- An animal should have a name.
	- An animal should have an age.
	- An animal should have a gender.
	- An animal should have a species.
	- An animal can have multiple toys.

- Client:
	- A client should have a name.
	- A client should have a number of children.
	- A client should have an age.
	- A client should have a number of pets.

- Shelter:
	- The shelter should display all the clients.
	- The shelter should display all the animals.
	- The shelter should display all the animals.

- Relationships:
	- A client should be able to adopt an animal.
	- A client should be able to put an animal up for adoption

#####Phase 0

- Type `gem install coveralls` in your terminal

#####Phase 1
- Create your Animal and Cient classes **(one at a time)**
  - Your specs will tell you what methods are expected in each class
  - Make sure you make all the specs pass for a single class before moving on to the next one

#####Phase 2
- Create your Shelter Class
  - Ensure that new animals and clients can be added to the shelter
  - Make sure your specs for shelter pass before moving on

#####Phase 3
- Create a basic menu
  - At start, the user is prompted with a menu of options
  - After selecting from the menu the task the user is prompted through the entire process
  - Start with the following options
    - display all animals
    - display all clients
    - create an animal
    - create a client
  - The code for these features will go in your main.rb, and function.rb files

#####Phase 4
- Expand your menu
  - Add the following features
    - adopt an animal
    - return an animal
  - Hint: when an animal is adopted or returned it will be moved between the client and shelter object
