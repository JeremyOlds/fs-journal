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

with .get command you can use /:id to tell node that his is something going to be supplies by the user.

breakpoints are debugging tools that allows you to look at code while it is running from a chosen point.
postman is a tool that mocks having a client built out and can send requests on our behalf.

