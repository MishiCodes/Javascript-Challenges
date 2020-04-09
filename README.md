# Javascript-Challenges
Javascript Challenges covering important Javascript topics 
## 1. Variables & basic data types in javascript
### Objectives
Declaring and defining variables.
Learn about basic data types in Javascript (String, Number, Object, Array)
### Instructions
Declare and define the following variables:

* name with the value "John Smith" 
* age with the value 55 
* height with the value 175.5 
* favoriteColors as an array with the following items "Red", "Green" and "Blue" 
* user as an object with the fields: 
    * name with the value "John Smith" 
    * age with the value 55 
    * height with the value 175.5 
    * favoriteColors as an array with the following items "Red", "Green" and "Blue" 
### Tips & Reflections
Learn about javascript modules and how to export and import values. The code for exporting the variables in this lab is already provided. Don't change it but try to understand it.
Try to experiment with var, let and const. What are the differences between them?
### Useful links
freeCodeCamp.org - Full Course video
W3 Schools - Operators tutorial
W3 Schools - Functions tutorial
W3 Schools - Data types tutorial
MDN Guide - Getting started tutorial
Eloquent Javascript - Chapter 1 book
Eloquent Javascript - Chapter 2 book
Eloquent Javascript - Chapter 4 book
## 2. Functions syntax in javascript
Objectives
learn about basic function syntax in javascript
learn about basic javascript operators
Instructions
Create a function sayHey that returns the string "Hey".
Create a function square that takes a number as an argument and return the square of that number.
Examples
sayHey();   // Should return "Hey"
square(2);  // Should return 4
Tips & Reflections
Try to experiment with normal function declaration using the function keyword as well as the newly introduced arrow functions. What are the differences between them?
Useful links
freeCodeCamp.org - Full Course video
W3 Schools - Functions tutorial
MDN - Functions tutorial
Eloquent Javascript - Chapter 3 book

## 3. Making decisions with conditionals
Objectives
Learn about the basic control flow mechanisms in javascript.
Learn about the basic syntax of if/else, switch and the ternary operator.
Instructions
Write a function isHeavy(weight) that takes in a number and returns true if weight is >= 100, false otherwise.
Implement a function dayName(dayOfWeek) that takes a number in the range [0-6] and return the week name corresponding to the number.
Examples
isHeavy(5);     // should return false
isHeavy(100);   // should return true

dayName(0);     // should return "Sunday"
dayName(1);     // should return "Monday"
dayName(6);     // should return "Saturday"
Tips & Reflections
Try both normal if/else as well as the ternary operator. What is the difference?
Is the switch statement really necessary? Is it possible to achieve the same execution order using normal if/else if/else?
Is it possible to implement dayName(dayOfWeek) without using if/else or switch?
Useful links
freeCodeCamp.org - Full Course video
W3Schools - If/Else tutorial
W3Schools - Switch tutorial
MDN - Control flow tutorial
Eloquent javascript - Chapter 2 (Condition execution) book

## 4. Loops and iteration
Objectives
Learn about loops and iteration in javascript.
Learn the basic syntax of for and while.
Instructions
Write a function repeatString(string, n) that repeats the given string n times.
Examples
repeatString("foo", 0);    // Should return ""
repeatString("foo", 1);    // Should return "foo"
repeatString("foo", 2);    // Should return "foofoo"
Tips & Reflections
Try to implement the function with both for and while. What is the difference which one you think is cleaner?
Is there other ways to implement the function?
How can we improve the performance of this function?
Useful links
freeCodeCamp.org - Full Course video
W3Schools - Loop for tutorial
W3Schools - Loop while tutorial
MDN - Loops and iteration tutorial
Eloquent javascript - Chapter 2 (For & While loops) book

## 5. Array iteration
Objectives
Learn about some fundamental operation for arrays in javascript.
Learn to iterate through each item in an array.
Learn about mapping, filtering and searching of indexed collections.
Instructions
Create a function logAll(array) that iterate through each item in the array (from start to end) and log the item using console.log(item).
Create a function squareList(listOfIntegers) that returns a list of squared numbers.
Create a function onlyPositives(listOfIntegers) that filters the given list and return only the positive items in the array.
Create a function firstNegative(listOfIntegers) that returns the first negative number in the list or null if the list has no negative numbers.
Examples
logAll([1]);                    // Should log 1

squareList([1,2]);              // Should return [1, 4]

onlyPositives([-1, 1]);         // Should return [1]

firstNegative([-1, -2, 1, 2]);  // Should return 1

firstNegative([1,2,3]);         // Should return null

Tips & Reflections
It's very important to master these useful array methods forEach, map, filter, find, indexOf and reduce. Read the documentation and try to experiment with them.
Experiment with the different ways to iterate through an array while, for, forEach, for in.
Useful links
W3Schools - array iteration tutorial
MDN - Indexed collections tutorial

## 6. Objects 101
Objectives
learn about objects in javascript.
learn about getting, setting and updating object properties.
Instructions
Implement a function getName(user) that returns the name property of the user object.
Implement a function setName(user, newName) that sets name property of user to newName.
Implement a function addFavoriteColor(user, color) that adds color to the end of the favoriteColors property of user.
Examples
const john = {
    name: 'John',
    favoriteColors: [],
};

getName(john);                  // Should return 'John'
setName(john, "John Smith");    // Should set john.name to "John Smith"
addFavoriteColor(john, "red");  // Should set john.favoriteColors to ["red"]
addFavoriteColor(john, "blue"); // Should set john.favoriteColors to ["red", "blue"]

Tips & Reflections
What is the difference between accessing properties using the dot notation obj.property and the bracket notation obj["property"]? When is it useful to use the bracket notation?
Useful links
W3Schools - Objects tutorial
MDN - Working with objects tutorial
Eloquent javascript - Chapter 4 (Objects) book

## 7. Classes in javascript
Objectives
Learn about the fundamental javascript class concepts.
Learn about constructor and super.
Learn about class properties and methods.
Learn about inheritance in javascript.
Instructions
Create a class Animal with:

name property
a constructor(name) that bootstraps an Animal object with the given name.
a walk() method that uses console.log() to log the following message: <name> is walking. Where <name> is replaced with the actual animal name.
Create a class Dog that inherits Animal class. The class should have:

a constructor(name) that uses super(name) to bootstrap the object using parent constructor.
a speak() method that uses console.log() to log the following message: <name> says woof. where <name> is the dog name.
Create a class Cat that inherits Animal class. The class should have:

a constructor(name) that uses super(name) to bootstrap the object using parent constructor.
a speak() method that uses console.log() to log the following message: <name> says meow. where <name> is the cat name.
Examples
const buddy = new Animal("Buddy");
buddy.walk(); // Should log "Buddy is walking"

const coco = new Dog("Coco");
coco.walk(); // Should log "Coco is walking"
coco.speak();// Should log "Coco says woof"

const tiger = new Cat('Tiger');
tiger.walk(); // Should log "Tiger is walking"
tiger.speak();// Should log "Tiger says meow"
Tips & Reflections
There are many ways to create objects and classes in javascript. Try to explore the different ways and understand the different tradeoffs between them.
Useful links
W3Schools - Classes tutorial
MDN - Classes tutorial
Cheat sheet Cheat sheet

## 8. Iterating through object properties
Objectives
Learn to iterate through object properties.
Instructions
Write a function shallowEqual(obj1, obj2) that iterate through all the properties of obj1 and check that they are equal to corresponding properties of obj2.
Examples

shallowEqual({ a: 1, b: "b"}, { a: 1, b: "b"}); // should return true
shallowEqual({ a: 1, b: "B"}, { a: 1, b: "b"}); // should return false
shallowEqual({ a: 1}, { a: 1, b: "b"});         // should return false
Tips & Reflections
What are the different ways to iterate through all properties in an object? Which one do you prefer and why?
Useful links
W3Schools - Object properties
MDN - Enumerate the properties of an object

## 9. Browser events
Objectives
Learn about event handling in a browser context.
Instructions
Given the following html document:

<html>
    <body>
        <button id="heyBtn">Hey</button>
        <button id="byeBtn">Bye</button>
    </body>
</html>
Your task is to attach the following event handlers using javascript:

Attach an onclick event handler to heyBtn. When the button is clicked this message should be logged "Hey" (use console.log(msg) for logging).
Attach an onclick event handler to byeBtn. When the button is clicked this message should be logged "Bye" (use console.log(msg) for logging).
Tips & Reflections
Use your browser. If you need to debug your solution. It's very helpful to familiarize yourself with chrome developer tools.
Modern browsers has a lot of different events that you can react to. Search for "DOM events" to see more examples.
Learn about css selectors in javascript using document.querySelector(selector) and document.querySelectorAll(selector).
Useful links
W3Schools - addEventListener tutorial
freeCodeCamp.org - OnClick event tutorial
MDN - OnClick event docs
freeCodeCamp.org - addEventListener video

## 10. HTTP
Objectives
Learn about the HTTP request/response cycle.
Implement a restful API client using the popular axios package.
Learn about javascript promises.
Instructions
Implement a class TaskApi with the following static methods

static get(taskId) should make a GET http request to https://jsonplaceholder.typicode.com/todos/<taskId> where <taskId> is replaced with the given taskId parameter.
static create(taskData) should make a POST http request to https://jsonplaceholder.typicode.com/todos with the given taskData in response body.
static update(updatedTask) should make a PUT http request to "https://jsonplaceholder.typicode.com/todos/" + updatedTask.id. updatedTask should be sent in the request body.
static delete(taskId)
All these methods should use axios module and should return the Promise returned by axios. The methods that should be used are:

axios.get(url) for making GET requests.
axios.post(url, data) for making POST requests.
axios.put(url, data) for making PUT requests.
axios.delete(url) for making DELETE requests.
Tips & Reflections
It's highly recommended that you familiarize yourself with API clients that have a graphical user interface since they can be super useful for making and debugging http requests. One popular program that you can test is Postman.
Promises exists in many concurrent programming language. What problems do they try to solve?
Useful links
freeCodeCamp.org - HTTP and everything you need to know about it tutorial
freeCodeCamp.org - Rest API tutorial
axios official github docs
freeCodeCamp.org - Promises tutorial

## 11. Regular expressions & Email validation
Objectives
Learn about some basic regular expression patterns.
Instructions
Write a function isEmail(string) should return true if string is a valid email eg. some_name123@domain.com.

Examples
isEmail("foo@example.com");    // Should return true
isEmail("foo");                // Should return false
Tips & Reflections
Try https://regexr.com/ to test your regex expressions.
Useful links
freeCodeCamp.org - Learn regular expressions video
W3Schools - Regular expressions tutorial
MDN - Regular expressions tutorial

## 12. Variable length function arguments
Objectives
Learn about variable length function arguments in javascript.
Learn about the special arguments object.
Instructions
Create a function concat that can take 0 or more strings as arguments and return a joined string using commas as separator.

Examples
concat();                // should return ""
concat("a");             // should return "a"
concat("a", "b", "c");   // should return "a,b,c"
Tips & Reflections
Can you think of other use-cases where variable length arguments can be useful?
Useful links
W3Schools - Function parameters tutorial
MDN - Arguments object docs
StackOverflow - Variable number of arguments

## 13. Higher order functions (HOF)
Objectives
Learn about fundamental functional programing concepts.
Learn about higher order functions.
Learn about anonymous functions.
Learn about closures.
Instructions
Write a function once(callback) that takes a function as a parameter and returns a new function that can be executed only once.
Implement a function everyOtherTime(callback) that takes a function as a parameter and returns a new function that will be executed every other time it's invoked.
Examples
function hey() {
    console.log("Hey");
}

const heyOnce = once(hey);
heyOnce();      // Should log "Hey"
heyOnce();      // Won't do anything
heyOnce();      // Won't do anything

const heyEveryOtherTime = everyOtherTime(hey);
heyEveryOtherTime();        // Should log "Hey"
heyEveryOtherTime();        // Won't do anything
heyEveryOtherTime();        // Should log "Hey"
heyEveryOtherTime();        // Won't do anything

Tips & Reflections
Can you think of use cases when a function should only be executed once?
Think of other use-cases of higher order functions.
Useful links
freeCodeCamp.org - Into to higher order functions tutorial
Wikipedia - Higher order functions
Eloquent javascript - Chapter 5 book

## 14. Recursive functions
Objectives
Learn about the concept of recursion in computer science.
Use recursion to solve a common math problem.
Instructions
Create a function factorial(n) that return the n'th factorial number by using recursion.

Examples
factorial(0);    // Should return 1
factorial(1);    // Should return 1
factorial(2);    // Should return 2
factorial(4);    // Should return 120
Tips & Reflections
Recursion is a very central concept in computer science and is used in the divide and conquer algorithm design technique. Recursion can replace for and while loops and result in shorter and more readable code. Can you think of places in your code where you can replace for and while with recursion?
Useful links
Computerphile - What on earth is recursion? video
HackerRank - Recursion video
freeCodeCamp.org - Recursion tutorial

## 15. Data structures - Queue
Objectives
Implement a queue in javascript.
Instructions
Implement a Queue class structure with the following methods:
enqueue(item) adds item to the end of the queue.
dequeue() remove the first item in the queue and returns it.
Examples
const q = new Queue();
q.enqueue(1);
q.enqueue(2);

q.dequeue();    // Should return 1
q.dequeue();    // Should return 2
Tips & Reflections
Queue are very common data structures that are used in many scenarios. Can you think of Some?
When implementing the Queue class there are many different ways to store the items. You can for example use a linked list or just a plain javascript array. What are the different tradeoffs between them? Can you think of other ways to store the items?
FIFO and LIFO are common abbreviation in computer science. What do they stand for? In which category does our Queue fall in?
Useful links
Wikipedia - Queue
Geeks for geeks - Queue tutorial
Hacker rank - Stacks and Queues video

## 16. Data structures - Stack
Objectives
Implement a stack data structure from scratch.
Instructions
Create a class Stack with the following methods:
push adds an item to the top of the stack.
pop removes an item from the top of the stack and returns it.
Examples
const s = new Stack();
s.push(1);
s.push(2);
s.push(3);

s.pop();    // Should return 3
s.pop();    // Should return 2
s.pop();    // Should return 1
Tips & Reflections
Can you think of use cases where stacks might be useful?
FIFO and LIFO are common abbreviation in computer science. What do they stand for? In which category does our Stack fall in?
Useful links
Wikipedia - Stack
Geeks for Geeks - Stack tutorial
Hacker rank - Stacks and Queues video

## 17. Palindrome
Objectives
Practice using control flow structures and string functions in javascript.
Instructions
Implement a function isPalindrome(word) that takes a string as a parameter and return true if the string is a palindrome.

Examples
isPalindrome("Madam");      // Should return true
isPalindrome("Hej");        // Should return false
Tips & Reflections
Make sure to have a plan to handle uppercase and lowercase. "Madam" is a palindrome, also "madam".
Useful links
Wikipedia - Palindrome

## 18. Hamming distance
Objectives
Practice working with strings and control flow in javascript.
Instructions
Implement a function hammingDistance(str1, str2) that takes 2 strings and return the hamming distance

Examples
hammingDistance("foo", "foo");              // Should return 0
hammingDistance("ab", "aB");                // Should return 1
hammingDistance("karolin", "kathrin");      // Should return 3
Useful links
Wikipedia - Hamming distance.

## 19. Hamming distance
Objectives
Practice working with strings and control flow in javascript.
Practice working with recursive functions.
Instructions
Implement a function hammingDistance(str1, str2) that takes 2 strings and return the levenshtein distance

Examples
levenshteinDistance("foo", "foo");            // Should return 0
levenshteinDistance("", "abcd");              // Should return 4
levenshteinDistance("cooking", "coding");     // Should return 2
Tips and reflections
Try to think about a recursive solution? What is the base case of recursion?
What is the difference in time complexity between the recursive and iterative version? Which one is easier to implement and read?
Useful links
Wikipedia - Levenshtein distance.

## 20. Sorting algorithms
Objectives
Implement common sorting algorithms.
Understand the time complexity of different sorting algorithms
Instructions
Implement a function sort(arrayOfNumbers) that takes an array of numbers and return a sorted array. Without using the built in sort function.
Examples
sort([5,3,4])    // Should return [3,4,5]
Tips & Reflections
Start with selection sort and insertion sort, since they are relatively easy to implement. What are the differences between them?
Why not implement you're own quick sort?
What is the time complexity of an algorithm? How does the different sorting algorithms that you've implemented differ in terms of time complexity?
Useful links
Visual comparison of sorting algorithms video
Wikipedia - Selection sort
Wikipedia - Insertion sort
Wikipedia - Quick sort

## 21. Primality test
Objectives
Practice using data structures and control flow mechanisms in javascript to solve a common math problem.
Instructions
Implement a function isPrime(number) that takes a positive number as a parameter and returns true if the number is prime, false otherwise.

Examples
isPrime(2); // Should return true
isPrime(4); // Should return false
Tips & Reflections
There many different algorithms that deals with primality testing with different performance characteristics and correctness guarantees. Try to understand these differences before choosing the algorithm that you want to implement.
Useful links
Wikipedia - Prime number
Wikipedia - Primality test

## 22. Graph Search (BFS/DFS)
### Objectives
Learn about some fundamental concepts related to graph theory.
Learn about different ways to represent graph data structures.
Implement BFS (Breadth first search) or DFS (Depth first search) from scratch.
### Instructions
Implement a function graphSearch(edges, start, end) that takes the following parameters:

edges is a list of the graph edges. Edges are stored as an array of arrays. Each element in the array is an edges: [ [from_1, to_1], [from_2, to_2] ].
start is the start node where the search should begin.
end is the end or target node which is the node we are looking for.
The function should return true if there is a path from from to to

### Examples
example graph

const edges = [
    [1, 2],
    [1, 3],
    [2, 4],
    [3, 4],
];
graphSearch(edges, 1, 1); // Should be true graphSearch(edges, 1, 2); // Should be true graphSearch(edges, 1, 4); // Should be true

graphSearch(edges, 2, 1); // Should be false graphSearch(edges, 2, 3); // Should be false graphSearch(edges, 3, 2); // Should be false

### Tips & Reflections
Graphs are extremely common in every day life. Graph databases are used to represent flight traffic, social networks, knowledge graphs and many other things. Can you think of other examples?
What is the difference between directed and undirected graphs?
What are the different tradeoffs between BFS and DFS? When is it useful to use each?
Why is searching for paths in a graph such an important thing? Can you think of some examples?
### Useful links
Wikipedia - Graph data structure
Medium - What the Graph? blog article
Wikipedia - Breadth first search
Wikipedia - Depth first search
HackerRank - Graph search video
freeCodeCamp.org - Graph theory tutorial
