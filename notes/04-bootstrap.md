# Bootstrap
grid system: 
start with a container that will hold all the grids.
rows act like flexbox containers withing grids
col is a column that you can put in rows. cols are sized on a base 12 to take up the row

https://getbootstrap.com/docs/5.3/getting-started/introduction/
bootstrap documentaion to find info.

bringing in bootstrap:
link:bs5

dont put margin on the x axis on your columns, it'll break the formatting. Padding is fine.

utility classes:
class "container"
class "row"
class "col"

justify-content-between
justify-content-center
d-flex = display flex utility
m-4 = m is for the margin utility the -# is for teh sizing. 
mx
container-fluid = same as a container but removes the margin from base container.
bg-(color) = background color settings. utility command is bg- and type in whatever color you want based on bootstrap colors.
p-1-5 = adds padding to element. scales in 1 to 5 you can add x for the x axis, y for the y axis, e for just the end.
fs-1-5 = changes the size of the font 
align-items-center = aligns items to the center.
fw-bold = changes the font weight. bold is just a parameter.
d-none = never display
d-md-block = on medium screens or lager
text-center = centers the text on the
sticky-top = sticks the element to its direct parent.
img-fluid = command that tells the image is not allowed to spill outside its column
rounded = adds rounding to the border
btn = changes styling of a button. can also use btn-outline-(color) to make an outline button that highlights.
order = sets the order