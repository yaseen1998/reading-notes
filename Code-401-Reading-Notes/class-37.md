# class-37
## React
### Introducing JSX
`const element = <h1>Hello, world!</h1>;`<br>
It is called JSX, and it is a syntax extension to JavaScript.
<br>
#### Why JSX?
React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.
<br>
#### Embedding Expressions in JSX
<img src ='https://cdn-images-1.medium.com/max/2000/0*btUO9W4LD1jyiBNq'/>
#### Specifying Attributes with JSX
You may also use curly braces to embed a JavaScript expression in an attribute:

`const element = <img src={user.avatarUrl}></img>;`<br>
```
const element = (<div>
<h1>Hello!</h1> 
<h2>Good to see you here.</h2></div>);
```
#### JSX Prevents Injection Attacks
```
const title = response.potentiallyMaliciousInput;
// This is safe:
const element = <h1>{title}</h1>;
```
#### JSX Represents Objects
```
const element = (
  <h1 className="greeting">
    Hello, world!
  </h1>
);
```
```
const element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);
```
```
const element = {
  type: 'h1',
  props: {
    className: 'greeting',
    children: 'Hello, world!'
  }
};
```
### Rendering Elements
```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```
```
function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);
```
