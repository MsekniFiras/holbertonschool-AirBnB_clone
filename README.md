
![AirBnB Clone](https://github.com/MsekniFiras/holbertonschool-AirBnB_clone/blob/main/assets/hbnb_logo.png)

## Description 

HolbertonBnB is a complete web application, integrating database storage, a back-end API, and front-end interfacing in a clone of AirBnB.

The project currently only implements the back-end console.

## Storage 

Every time the backend is initialized, HolbertonBnB instantiates an instance of FileStorage called storage. The storage object is loaded/re-loaded from any class instances stored in the JSON file file.json. As class instances are created, updated, or deleted, the storage object is used to register corresponding changes in the file.json.

## Console

The console is a command line interpreter that permits management of the backend of HolbertonBnB. It can be used to handle and manipulate all classes utilized by the application (achieved by calls on the storage object defined above).

### Using the Console

The HolbertonBnB console can be run both interactively and non-interactively. To run the console in non-interactive mode, pipe any command(s) into an execution of the file console.py at the command line.
Alternatively, to use the HolbertonBnB console in interactive mode, run the file console.py by itself.
While running in interactive mode, the console displays a prompt for input.
To quit the console, enter the command quit, or input an EOF signal (ctrl-D).

## Console Commands
The HolbertonBnB console supports the following commands:

* create
  * Usage: create <class>
Creates a new instance of a given class. The class' ID is printed and the instance is saved to the file file.json.
* show
  * Usage: show <class> <id> or <class>.show(<id>)
Prints the string representation of a class instance based on a given id.
* destroy
  * Usage: destroy <class> <id> or <class>.destroy(<id>)
Deletes a class instance based on a given id. The storage file file.json is updated accordingly.
* all
  * Usage: all or all <class> or <class>.all()
Prints the string representations of all instances of a given class. If no class name is provided, the command prints all instances of every class.
* count
  * Usage: count <class> or <class>.count()
Retrieves the number of instances of a given class.
* update
  * Usage: update <class> <id> <attribute name> "<attribute value>" or <class>.update(<id>, <attribute name>, <attribute value>) or <class>.update( <id>, <attribute dictionary>).
Updates a class instance based on a given id with a given key/value attribute pair or dictionary of attribute pairs. If update is called with a single key/value attribute pair, only "simple" attributes can be updated (ie. not id, created_at, and updated_at). However, any attribute can be updated by providing a dictionary.

## Authors
* Msekni Firas
* Youssef Saad
