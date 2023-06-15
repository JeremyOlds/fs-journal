# CSS
in css selecting the element is the first step.

ctrl + / comments out selected code.
ctrl + / can also add in comments

hover over any command to see the syntax of the command.

specificity is important as to not ignore some of your code.

vh = viewheight. sizes things to the % size of the viewport of the screen.
em = another size for font. 1em = 16 pixels

:root {} allows you to create variables that can be used through the different css classes. example"
:root{--snow: #fd76fxe;} can call --snow to see the color

<!-- Media Rules -->
<!-- setting the screen parameters on the media -->
@media (max-width 768px){
  <!-- any rules we add in the media rule, will occur when the screen is below this size -->
  .class-call{
    undo any changes you dont wish for and add in the new changes
  }
}


commands:

color: changes the color of the font
padding: applies spacing on the inside of the selected element, up to 4 arguments in the order top bottom left right.
margin: applies spacing on the outside of the selected element
border: creates a border on the selected side of the element.
border radius: rounds teh edges of the border
text-shadow: creates a shadow on text.
display: changes teh display of the element
justify-content: used to adjust the elements within a flex display
object-fit:fits the object within the parameters of the element.
object-position: telling where to focus on the image.
box-shadow: adding shadows to elements that aren't text. such as images or divs
font-weight: change the font to be bold/thicker.
font-size:changes the font size.
background-img: allows you to set the background as an image
background size: sets the size of the background. 
background position: sets the position of the background. can be adjusted with %
background-repeat:
overflow - if anything overflows on the designated axis it creates a scroll bar.
  determine the axis with x or y and auto is the parameter.
flex-grow - allows the container to fill in the flex space between containers.

PsuedoSelectors:
hover - applies effect when mouse hovers over