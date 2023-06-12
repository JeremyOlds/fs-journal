# JavaScript

creating the link to javascript files should always be in the bottom of your body.
example:
<!-- <script src ="app.js"><script> -->
use camelscript. camelscript is the act of creating a variable with the first word being lowercase while every subsequent word is capitalized.

let - allows you to create a variable
const - creates a variable that cannot be changed once declared.
boolean - variable that only accepts true or false values.
number - variable that only holds a number.

${} - string interpolation. needs the back ticks `` to use string interpolation. allows you to use javascript in a string.
usage of backticks `` in strings allows you to add quotes or double quotes to it without errors.

objects - a way to store multiple pieces of data in one piece of data.
example:
% bad example
let catName = "gopher"
let catAge = 2
let catIsHungry = true
% good example
let cat = {
  name: "Gopher",
  age: 2
  isHungry :
}

to pull elements from na object you need to use . notation; IE: cat.isHungry pulls isHungry from cat.

arrays - collection of data (keep it the same datatype ya dingus)

functions - block of code that can be run manually as many times as neccessary.

function sayHello() {

}

console.group() and console.groupEnd() - allows you to group up console logs 