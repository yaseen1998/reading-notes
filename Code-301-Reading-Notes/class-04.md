## What is a ‘Controlled Component’?
In HTML, form elements such as `<input>`,
`<textarea`>, and `<select>` typically maintain their own state and update it based on user input. 
In React, mutable state is typically kept in the state property of components,
and only updated with setState().

<img src = 'https://miro.medium.com/max/1400/1*3iHnKaQK64ClycpGikpnIA.png'>

## Controlled Input Null Value
Specifying the value prop on a controlled component prevents the user from 
changing the input unless you desire so. If you’ve specified a value but the input is still editable,
you may have accidentally set value to undefined or null.

## Alternatives to Controlled Components
It can sometimes be tedious to use controlled components, 
because you need to write an event handler for every way your data can 
change and pipe all of the input state 
through a React component.

## Fully-Fledged Solutions
If you’re looking for a complete solution including validation, 
keeping track of the visited fields, and handling form submission,
Formik is one of the popular choices.

## Why would we use a ternary operator?

This shorter code yields
`condition ? value if true : value if false`

example :
`(x===y) ? console.log(true) : console.log(false)`
