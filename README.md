# 0x00. AirBnB clone - The console

The image shows the basic concept for this project

! [airbnb_concept.png]

## Project Description

* This is a project to create AirBnB clone.
* [console] - contains the codes for command interpreter
* [models] - is a folder containing the Parent class (BaseModel), the subclasses (User, Amenity, State, Place, Review) and the engine folder hosting the Filestorage.
* [tests] - a folder containing all the unittest for the codes.

## Description of command line interpreter

### Installation

[git clone git@github.com:gjdame/AirBnB_clone.git
cd AirBnB_clone]

### How to start it

Interactive Mode

[$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$]

Non Interactive Mode

[$ echo "help" | ./console.py
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
$]

### How to use it

In the console.py, you will find the following commands:

* [help]

    - Usage: [help]
    - Function: [displays available commands]

* [create]

    - Usage: [create <class>]
    - Function: [creates new object (ex. a new User, Place)]

* [update]

    - Usage: [User.update('123', {'name' : 'Jacob'})]
    - Function: [updates attribute of an object]

* [destroy]
    - Usage: [User.destroy('123')]
    - Function: [destroys specified object]

* [show]

    - Usage: [User.show('123')]
    - Function: [retrieves an object from a file, a database]

* [all]

    - Uasge: [User.all()]
    - Function: [displays all objects in class]

* [count]

    - Usage: [User.count()]
    - Function: [returns count of objects in specified class]

* [quit]

    - Usage: [quit]
    - Function: [exits command interpreter]

### Examples

* Creating user

### Unittest

* Run the entire:

  [$ python3 unittest -m discover tests]

* Run single file test:

  [$ python3 unittest -m tests/test_console.py]

### Authors

  - Marcus Ruth
  - Ifeanyi Nze
