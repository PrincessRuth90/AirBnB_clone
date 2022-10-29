# 0x00. AirBnB clone - The console

### Project Description

* This is a project to create AirBnB clone.
* [console] - contains the codes for command interpreter
* [models] - is a folder containing the Parent class (BaseModel), the subclasses (User, Amenity, State, Place, Review) and the engine folder hosting the Filestorage.
* [tests] - a folder containing all the unittest for the codes.

### Description of command line interpreter

### Installation

  git clone git@github.com:gjdame/AirBnB_clone.git
cd AirBnB_clone

### How to start it

Interactive Mode

  ~$ ./console.py
  (hbnb) help

  Documented commands (type help <topic>):
  ========================================
  EOF  help  quit

  (hbnb) 
  (hbnb) 
  (hbnb) quit
  ~$

Non Interactive Mode

  ~$ echo "help" | ./console.py
  (hbnb)

  Documented commands (type help <topic>):
  ========================================
  EOF  help  quit
  (hbnb) 
  $
  ~$ cat test_help
  help
  $
  $ cat test_help | ./console.py
  (hbnb)

  Documented commands (type help <topic>):
  ========================================
  EOF  help  quit
  (hbnb) 
  $

### How to use it

In the console.py, you will find the following commands:

* help

    - Usage: help
    - Function: displays available commands

* create

    - Usage: create <class>
    - Function: creates new object (ex. a new User, Place)

* update

    - Usage: User.update('123', {'name' : 'Jacob'})
    - Function: updates attribute of an object

* destroy
    - Usage: User.destroy('123')
    - Function: destroys specified object

* show

    - Usage: User.show('123')
    - Function: retrieves an object from a file, a database

* all

    - Uasge: User.all()
    - Function: displays all objects in class

* count

    - Usage: User.count()
    - Function: returns count of objects in specified class

* quit

    - Usage: quit
    - Function: exits command interpreter

### Examples

* Creating user

(hbnb) create User
7787b95d-69c6-4408-aaf5-2597ea3d847d                   (hbnb)
(hbnb) update User                                     ** instance id missing **
(hbnb) User.show("7787b95d-69c6-4408-aaf5-2597ea3d847d")
[User] (7787b95d-69c6-4408-aaf5-2597ea3d847d) {'created_at': datetime.datetime(2022, 10, 28, 22, 50, 1, 603228), 'id': '7787b95d-69c6-4408-aaf5-2597ea3d847d', 'updated_at': datetime.datetime(2022, 10, 28, 22, 50, 1, 603262)}                                                   (hbnb)
(hbnb) User.update("7787b95d-69c6-4408-aaf5-2597ea3d847d", "first_name", "Marcus")
(hbnb) User.show("7787b95d-69c6-4408-aaf5-2597ea3d847d")
[User] (7787b95d-69c6-4408-aaf5-2597ea3d847d) {'created_at': datetime.datetime(2022, 10, 28, 22, 50, 1, 603228), 'id': '7787b95d-69c6-4408-aaf5-2597ea3d847d', 'first_name': 'Marcus', 'updated_at': datetime.datetime(2022, 10, 28, 22, 52, 44, 51803)}                           (hbnb)
(hbnb) quit

### Unittest

* Run the entire:

    $ python3 unittest -m discover tests

* Run single file test:

    $ python3 unittest -m tests/test_console.py

### Environment

  * Language: Python3
  * OS: Ubuntu 14.04 LTS
  * Style guidelines: PEP 8

### Authors

  - Marcus Ruth
  - Ifeanyi Nze
