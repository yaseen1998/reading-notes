# class_38
## Conditional Rendering
Conditional rendering in React works the same way conditions work in JavaScript. 
<br>
```
function Greeting(props) {
  const isLoggedIn = props.isLoggedIn;
  if (isLoggedIn) {
    return <UserGreeting />;
  }
  return <GuestGreeting />;
  ReactDOM.render(
  // Try changing to isLoggedIn={true}:
  <Greeting isLoggedIn={false} />,
  document.getElementById('root')
);
  ```
  ### Element Variables
  You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.
  <img src='https://hub.packtpub.com/wp-content/uploads/2019/02/React-webhooks-3.png'/>
  
  ### Inline If with Logical && Operator
  You may embed expressions in JSX by wrapping them in curly braces. This includes the JavaScript logical && operator. 
  ```
  function Mailbox(props) {
  const unreadMessages = props.unreadMessages;
  return (
    <div>
      <h1>Hello!</h1>
      {unreadMessages.length > 0 &&
        <h2>
          You have {unreadMessages.length} unread messages.
        </h2>
      }
    </div>
  );
}

const messages = ['React', 'Re: React', 'Re:Re: React'];
ReactDOM.render(
  <Mailbox unreadMessages={messages} />,
  document.getElementById('root')
);
```
### Inline If-Else with Conditional Operator
Another method for conditionally rendering elements inline is to use the JavaScript conditional operator condition ? true : false.
```
render() {
  const isLoggedIn = this.state.isLoggedIn;
  return (
    <div>
      The user is <b>{isLoggedIn ? 'currently' : 'not'}</b> logged in.
    </div>
  );
}
```
### Preventing Component from Rendering
In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.


