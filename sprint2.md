# Sprint #2

## Goals for Month January 

- [] Work on a project at least 1 hr a day.
- [] Learn Object Oriented Program with Python
- [] Be more proficent in VS Code Editor
- [] Do one project a week
- [] Learn basics of React


Project base work

## January 26, 2020

## Today's Progress

**Node JS**

Key concepts to know about node.js is
    - it allows you to import and export javascript files making your web applications more modular (before ES6 came around this was not a standard practice in javascript)
    - package manager - it allows you to install packages other developers have created with ease
    - Allows you to create a server - the server is the bridge between frontend (html css) and the backend (databases, api)
        In laymens terms a server provides you something that you want or need. i.e. a resturant server will provide you food
        A server in web development will provide you retrive data, add data to a database, delete data or modify data.
        This is the service that servers are giving.  
        
        Resources:
        [Mozilla what is a web server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server)
        [Mozilla Server Side Programming](https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Introduction)

**React JS**

Learned how to create a react project:

`npx create-react-app {name of app}`

I made a mistake using an older version of this command
`npm create-react app {name-of-app}` and it caused me a lot of confusion. I was able to solve it by looking at github issue [npm i -g create-react-app not working #3423](https://github.com/facebook/create-react-app/issues/3423)

Learned file structure of a react single page project

The `public` folder is where all the static files go.
The `src` folder is where the javascript files that create your application go. There are different ways to mangage the file structure of a react project [file strcture faq](https://reactjs.org/docs/faq-structure.html).

It seems like the file structure with the Trilogy bootcamp is 
`components` folder  is a piece of your web page layout ie header, navigation, footer etc.
`style` folder where the css styles of everything is
`App.js` file where I create a page layout/template of all the components that where made in the components folder
`index.js` file is where I render the page layout from App.js into the virtual DOM




## Retrospection

### What went well

### What didn't go well



## Januay 14, 2020

## Today's Progress
Finished Part III of Miguel's Flash Mega tutorial.

Learned about environmental variables 
https://www.journaldev.com/24935/python-set-environment-variable
https://www.geeksforgeeks.org/python-os-environ-object/

What is an environmental variable?


Remember the two app entities? Here you can see both together in the same sentence. The Flask application instance is called app and is a member of the app package. The from app import app statement imports the app variable that is a member of the app package. If you find this confusing, you can rename either the package or the variable to something else.

`from app import app`

`from app` portion is talking about the package called app. A package in python is a directory that has a `__initi__.py` file. In the initi.py file is used to intialize code for the packages

`import app` is talking about the variable called app which we created in `__initi__.py `

What is a python package / what is a python module

https://www.programiz.com/python-programming/package

What is os module
https://www.pythonforbeginners.com/os/pythons-os-module

operating system 



The User class created above inherits from db.Model, a base class for all models from Flask-SQLAlchemy. 

What is a base class?

Base class is the parent class.
In python a subclass can inteherit from a super class(base class, parent class) through the syntax.
`
class DerivedClassName(BaseClassName):
    <statement-1>
    .
    .
    .
    <statement-N>
`

https://flask-sqlalchemy.palletsprojects.com/en/2.x/models/



What are migrations?

The generated migration script is now part of your project, and needs to be incorporated to source control. You are welcome to inspect the script if you are curious to see how it looks. You will find that it has two functions called upgrade() and downgrade(). The upgrade() function applies the migration, and the downgrade() function removes it. This allows Alembic to migrate the database to any point in the history, even to older versions, by using the downgrade path.

The flask db migrate command does not make any changes to the database, it just generates the migration script. To apply the changes to the database, the flask db upgrade command must be used.

SQL migrations

Migrations are files that, when run, execute SQL to perform DDL on a schema. If you perform an incorrect migration, you can rollback, or undo, that change. You can think of using migrations as an analogue to using Git for the entire project. The difference is that migrations are a form of version control specifically for the structure of your data over time.



Javascript
let has a block scope

var scope is looser than let.

https://dev.to/sarah_chima/var-let-and-const--whats-the-difference-69e

Scope essentially means where these variables are available for use. var declarations are globally scoped or function/locally scoped. It is globally scoped when a var variable is declared outside a function. This means that any variable that is declared with var outside a function block is available for use in the whole window. var is function scoped when it is declared within a function. This means that it is available and can be accessed only within that function.

## Thoughts

Learning about different terminologies is confusing when you are coming from different languages.

## Januray 4-13,2020

During this time I learned that the pep-8 standard way of create python functions is using snake case.
**snake case** is when you create varible names with a underscore or dash in between them i.e my_function. 
According to the docs it is easier to read that way. Its not a hard and fast rule. The only thing that is important is to stay consistent. 

I had a job interview that was focusing on. I brushed up on some object oriented programming.

## Today's Progress

I did not get the job but I learned that I should just focus on thing that give me joy and that I'm truly interested in.


## January 3, 2020

## Today's Progress

Today I learned how to setup a Flask Project for larger projects. I went through parts 1 and 2 in Miguel's Flask Mega Tutorial. 
 I also looked at Travesy Media's Part 1 Flask tutorial as well. 

 I learned how to create a `.flaskenv` file today. [Stack Overflow](https://stackoverflow.com/questions/49578955/is-adding-flask-env-vars-to-the-virtualenvs-activate-script-ok)

 I relearned how to make simple routes and simple templates.

 ## Thoughts

 Tomorrow I would like to explore how to intergrate bootstrap themes onto my microblog tutorial site.
 Future projects that I have in mind is to recreate my first website from Northwestern Coding Bootcamp maybe even link it with
 100 days of code blog post similar to this website https://antzee1.github.io/100-days-of-code/.

 

## January 2, 2020

## Today's Progress:

I learned about class functions, static functions and instance functions thanks to Corey Scharefer's [Youtube video series](https://www.youtube.com/watch?v=BJ-VvGyQxho) on OOP in Python. 

Instance variables are properties of an object. They are created using the `self` key word.

Class variables are shared within all instances of a class.

Class functions - In order to create a class function use the decorator `@classmethod`.  I can use this decorator to do constructor overrloading.

Instance functions are created  `def myfunction(self)` the keyword self needs to be passed in.

While class functions are created `def myfunction(cls)` the cls (stands for class) needs to be passed in.

God Object(classes) - An object that does way too much.

CRC Cards - Class Responsibility and Collaboration

I also created a Hello World app with Flask. I finally, finally! Got my VS Code IDE intergrated with the Anaconda Distro that I have installed on my laptop.

I needed to add 3 environment paths on my Windows 10 machine so I can access commands on my git terminal and not just on the Anaconda Prompt. like the followings:
`
D:\Anaconda3; 
D:\Anaconda3\Scripts; 
D:\Anaconda3\Library\bin 
`

After I did this I was able to access different Python environments.


## Thoughts

The more I learn about OOP programming the more confused I become. It's something that will take months of practice not just days.


## Links to work
Object Oriented Progamming CS_Concepts
Flask30 Day1/hello

## January 1, 2020

## Today's Progress:

Not a lot of progress was made today. The only thing that I have done is play around with the concept of inheritance in Python. I created
a python class Cylinder which is a subclass of Circle. Learned about the `super` key word and how to use polymorphism to tweak the subclass constructor to make my code DRY.

[Java OOP Inheritance Exercies](https://www.ntu.edu.sg/home/ehchua/programming/java/J3f_OOPExercises.html#zz-2.)

## Thoughts: 
Did not make much progress today. I am somewhat burnt out. Going to take a break for the new year.

## Link to work: 

## December 31, 2019

## Today's Progress:

APIE - Abstraction, polymorphism, Inheritance, encapsulation 

- Object Oriented Analysis(OOA) - Understand your problem
- Object Oriented Design(OOD) - Create/ Design your solution to the problem
- Object Oriented Programming(OOP) - Program your solution

Whenever I am doing an OOA that object in my user stories are nouns (people,place,thing,concept).
When designing a program I can use `the` test to determine if a concept is an object. It's similar to `has-a` relationship test or `is-a` relationship test.

Aggregation and Composition are similar. In both you are combining different objects to create a whole new object. They both use the `has-a` relationship test. 
But Composition is a relationship of ownership. An object has ownership over another object. Some people use `part-of` relationship or `owns-of` relationship.  While aggreation objects can be independent of each other.
[Programming Knowledge](https://www.youtube.com/watch?v=rOo_BosuJBE) has a great youtube series breaking down OOP in Python.

Learned that in Python you cannot [overload](https://stackoverflow.com/questions/6434482/python-function-overloading) methods.


## Thoughts: 
Did not make much progress today. I am somewhat burnt out. Going to take a break for the new year.

## Link to work: 



## December 30, 2019

## Today's Progress:

- Learned how to do string interpolation with python 3 using [fstring](https://realpython.com/python-f-strings/). 
Its similar to Javascript interporation witn the tick marks.

- Learned how to make [default arguments](https://www.geeksforgeeks.org/default-arguments-in-python/) in a Python class

- Learned that unit test should be [self documenting](https://stackoverflow.com/questions/1726622/how-should-unit-tests-be-documented) meaning that the name of the unit test should be descriptive

- Learned about OOP Concept called Composition,defining a new class based on existing classes. Usually signified with `HAS-A relationship` .  i.e. A car has an engine.

While inheritance you are using the same blueprint of an exisitng class but you are making simple modifications. Inheritance is signifined with a `IS-A realtionship` i.e. A sword is a weapon.

## Thoughts:
Just hoping that I can last at least 7 days on this 100 day challenge. -_-

## Link to work: 
[Python Object Oriented Programming]()