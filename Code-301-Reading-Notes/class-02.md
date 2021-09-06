### What are component lifecycle events?
The methods that you are able to use on these are called lifecycle events. 

<img src = 'https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp'>

* ###  Mounting
* ### Updating
Anytime a component is updated or state changes then it is rerendered.
These lifecycle events happen during updating in this order.

* ### Unmounting
The final phase of the lifecycle
* ### constructor()
called before it is mounted.If the component is a subclass you should call super(props)

* ### static getDerivedStateFromProps()
exists for rare cases where the state relies on changes in props over time.

* ### render()
It will examine this.props and this.state when called. 
The render function should not modify the component state
because it would cause a lot of bugs by changing the state every time it rerenders.

* ### componentDidMount()
invoked immediately after a component is mounted. 
If you need to load anything using a network request or initialize the DOM, it should go here.

* ### shouldComponentUpdate()
Setting shouldComponentUpdate() to false allows you to prevent this from happening.

* ### getSnapshotBeforeUpdate()
allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.

* ### componentDidUpdate()
This method is useful for performing network requests after a change has occurred.

* ### componentWillUnmount()
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

## Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? render

## What is the very first thing to happen in the lifecycle of React? lifecycle

## What types of things can you pass in the props?  any thing you wnt to display props you pass into a component 
## <hr>What is the big difference between props and state?
*  props you pass into a component ,handle outside of that component
* state is handle inside of that component
## <hr> When do we re-render our application ? 
* in state you can do re-render from inside the component
## <hr> What are some examples of things that we could store in state? 
*anything you want to change in application need count update from inside
*

