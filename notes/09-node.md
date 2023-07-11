# Node

backend server stuff.

basic layout is similar to front end I.E creating a controller, service, etc.
to inherit things you use the 'extends' keyword. IE using the extends command on your controller to call another controller allows it to inherit another controllers options.

calling a constructor from the controller thats being inherited requires a 'super' command.
super('api/cats')
you must bring in the router from base controller into your controller. done by 'this.router'

the parameters for this is do we wish to append anything to our base super url followed by the code we wish to run.
.get('',this.getCats)


all methods you write in the controller will have three parameters, being request, response, and next

request is going to be the information that the client is requesting
response is going to be our information we want to give back to the user
next is our try/catch error handling.
getCats(req, res, next){
  try{
    res.send('example information')
  }
  catch(error){
    next(error)
  }
}

when working with serverside you must restart the server to be able to see changes. refreshing the page will not achieve this.

with .get command you can use /:id to tell node that his is something going to be supplies by the user. this can apply to the other commands as well. IE put, post, and delete.

breakpoints are debugging tools that allows you to look at code while it is running from a chosen point.
postman is a tool that mocks having a client built out and can send requests on our behalf.

.use - middleware to determine everything below the use command must use the given function/item inside the commands. IE use auth0 to



- Mongoose -

in the env file, change the connection string to your connection string from your database

domain and client id are stored in the application on mongodb

audience is stored in the api.

user password is stored in the database access where you can edit and change it.

make sure to put the domain, client, and audience in the env.js on client side as well as the server side.

Schema - a schematic for server side objects to be stored. parameters and security to show what is able to be stored.

enum - a parameter in schemas that says it must be one of the given values or it will throw an error.

once you create a schema, go to the DbContext and add a new collection for the given schema

.find() - This method will return an array of everything in the database collection. This method can be passed a filter object to return only matches of that filter. Mongoose DOC find

.findById() - This method will return one item from the database collection that has the _id passed in as an argument. Mongoose DOC findById

.create() - This method will insert an entry into the given collection from a database and return, the instance of the item from the database. Mongoose DOC create

.save() - Invoked from an object pulled from the database. If any values from the object were changed, this will save those changes to the database. Mongoose DOC save

.remove() - Invoked from an object pulled from the database. This will remove that item from the DB. Mongoose DOC remove