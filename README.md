# AirBnB Clone (AirBnB_clone_v4) - The Console

The console is the first segment of the AirBnB_clone_v4 project at Alx School's that will collectively cover fundamental concepts of higher level programming. The goal of AirBnB_clone_v4 project is to eventually deploy our server a simple copy of the AirBnB Website (HBnB). A command interpreter is created in this segment to manage objects for the AirBnB_clone_v4 website.

## Functionalities of this command interpreter:

- Create a new object (ex: a new User or a new Place)
- Retrieve an object from a file, a database, etc.
- Do operations on objects (count, compute stats, etc.)
- Update attributes of an object
- Destroy an object

## Table of Contents

- [Environment](#environment)
- [Installation](#installation)
- [File Descriptions](#file-descriptions)
- [Bugs](#bugs)
- [Authors](#authors)
- [License](#license)

## Environment

This project is interpreted/tested on Ubuntu 20.04 LTS using Python 3 (version 3.4.3).

## Installation

- Clone this repository: `git clone "https://github.com/solomonk6/AirBnB_clone.git"`
- Access the AirBnb directory: `cd AirBnB_clone`
- Run the console (interactively): `./console` and enter commands
- Run the console (non-interactively): `echo "<command>" | ./console.py`

## File Descriptions

- [console.py](console.py): The console contains the entry point of the command interpreter. List of commands this console currently supports:
  - `EOF`: exits the console 
  - `quit`: exits the console
  - `<emptyline>`: overwrites the default emptyline method and does nothing
  - `create`: Creates a new instance of `BaseModel`, saves it (to the JSON file), and prints the id
  - `destroy`: Deletes an instance based on the class name and id (save the change into the JSON file)
  - `show`: Prints the string representation of an instance based on the class name and id
  - `all`: Prints all string representations of all instances based or not on the class name
  - `update`: Updates an instance based on the class name and id by adding or updating an attribute (save the change into the JSON file)

- [models/](/models): Directory contains classes used for this project:
  - [base_model.py](/models/base_model.py): The BaseModel class from which future classes will be derived
  - [amenity.py](/models/amenity.py): Class for amenities
  - [city.py](/models/city.py): Class for city
  - [place.py](/models/place.py): Class for place
  - [review.py](/models/review.py): Class for review
  - [state.py](/models/state.py): Class for state
  - [user.py](/models/user.py): Class for user

- [models/engine/](/models/engine): Directory contains the File Storage class that handles JSON serialization and deserialization:
  - [file_storage.py](/models/engine/file_storage.py): Serializes instances to a JSON file & deserializes back to instances

- [tests/](/tests): Directory contains all unit test cases for this project:
  - [/test_models/test_base_model.py](/tests/test_models/test_base_model.py): Contains the TestBaseModel and TestBaseModelDocs classes
  - [/test_models/test_amenity.py](/tests/test_models/test_amenity.py): Contains the TestAmenityDocs class
  - [/test_models/test_city.py](/tests/test_models/test_city.py): Contains the TestCityDocs class
  - [/test_models/test_file_storage.py](/tests/test_models/test_file_storage.py): Contains the TestFileStorageDocs class
  - [/test_models/test_place.py](/tests/test_models/test_place.py): Contains the TestPlaceDoc class
  - [/test_models/test_review.py](/tests/test_models/test_review.py): Contains the TestReviewDocs class
  - [/test_models/test_state.py](/tests/test_models/test_state.py): Contains the TestStateDocs class
  - [/test_models/test_user.py](/tests/test_models/test_user.py): Contains the TestUserDocs class


## Bugs
No known bugs at this time. 

## Author
Solomon Kassa - [Github](https://github.com/solomonkassa) / 

