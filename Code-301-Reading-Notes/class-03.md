# Lists and Keys


### What is the purpose of a key?
#### Keys
Keys help React identify which items have changed, are added, or are removed. 
Keys should be given to the elements inside the array to give the elements a stable identity

<img src = 'https://res.cloudinary.com/practicaldev/image/fetch/s--WUusgcGF--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/mmbn4lz1jc5fltopgjjv.png'>

#### Extracting Components with Keys

<img src ='https://vegibit.com/wp-content/uploads/2019/04/react-set-attribute-prop.png'>

#### * Keys Must Only Be Unique Among Siblings
Keys used within arrays should be unique among their siblings. However,
they don’t need to be globally unique. 
We can use the same keys when we produce two different arrays

### What does .map() return? 
return the value in array

### If I want to loop through an array and display each value in JSX, how do I do that in React?
you can do that with map or foreach or for loop but don't forget use key

### Each list item needs a unique ____. key

### What is the spread operator?
The spread operator is a useful and quick syntax for adding items to arrays,
combining arrays or objects,
and spreading an array out into a function’s arguments

### What is spread operator used for?
* The spread syntax “spreads” the array into separate arguments. 
example : Math.max(...[1,3,5]) // 5
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

#### example of spread operator:

const fewFruit = ['🍏','🍊','🍌']<br>
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]<br>
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]<br>

#### example of spread operator:
const objectOne = {hello: "🤪"}<br>
const objectTwo = {world: "🐻"}<br>
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }<br>
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}<br>
objectFour.laugh() // 😂😂😂😂😂<br>
