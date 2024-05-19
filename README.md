#Airbnb Clone Console 

Project Overview

The objective of this project is to deploy a simplified version of the AirBnB website on a server. While it won't encompass all features, it will cover essential concepts of the higher-level programming track.

Initial Task: Develop a command interpreter to manage AirBnB objects.
This initial step is pivotal as it forms the foundation for subsequent projects. It integrates with HTML/CSS templating, database storage, API, and front-end development.

What is a Command Interpreter?
Think of it like the Shell, but tailored to a specific purpose. In our case, it's designed to manage project objects:

Creating new objects (e.g., User, Place)
Retrieving objects from files, databases, etc.
Performing operations on objects (e.g., counting, computing stats)
Updating object attributes
Deleting objects
Execution:
You can interact in both interactive and non-interactive modes:

Interactive mode:

bash
Copy code
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
Non-interactive mode:

bash
Copy code
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
Commands:

create: Create an object
show: Display an object based on ID
destroy: Remove an object
all: Show all objects of one type or all types
update: Modify an instance based on class name and ID
quit/EOF: Exit the console
help: View command descriptions
To initiate the console, type in the shell:

shell
Copy code
AirBnB_clone$ ./console.py
(hbnb)
Functionalities:

Create: Use format "create <class>" (e.g., create BaseModel)
Show: Display an instance based on class name and ID (e.g., show BaseModel 1234-1234-1234)
Destroy: Delete an instance of an object using "destroy <class> <id>" (e.g., destroy BaseModel 1234-1234-1234)
All: View all instances or of a specific class (e.g., all or all State)
Update: Modify an instance based on class name, ID, and attributes (e.g., update BaseModel 1234-1234-1234 email "aibnb@holbertonschool.com")
Quit: Exit the console
Help: View command descriptions (e.g., help or help quit)
Supported classes:

BaseModel
User
State
City
Amenity
Place
Review
Author: Kanisa Rebecca & Daniel Marial
