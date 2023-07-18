# Vue
use vue-starter under the bcw tools when creating new projects.
download

App.vue holds html, javascript, and css in a single file
pages are loaded in equivilancy to views.
in javascript seaction of a vue page: anything under setup is considered private, while everything in return is considered public.

logger.log - use instead of console.log , same effects as console so you can say logger.error and the rest.
Vue commands:
v-on: this is put before to use a vue command, @ can be used in place of v-on
v-on:click - acts as onclick
computed(()) - takes in a function that returns what you want.
regular return = computed(() => {return appstate.cheese}) - returning a series of values or functions
implied return = computed(() => appstate.cheese) - returns a singular value.

v-for - this is a for/and loop that can be put in the html
v-for='upgrade in upgrades'
v-if - if conditional that will only render html if true.
key - must be a unique property to help vue know what it is looking at. can use a colon to bind the property

data binding - everything written inside the parenthesis is considered javascript.

onMounted - computed that runs when the page loads.
onUnmounted - computed that runs when component is no longer mounted


router-link - go in tandem with router.js and view
useRoute() - gives information about current route.

v-model - sets up two way data binding between the html and the script

