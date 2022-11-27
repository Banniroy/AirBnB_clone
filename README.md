This is the AirBnB clone project. It is to deploy on our server a simple copy of the AirBnB website.

Only some of the features will be implemented to cover  all fundamental concepts of the higher level programming track.

A complete web application will be built composed by:

•	A command interpreter to manipulate data without a visual interface, like in a Shell (perfect for development and debugging)

•	A website (the front-end) that shows the final product to everybody: static and dynamic

•	A database or files that store data (data = objects)

•	An API that provides a communication interface between the front-end and your data (retrieve, create, delete, update them)

The command interpreter allows the user to interact with a program using commands in the form of text lines.

In the AirBnB clone project it will be used to be able to manage the objects i.e.

•	Create a new object (ex: a new User or a new Place)

•	Retrieve an object from a file, a database etc…

•	Do operations on objects (count, compute stats, etc…)

•	Update attributes of an object

•	Destroy an object



The application will be built step by step staring with the console

The console

•	create the data model

•	manage (create, update, destroy, etc) objects via a console / command interpreter

•	store and persist objects to a file (JSON file)

The first piece is to manipulate a powerful storage system. This storage engine will give an abstraction between “My object” and “How they are stored and persisted”. This means: from the console code (the command interpreter itself) and from the front-end and RestAPI that will be built later, there will be no need to pay attention (take care) of how objects are stored.

This abstraction will also allow changing of the type of storage easily without updating all of the codebase.

The console will be a tool to validate this storage engine

Files and Storage

•	models directory will contain all classes used for the entire project. A class, called “model” in a OOP project is the representation of an object/instance.

•	tests directory will contain all unit tests.

•	console.py file is the entry point of our command interpreter.

•	models/base_model.py file is the base class of all our models. It contains common elements:

o	attributes: id, created_at and updated_at

o	methods: save() and to_json()

•	models/engine directory will contain all storage classes (using the same prototype). For the moment we will have only one: file_storage.py.



Concepts to learn

•	Unittest 

•	Python packages concept page

•	Serialization/Deserialization

•	*args, **kwargs

•	Datetime

Web static

•	learn HTML/CSS

•	create the HTML of your application

•	create template of each object

MySQL storage

•	replace the file storage by a Database storage

•	map your models to a table in database by using an O.R.M.

Web framework - templating

•	create your first web server in Python

•	make your static HTML file dynamic by using objects stored in a file or database

RESTful API

•	expose all your objects stored via a JSON web interface

•	manipulate your objects via a RESTful API

Web dynamic

•	learn JQuery

•	load objects from the client side by using your own RESTful API




