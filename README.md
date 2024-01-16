# AirBnB clone

![AirBnb_Clone_Holberton_School_Logo](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/65f4a1dd9c51265f49d0.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=408ddae065f791da4c740f03baa6766b20dea3b025332268110aa20e1e8a029d)

A simple copy of the AirBnB website.
a complete web application composed by:

    A command interpreter to manipulate data without a visual interface, like in a Shell (perfect for development and debugging)
    A website (the front-end) that shows the final product to everybody: static and dynamic
    A database or files that store data (data = objects)
    An API that provides a communication interface between the front-end and your data (retrieve, create, delete, update them)

## Concepts to learn

    Unittest - and please work all together on tests cases
    Python packages concept page
    Serialization/Deserialization
    *args, **kwargs
    datetime
    More coming soon!

## Steps

You won’t build this application all at once, but step by step.

Each step will link to a concept:

### The console

    create your data model
    manage (create, update, destroy, etc) objects via a console / command interpreter
    store and persist objects to a file (JSON file)

The first piece is to manipulate a powerful storage system. This storage engine will give us an abstraction between “My object” and “How they are stored and persisted”. This means: from your console code (the command interpreter itself) and from the front-end and RestAPI you will build later, you won’t have to pay attention (take care) of how your objects are stored.

This abstraction will also allow you to change the type of storage easily without updating all of your codebase.

The console will be a tool to validate this storage engine

![Console Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/815046647d23428a14ca.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5cc298d432c8101da26650586de9391e4e1fb3c70007150505dfa4f8cced9b3c)

### Web static

    learn HTML/CSS
    create the HTML of your application
    create template of each object

![Web Static Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/87c01524ada6080f40fc.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=cca94785ec31b0ae9324c88adedee80f267401e5e8cce229566744386df9a5e5)

### MySQL storage

    replace the file storage by a Database storage
    map your models to a table in database by using an O.R.M.

![MySQL Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/5284383714459fa68841.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=aa9fce67c71bed17d67219962000932bbcd104630a2843c11e0ee1f190892ebc)

### Web framework - templating

    create your first web server in Python
    make your static HTML file dynamic by using objects stored in a file or database

![Web FrameWork Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/cb778ec8a13acecb53ef.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f3af32032de52175c483da871dab30d4f00b322260130a25d7e8f2fb0a28dcb9)

### RESTful API

    expose all your objects stored via a JSON web interface
    manipulate your objects via a RESTful API

![RESTful API Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/06fccc41df40ab8f9d49.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b37964a8aa01d30d22e058e88e2f0b8fad5b7b4697f23215bf8e0cc54864bb9c)

### Web dynamic

    learn JQuery
    load objects from the client side by using your own RESTful API

![Web Dynamic Part Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/d2d06462824fab5846f3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2f91520588437829ccc4f71289bd779560cd781bfa2641b5a5a7a3539f5a733a)

### Files and Directories

    models directory will contain all classes used for the entire project. A class, called “model” in a OOP project is the representation of an object/instance.
    tests directory will contain all unit tests.
    console.py file is the entry point of our command interpreter.
    models/base_model.py file is the base class of all our models. It contains common elements:
        attributes: id, created_at and updated_at
        methods: save() and to_json()
    models/engine directory will contain all storage classes (using the same prototype). For the moment you will have only one: file_storage.py.

### Storage

Persistency is really important for a web application. It means: every time your program is executed, it starts with all objects previously created from another execution. Without persistency, all the work done in a previous execution won’t be saved and will be gone.

In this project, you will manipulate 2 types of storage: file and database. For the moment, you will focus on file.

Why separate “storage management” from “model”? It’s to make your models modular and independent. With this architecture, you can easily replace your storage system without re-coding everything everywhere.

You will always use class attributes for any object. Why not instance attributes? For 3 reasons:

    Provide easy class description: everybody will be able to see quickly what a model should contain (which attributes, etc…)
    Provide default value of any attribute
    In the future, provide the same model behavior for file storage or database storage

#### How can I store my instances?

That’s a good question. So let’s take a look at this code:

class Student():
    def __init__(self, name):
        self.name = name

students = []
s = Student("John")
students.append(s)

Here, I’m creating a student and store it in a list. But after this program execution, my Student instance doesn’t exist anymore.

class Student():
    def __init__(self, name):
        self.name = name

students = reload() # recreate the list of Student objects from a file
s = Student("John")
students.append(s)
save(students) # save all Student objects to a file

Nice!

But how it works?

First, let’s look at save(students):

    Can I write each Student object to a file => NO, it will be the memory representation of the object. For another program execution, this memory representation can’t be reloaded.
    Can I write each Student.name to a file => YES, but imagine you have other attributes to describe Student? It would start to be become too complex.

The best solution is to convert this list of Student objects to a JSON representation.

Why JSON? Because it’s a standard representation of object. It allows us to share this data with other developers, be human readable, but mainly to be understood by another language/program.

Example:

    My Python program creates Student objects and saves them to a JSON file
    Another Javascript program can read this JSON file and manipulate its own Student class/representation

And the reload()? now you know the file is a JSON file representing all Student objects. So reload() has to read the file, parse the JSON string, and re-create Student objects based on this data-structure.

#### File storage == JSON serialization

For this first step, you have to write in a file all your objects/instances created/updated in your command interpreter and restore them when you start it. You can’t store and restore a Python instance of a class as “Bytes”, the only way is to convert it to a serializable data structure:

    convert an instance to Python built in serializable data structure (list, dict, number and string) - for us it will be the method my_instance.to_json() to retrieve a dictionary
    convert this data structure to a string (JSON format, but it can be YAML, XML, CSV…) - for us it will be a my_string = JSON.dumps(my_dict)
    write this string to a file on disk

And the process of deserialization?

The same but in the other way:

    read a string from a file on disk
    convert this string to a data structure. This string is a JSON representation, so it’s easy to convert - for us it will be a my_dict = JSON.loads(my_string)
    convert this data structure to instance - for us it will be a my_instance = MyObject(my_dict)

### Data Diagram 

![Data Diagram Image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/99e1a8f2be8c09d5ce5ac321e8cf39f0917f8db5.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240116%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240116T172850Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=1d2f30383692e1b0ccce53a5512b87fa7f05b282c59adadaa194d2bedb15c0d1)

