# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > Create, Update, read, destroy

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > post is to create, put is to update, get is to read, delete is to destroy

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > object relational mapping. mongoose

04. Which two `HTTP` request types include a body?

  > Put and Create

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > Asyncronous, Synchronous

06. What are the three types of data relationships? Provide an example of each.

  > one to one, person and SSN. one person only has one SSN and vice versa
  one to many, blog to posts. one blog can have many posts but the posts are all part of a single blog
  many to many, authors to books. many authors can write a book and many books can be written by an author

07. What is middleware?

  > an application that serves as a bridge between a database and application

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > Request and Response

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > ?tag=winter

10. What is a ***virtual property***?

  > Additional fields for a given model
