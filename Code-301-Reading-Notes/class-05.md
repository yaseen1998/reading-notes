## How would you break a mock into a component heirarchy?
*  draw boxes around every component in the mock and give them all names.
* your model was built correctly

## What is the single responsibility principle and how does it apply to components?
 that is, a component should ideally only do one thing. If it ends up growing, 
 it should be decomposed into smaller subcomponents.
 
 ## What does it mean to build a ‘static’ version of your application ?
  renders your data model, you’ll want to build components that reuse other components 
  and pass data using props. props are a way of passing data from parent to child.
  If you’re familiar with the concept of state, don’t use state at all to build this static version.
  State is reserved only for interactivity, that is, data that changes over time. 
  Since this is a static version of the app, you don’t need it.
  
  ## Once you have a static application, what do you need to add?
  * build top-down
  * bottom-up
  * FilterableProductTable
  * ProductRow
  
  ## What are the three questions you can ask to determine if something is state?
* 1- Is it passed in from a parent via props? If so, it probably isn’t state.
* 2- Does it remain unchanged over time? If so, it probably isn’t state.
* 3- Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?
by follow this step :
* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state

## Things I want to know more about
what static application and state live 
