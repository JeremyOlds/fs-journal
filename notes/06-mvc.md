# MVC

crtl + . gives options to declare methods in other files if referenced.

Classes -

Constrructors - returns a reference from where the object is stored. when the class is called it runs the constructor

View is what is viewable on the screen. it talks to the controller
Controller - what holds the controls for the specified
service - contains the functions that the controllers will call to run actions
models/appState - holds all of our global variables

Import = pulling material from other files to be used in this file.

Export = exporting material from the file to be used in other files Example:
export class PlayersController {
  constructor(){
    insert code here
  }
}


mvc - model view controller
method - a function written inside of an object. can be polymorphic AKA it also can be a class
service - changes data out on models.
model - 
get - must return a value and they do not take in any parameters

debugger - if console is open, as soon as you hit the line of code it will open a debug window and you can run line by line

industry standard - put _ before functions that are 

listeners - on an event run a function.
exampe: AppState.on('what you are watching', function you want to run)

emitter - how to manually activate a listener
example: Appstate.emit('id that you change')

local storage -

href in html - hash reference. can be used in a(anchor) tags to navigate.

