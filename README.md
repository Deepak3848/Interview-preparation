# Interview-preparation
Interview question and answers

#----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Interview Question

HTML - 5

1. Whats is !DOCTYPE.
=> A doctype or document type declaration is an instruction which tells the web browser about the markup language in which the current page is written. 
The Doctype is not an element or tag,it lets the browser know about the version of or standard of HTML or any other markup language that is being used in the document

2. If I remove !DOCTYPE then what will be the output.
=> The <!DOCTYPE> declaration must be the very first thing in your HTML document, before the tag.

The <!DOCTYPE> declaration is not an HTML tag; it is an instruction to the web browser about what version of HTML the page is written in.

A lot of IDEs allow users to leave this out and default to a certain HTML style, but leaving it out does pose a potential threat in browser compatibility and the use of older versions of HTML.

For example: new features & tags in HTML5 such as <article>,< footer >, <header>,<nav>, <section> may not be supported if the <!DOCTYPE> is not declared.


3. Difference between display block, inline-block and inline.
=> Compared to display: inline , the major difference is that display: inline-block allows to set a width and height on the element. 
	Also, with display: inline-block , the top and bottom margins/paddings are respected, but with display: inline they are not.
	
4. HTML 5 new tags. => new features & tags in HTML5 such as <article>,< footer >, <header>,<nav>, <section>

5. What is the semantic and non-semantic element?
=> A semantic element clearly describes its meaning to both the browser and the developer. Examples of non-semantic elements: <div> and <span> - Tells nothing about its content. 
Examples of semantic elements: <form> , <table> , and <article> - Clearly defines its content.

6. What is web storage?
=> localStorage, sessionStorage,

7. What is a difference between local storage and session storage?
8. Web workers in html5.

9. Difference between responsive and adptive sites.
=> Put simply, responsive is fluid and adapts to the size of the screen no matter what the target device. 
   Adaptive design, on the other hand, uses static layouts based on breakpoints which don't respond once they're initially loaded.
   
10. Display inline-block can take width and height. 
=> Compared to display: inline, the major difference is that display: inline-block allows to set a width and height on the element.


CSS - 3

1. What is css and Ways to Insert CSS in web page.

2. CSS Margin Collapse.
=> Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

3. Difference between Pseudo-classes and CSS Pseudo-elements. 
=> A pseudo-element is a 'fake' element, it isn't really in the document with the 'real' ones. Pseudo-classes are like 'fake' classes that are applied to elements under certain conditions, 
much like how you would manipulate the classes of elements using JavaScript.

Pseudo-classes : a:link, visited, a:hover, a:active
               :first-child => pseudo-class matches a specified element that is the first child of another element.
               :lang => pseudo-class allows you to define special rules for different languages.

Pseudo-element :  is used to style specified parts of an element.
               ::first-line pseudo-element is used to add a special style to the first line of a text.
               ::first-letter pseudo-element can only be applied to block-level elements.
               ::before pseudo-element can be used to insert some content before the content of an element.
               ::after pseudo-element can be used to insert some content after the content of an element.
               ::marker pseudo-element selects the markers of list items.
               ::selection pseudo-element matches the portion of an element that is selected by a user.

4. explain box model in detail.

=>The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. 
  Content - The content of the box, where text and images appear
  Padding - Clears an area around the content. The padding is transparent
  Border - A border that goes around the padding and content
  Margin - Clears an area outside the border. The margin is transparent

5. List the position property and explain each property.

6. CSS combinators and explain descendant(space),child(>),adjacent sibling(+) and general sibling(~) selector.

7. Explain flexbox and all the property of flexbox.

8. What is media query.

9. Write the css three div in one row.

10. Explain css grid system.

11. What is Specificity?
=> If there are two or more conflicting CSS rules that point to the same element, the browser follows some rules to determine which one is most specific and therefore wins out.

Think of specificity as a score/rank that determines which style declarations are ultimately applied to an element.

The universal selector (*) has low specificity, while ID selectors are highly specific! 

12. How to write css variable.
13. What is width of below div
div {
  width: 320px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
}
=> 350px

14. What is width of below div

div {
  width: 320px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
  box-sizing: border-box;
}
=> 320px (The CSS box-sizing property allows us to include the padding and border in an element's total width and height.)
 
15. I need 3 div in one row. write css code.
=>
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

.flex-container {
  display: flex;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  margin: 10px;
  padding: 20px;
  font-size: 30px;
}


SCSS

1. What is scss.
2. What is variable in scss.
3. What is Nesting,Partials,Import,Mixins,Inheritance and Operators.


Bootstrap 4


1. What is bootstrap.
2. Difference between container and container-fluid.
=> container has a max width pixel value, whereas . container-fluid is max-width 100%. 
   container-fluid continuously resizes as you change the width of your window/browser by any amount.
   container class provides a responsive fixed width container. 
   container-fluid class provides a full width container, spanning the entire width of the viewport.
   
3. Explain grid system and end points(breakpoints).
3. What is utilities.

4. Explain all Flex class in bootstrap 4.0.
=> <div class="d-flex justify-content-start">...</div>
<div class="d-flex justify-content-end">...</div>
<div class="d-flex justify-content-center">...</div>
<div class="d-flex justify-content-between">...</div>
<div class="d-flex justify-content-around">...</div>

5. Button class in bootstrap and how to write it.
=> <button type="button" class="btn">Basic</button>
<button type="button" class="btn btn-default">Default</button>
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-link">Link</button>


Javascript:

1. JavaScript Data Types.
2. What is Hoisting.

3. What is use of "Use Strict" in javascript.
=> It is not a statement, but a literal expression, ignored by earlier versions of JavaScript. The purpose of "use strict" is to indicate that the code should be
 executed in "strict mode". 
	With strict mode, you can not, for example, use undeclared variables.

4. Explain callback function
=> A callback function is a function passed into another function as an argument, 
	which is then invoked inside the outer function to complete some kind of routine or action.
	
let user = [
   { name: 'Deepak', role: 'Lead Engineer'},
   { name: 'James', role: 'Tech lead' }
  ];
  
  const getUser = () => {
    setTimeout(() => {
      console.log(user);
    }, 1000);
  };
  
  const getUpdatedUsrs= (data, cb) => {
    setTimeout(() => {
       user.push(data);
       cb();
    }, 2000);
  }
  
  
  getUpdatedUsrs({name: 'Ryan', role: 'Test Enginner'}, getUser);

Reverse string using for loop - 
function reverseString(str) {

    // empty string
    let newString = "";
    for (let i = str.length - 1; i >= 0; i--) {
        newString += str[i];
    }
    return newString;
}

// take input from the user
const string = prompt('Enter a string: ');

const result = reverseString(string);
console.log(result);

5. whats is inheritance and can you write the syntax.

6. How to empty an array in JavaScript
const arrayList = ['a', 'b', 'c', 'd', 'e', 'f'];
=> 
arrayList = []
arrayList.length = 0;
arrayList.splice(0, arrayList.length);

 while (arrayList.length > 0) {
            arrayList.pop();
  }
  
  while (arrayList.length > 0) {
            arrayList.shift();
        }
		
console.log(arrayList);

7.
var a = 2 - 5 / 3 * 1 + 2; = 2-5/3+1 = 2-5/4 = 
console.log(a);
=> 2.333333333333333

8. 
const multiply = (a = 2, b = 3, c = 2) => a * b * c;
console.log(multiply(2)); 
=> 12

9. 
console.log(4 > 5 > 3 > 2 > false) 
=> false

10. 
console.log(1 < 2 < 3 < 2)
=> true

11.  (function () {
            console.log(1);
            setTimeout(function () { console.log(2) }, 1000);
            setTimeout(function () { console.log(3) }, 0);
            console.log(4);
        })();
		
=> 1 4 3 2

12. var person1 = { name: 'vishal', age: 20 }
I want kay and value
=>
console.log(Object.keys(person1)); //["name", "age"]
console.log(Object.values(person1)); //["vishal", 20]

13. const arr8 = [[1, 2], [3, 4], [null, [Infinity]], -2, 3, "vishal",[5, 6]]; 
=>
0: (2) [1, 2]
1: (2) [3, 4]
2: (2) [null, Array(1)]
3: -2
4: 3
5: "vishal"
6: (2) [5, 6]
length: 7

=> 
var newArry8 = arr8.flat(Infinity);
console.log(newArry8);

=> 0: 1
1: 2
2: 3
3: 4
4: null
5: Infinity
6: -2
7: 3
8: "vishal"
9: 5
10: 6
length: 11

14. Write the code. Addition of positive number in array.

var myArr1 = [1, 2, 3, 4, null, 'vishal', -2, true];
        var count1 = 0
        myArr1.forEach((element) => {
            if (typeof element === 'number' && element > 0) {
                count1 = count1 + element;
            }
        })
    console.log(count1) 
=> 10


15. Output of given code.
var salary = "1000";
        (function () {
            console.log("Original salary was " + salary);
            var salary = "5000";
            console.log("My New Salary " + salary);
        })();
        console.log("My New Salary " + salary);

=> 
Original salary was undefined
My New Salary 5000
My New Salary 1000
 
16. Output of given code.
var bar = true;
console.log(bar + 0); 
=> 1

17. Output of given code.
var trees = ["xyz", "xxxx", "test", "ryan", "apple"];
delete trees[3];
console.log(trees.length);
=> 5

18. Explain call stack.
19. Promises  in javascript
=>
-----------------------------------------------------------------------------------------------------------------------------
let usersArray = [
  { name: 'Deepak', profession: 'Tech Lead' },
  { name: 'Vaibhav', profession: 'Principal Lead'}
]

const getUsers = () => {
  console.log(1)
  setTimeout(() => {
    console.log('getUsers', usersArray)
  }, 1000);
};

const getLatestUsers = (data) => {
  return new Promise((resolve, reject) => {
   console.log(2)
  setTimeout(() =>  {
    usersArray.push(data);
    let error = false;
    (!error) ? resolve('looks fine') : reject('something not right');
  }, 2000);
  });
}

//getUsers();

getLatestUsers({ name: 'James', profession: 'Sr. Test Lead'})
  .then(getUsers)
  .catch((err) => console.log(err));
-----------------------------------------------------------------------------------------------------------------------------
20. Async/Await 
=> Async/Await is the extension of promises which we get as a support in the language. You can refer Promises in Javascript to know more about it. Async: ...
It makes sure that a promise is returned and if it is not returned then javascript automatically wraps it in a promise which is resolved with its value


-----------------------------------------------------------------------------------------------------------------------------
21. ES5 Features
=> 
"use strict"
String.trim()
Array.isArray()
Array.forEach()
Array.map() 
=> The map() method creates a new array with the results of calling a function for every array element.

The map() method calls the provided function once for each element in an array, in order.

Note: map() does not execute the function for array elements without values.

Note: this method does not change the original array.

Difference between array.map() and array.forEach() => The first difference between map() and forEach() is the returning value. 
The forEach() method returns undefined and map() returns a new array with the transformed elements. Even if they do the same job, the returning value remains different.
const myAwesomeArray = [1, 2, 3, 4, 5]
myAwesomeArray.forEach(x => x * x)
//>>>>>>>>>>>>>return value: undefined

myAwesomeArray.map(x => x * x)
//>>>>>>>>>>>>>return value: [1, 4, 9, 16, 25]

Array.filter()
Array.reduce()
Array.reduceRight()
=> The reduce() method starts at the first element and travels toward the last,
 whereas the reduceRight() method starts at the last element and travels toward the first
Array.every()
Array.some()
Array.indexOf()
Array.lastIndexOf()
JSON.parse()
JSON.stringify()
Date.now()
Property Getters and Setters
New Object Property Methods

22. New Features in ES6
=> 
The let keyword
The const keyword
JavaScript Arrow Functions
JavaScript Class
JavaScript Promise
JavaScript Symbol
Default Parameter Values
Function Rest Parameter
Array.find()
Array.findIndex()
New Number Properties
New Number Methods
New Global Methods

23. JavaScript String padding and what is output of below code
let str = "5";
str = str.padStart(4,0);

=> 00005

24. JavaScript Classes and Constructor 
25. is it JavaScript Asynchronous or synchronous => JavaScript is Synchronous
Spoiler: at its base, JavaScript is a synchronous, blocking, single-threaded language. That just means that only one operation can be in progress at a time
26. Explain asynchronous
27. Difference Between call() and apply()
=>
The call() method takes arguments separately.
The apply() method takes arguments as an array.
Call invokes the function and allows you to pass in arguments one by one. Apply invokes the function and allows you to pass in arguments as an array. Bind returns a new function, allowing you to pass in a this array and any number of arguments.
example - 
let person1 = {
    name: 'Deepak Marathe',
    role: 'Software Enginner'
}

let getPersonDetails = function(hometown, state) {
 return ((`The person 1 name is  ${this.name} and he is ${this.role}. He is from ${hometown} ${state}`));
}

//call
console.log('call - ', getPersonDetails.call(person1,'Pune', 'M.H'));
//apply
console.log('apply - ', getPersonDetails.apply(person1, ['Pune', 'M.H']));

//bind
let fnBind = getPersonDetails.bind(person1, 'Mumbai', 'M.H');

console.log('Bind -', fnBind());

28. Explain JavaScript Object Prototypes
=> The prototype is an object that is associated with every functions and objects by default in JavaScript,
 where function's prototype property is accessible and modifiable and object's prototype property (aka attribute) is not visible. 
Every function includes prototype object by default.
29. Use of this Keyword in javascript
30. Difference between var, let and const.



Angular 7

1. What is Angular? 
=> Angular is an open-source front-end web framework. It is one of the most popular JavaScript frameworks that are mainly maintained by Google. 
It provides a platform for easy development of web-based applications and empowers the front end developers in curating cross-platform applications.  

2. What are the advantages of using Angular? 
=> A few of the major advantages of using Angular framework are listed below: 
 It supports two-way data-binding.  It follows MVC pattern architecture. 
 It supports static template and Angular template. 
 You can add a custom directive. 
 It also supports REST full services. 
 Validations are supported. 
 Support for dependency injection. 
 Has a strong feature like Event Handlers, Animation, etc.

3. Differentiate between Angular and Angular JS. 
=> 
Angular: 
 Uses components and directives. 
 Recommended Language: TypeScript. 
 Provides mobile support. 
 Supports hierarchical Dependency Injection with a unidirectional tree-based change detection. 
 Faster than Angular JS with upgraded feature

4. What are directives in Angular? 
=>
Component directives
Structural directives: 
Attribute Directives: 

5.  What are angular decorators? 
=> There are 4 Types of decorators 
	1) Class decorators, e.g. @Component and @NgModule 
	2) Property decorators for properties inside classes, e.g. @Input and @Output 
	3) Method decorators for methods inside classes, e.g. @HostListener 
	4) Parameter decorators for parameters inside class constructors, e.g. @Inject 
	
6. What are the angular @NgModule metadata? 
=>
@NgModule({ 
    declarations:[Component1, Component2], 
    imports: [Module1, Module2], 
    exports: [MyModule], 
    providers: [Service1, Service2], 
    bootstrap: [AppComponent] 
}) 

7. What are the angular @Component metadata? 
=> 
@Component({ 
changeDetection?: ChangeDetectionStrategy 
viewProviders?: Provider[] 
moduleId?: string 
templateUrl?: string 
template?: string 
styleUrls?: string[] 
styles?: string[] 
animations?: any[] 
encapsulation?: ViewEncapsulation 
interpolation?: [string, string] 
entryComponents?: Array<Type<any> | any[]> 
preserveWhitespaces?: boolean 
 
// inherited from core/Directive 
selector?: string 
inputs?: string[] 
outputs?: string[] 
host?: {...} 
providers?: Provider[] 
exportAs?: string 
queries?: {...} 
})

8. What is data binding? 
=> Data binding is a core concept in Angular and allows to define communication between a component and the DOM, 
making it very easy to define interactive applications without worrying about pushing and pulling data.  

There are four forms of data binding and they differ in the way the data is flowing. 

1) Interpolation: {{ value }} => From the Component to the view 
      <li>Name: {{ user.name }}</li> 
      <li>Email: {{ user.email }}</li> 
2) Property binding: [property]=”value” => From the Component to the view 
      <img [src]="imagePath" class="image-adjustment"/> 
3) Event binding: (event)=”function” => From the view to the Component 
      <button (click)="cookBacon()"></button> 
4) Two-way data binding: [(ngModel)]=”value” = >  Two-way data binding allows to have the data flow both ways     
     <input type="email" [(ngModel)]="user.email"> 
	 
9. What is AOT? 
=> AOT stands for Angular Ahead-of-Time compiler. 
It is used for pre-compiling the application components and along with their templates during the build process. 
Angular applications which are compiled with AOT has a smaller launching time. 
Also, components of these applications can execute immediately, without needing any client-side compilation. 
Templates in these applications are embedded as code within their components. 
It reduces the need for downloading the Angular compiler which saves you from a cumbersome task. 
AOT compiler can discard the unused directives which are further thrown out using a tree-shaking tool.

10. What are pipes? Give me an example.  
=> A pipe takes in data as input and transforms it to a desired output. You can chain pipes together in potentially useful combinations. 
You can write your own custom pipes. Angular comes with a stock of pipes such as DatePipe, UpperCasePipe, LowerCasePipe, CurrencyPipe, and PercentPipe.
 
There are two types of pipes 
1) Build-in =>  
    a. Parameterized 
        {{appValue|Pipe1: parameter1: parameter2 }} 
        {{today | date:'MM-dd-yyyy' }}  
        {{salary | currency:'USD':true}} 
    b. Chaining 
        {{ today | date:'fullDate' | uppercase}} 
 
2)  Custome =>  
    a. Filter 
        {{ name | alphabet}}
		
11. What are the different types of filters in Angular?	
=>
uppercase
lowercase
titlecase
date
json
currency
number
keyvalue

12. What is Dependency Injection in Angular?  
=> Dependency Injection (DI) is a software design pattern where the objects are passed as dependencies rather than hard-coding them within 
the component. The concept of Dependency Injection comes in handy when you are trying to separate the logic of object creation to that of 2
its consumption. The ‘config’ operation makes use of DI that must be configured beforehand while the module gets loaded to retrieve the 
elements of the application. With this feature, a user can change dependencies as per his requirements. 	

13. What is angular lifecycle hooks? 
=>
 ngOnChanges() 
 ngOnInit() 
 ngDoCheck() 
 ngAfterContentInit() 
 ngAfterContentChecked() 
 ngAfterViewInit() 
 ngAfterViewChecked() 
 ngonDestroy()

14. What is Transpiling in Angular? 
=> Transpiling in Angular refers to the process of conversion of the source code from one programming language to another. 
In Angular, generally, this conversion is done from TypeScript to JavaScript. It is an implicit process and happens internally.

15. Application flow of angular? 

16. How to optimize Angular app? 
=> 
 Consider lazy loading instead of fully bundled app if the app size is more. 
 Make sure that any 3rd party library, which is not used, is removed from the application. 
 Have all dependencies and dev-dependencies are clearly separated. 
 Make sure the application doesn’t have un-necessary import statements. 
 Make sure the application is bundled, uglified, and tree shaking is done. 
 Consider AOT compilation.

17. How many types of compilation? 
=> Angular provides two types of compilation: 
1) JIT(Just-in-Time) compilation => In JIT compilation, the application compiles inside the browser during runtime. 
2) AOT(Ahead-of-Time) compilation => Whereas in the AOT compilation, the application compiles during the build time.

JIT - Compile TypeScript just in time for executing it.

Compiled in the browser.
Each file compiled separately.
No need to build after changing your code and before reloading the browser page.
Suitable for local development.
AOT - Compile TypeScript during build phase.

Compiled by the machine itself, via the command line (Faster).
All code compiled together, inlining HTML/CSS in the scripts.
No need to deploy the compiler (Half of Angular size).
More secure, original source not disclosed.
Suitable for production builds.

----------------------------------------------------------------------------

18. How does one share data between components in Angular?
=> 
Parent to child using @Input decorator
Child to parent using @Output and EventEmitter

19. What is the equivalent of ngShow and ngHide in Angular? 
=> Just bind to the hidden property 

20. What is the difference between *ngIf vs [hidden]? 
=> *ngIf effectively removes its content from the DOM while [hidden] modifies the display property and only instructs the 
browser to not show the content but the DOM still contains it. 


21. What is the difference between "@Component" and "@Directive" in Angular?  
=> 
Components have their own view (HTML and styles).  
Directives are just "behavior" added to existing elements and components. 

22. How would you protect a component being activated through the router? 
=> The Angular router ships with a feature called guards. These provide us with ways to control the flow of our application. 
We can stop a user from visitng certain routes, stop a user from leaving routes, and more. The overall process for protecting Angular routes: 
 CanActivate: Check if a user has access 
 CanActivateChild: Check if a user has access to any of the child routes 
 CanDeactivate: Can a user leave a page? For example, they haven't finished editing a post 
 Resolve: Grab data before the route is instantiated 
 CanLoad: Check to see if we can load the routes assets

23. How would you run unit test? 
=> ng test 

24. What is an observable? 
=> Angular uses Observable to treat asynchronous code. The same way that we use callbacks and promises in vanilla JavaScript. In fact, 
the Observable will be added to future versions of JavaScript, but until that happens it is implemented in Angular with the help of 
the RxJS library. Observables are widely used in Angular for handling asynchronous code. For example, to work with Ajax, 
when listening to events and navigating between the pages of an application (routing). To understand why we need to use 
asynchronous code instead of plain JavaScript, think about a code that waits for a response from a remote server. 
There is no way of knowing when the response will return, and whether it will ever come back, so it is not a good idea to stop 
executing the script until the response is received. Asynchronous code is a much better solution, and the way Angular prefers to 
handle asynchronous code is through observables. 

25. Explain the difference between `Promise` and `Observable` in Angular? 
=> 
Promise: Promises work with asynchronous operations. They either return a single value (i.e the promise resolves) or an error message 
(i.e the promise rejects). Another important thing to remember regarding promises is that a request initiated from a promise is not canceled.
 
Disadvantages of Promise: 
 User could not cancel a request to the API. 
 User could not retry a failed call. 
 As our application gets bigger, promises become hard to manage. 

Observable: An Observable is an array or a sequence of events over time. It has at least two participants, the creator 
(the data source) and the subscriber (subscription where data is being consumed). Compared to a promise, an observable can be canceled. 
RxJS is all about unifying the ideas of promise callbacks and data flow and making them easier to work with. 
Observables provide operators, like map, forEach, reduce...similar to an array.
There are also powerful operators like retry(),  reply(), retryWhen(), delay()

26. Explain the difference between "Constructor" and "ngOnInit" 
=> The main difference between constructor and ngOnInit is that ngOnInit is lifecycle hook and runs after constructor. 
Component interpolated template and input initial values aren't available in constructor, but they are available in ngOnInit.

27. How to bundle an Angular app for production? 
=> ng build --prod 

28. Type of loading in angular 
=> There are 3 types of loading. 
1) Eager Loading: In Eager loading, all the feature modules will be loaded before the application starts and all required dependencies will be resolved. 
2) Lazy Loading: Load the module on the user demand. When clicking on any module that time loads the module. 
3) Pre-Loading: A preload strategy creates rules that determine which modules to preload. So, if you have multiple lazy-loaded modules, 
a preloading strategy would determine which modules to preload and when to preload them.

29. What is the purpose of Wildcard route? 
=> A wildcard route has a path consisting of two asterisks. It matches every URL. 
The router will select this route if it can't match a route earlier in the configuration. 
A wildcard route can navigate to a custom "404 Not Found" component or redirect to an existing route 

eg. 
{ 
    path: '**', component: PageNotFoundComponent 
} 

30. What is router outlet? 
=> Router-outlet in Angular works as a placeholder which is used to load the different components dynamically based on the activated component 
or current route state. To enable routing, we need to use router-outlet into our HTML template like this. 
<router-outlet></router-outlet> 

31. What are RxJS subjects? 
=> Subjects are used for multicasting Observables. This means that Subjects will make sure each subscription 
gets the exact same value as the Observable execution is shared among the subscribers. You can do this using the Subject class.

32. variants of RxJS subjects 
=>  
Subject: A special type of Observable which shares a single execution path among observers 
 
Behavior subject: Requires an initial value and emits the current value to new subscribers. 

Replay subject: Replays or emits old values to new subscribers 
 
Async subject: Emits its last value on completion 

33. What is encapsulation? 
=> The View Encapsulation in Angular is a strategy which determines how angular hides (encapsulates) the styles defined in the 
component from bleeding over to the the other parts of the application. 

The following three strategies provided by the Angular to determine how styles are applied. 

 ViewEncapsulation.None 
 ViewEncapsulation.Emulated 
 ViewEncapsulation.ShadowDOM

1. The ViewEncapsulation.None is used, when we do not want any encapsulation. 
When you use this, the styles defined in one component affects the elements of the other components.

2. This strategy isolates the component styles. They do not bleed out to other components. 
The global styles may affect the element styles in the component The Angular adds the attributes to the styles and mark up

34. How to Use Change Detection in Angular?
=>Change Detection means updating the DOM whenever data is changed. Angular provides two strategies for Change Detection. 
In its default strategy, whenever any data is mutated or changed, Angular will run the change detector to update the DOM. 
In the onPush strategy, Angular will only run the change detector  when a new reference is passed to @Input() data. 
To update the DOM with updated data, Angular provides its own change detector to each component, 
which is responsible for detecting change and updating the DOM. 

35. Pure and Impure Pipes in Angular? 
=>
Async Pipe - This is an impure pipe. As async pipe deals with observables, it is marked as impure. This pipe has its own internal state which 
deals with the subscription of the observables under the hood. Angular has to create the instance of this pipe every single time as 
it is used with different observables. We can't use the same instance of this pipe as this will interfere observables with each other. 
This pipe is called on every change detection cycle as observable can produce new value at any point in time. 
So we need to process the value at every digest cycle. 

JsonPipe and SlicePipe - These both pipes are considered impure as the inputs passed to both are mutable. 
If the input is of type mutable, we need to call the pipe at every change detection cycle. An input object can be changed without 
changing the object reference. These both pipes doesn't have any internal state. But still considered as impure.

36. Difference between Reactive forms and Template driven forms in Angular

37. Difference Between setValue() And patchValue() In Angular? 
=>
setValue(): method will set all fromcontrol values from model. If you do not mention any of the formcontrol values in model,then it will throw an 
exception.
patchValue(): 
patchValue() method will also set Formcontrol values from a model but only for those which we have mentioned in the model. So,  
it is not necessary to pass all the model info in patchValue() method.

38. Difference Between valueChanges and statusChanges In Angular
=> valueChanges and statusChanges both return Observable instance and we can subscribe them to get data. 
valueChanges emits an event every time when the value of control changes either using UI or programmatically. 
statusChanges emits an event every time when the validation status of the control is recalculated. 
statusChanges gives current validation status of a control. valueChanges gives current value of a control. 
valueChanges can be used for conditional validation in reactive form. 


39. Explain dynamic component or entyLevel components
=> Component templates are not always fixed. An application may need to load new components at runtime.







Redux

1. What is redux?
=> Redux is a predictable state container for JavaScript apps which makes it possible to use a centralized state management in your application.


Redux can be used with any modern JavaScript-based web frameworks. Before starting to build our Angular Redux sample application let’s first clarify the core concept of Redux.
Redux organizes your application state in the store, a single data structure in your application. The components of your application read the state of the application from the store. The store is never mutated directly. Instead a action is dispatched to a reducer function. The reducer function creates a new application state by combining the old state and the mutations defined by the action.
Let’s explore the building blocks of Redux one by one:


Store:
The store is a single JS object. To create a store you simple need to a add a TypeScript file to the project and declare a new interface type 
which contains all the properties you’d like to keep in the store.

Actions:
Actions are plain JS objects that represent something that has happened. Can be compared to events.

Reducers:
A reducer is a function that specifies how the state changes in response to an action.





Testing

1. How to write test case in angular.
2. Which testing tool use of unit testing in angular.
3. How to run test case.
4. Can you write one test case for below function
function helloWorld() {
  return 'Hello world!';
}
=>

We would write a Jasmine test spec like so:

TypeScript
describe('Hello world', () => { (1)
  it('says hello', () => { (2)
    expect(helloWorld()) (3)
        .toEqual('Hello world!'); (4)
  });
});


The describe(string, function) function defines what we call a Test Suite, a collection of individual Test Specs.
The it(string, function) function defines an individual Test Spec, this contains one or more Test Expectations.
The expect(actual) expression is what we call an Expectation. In conjunction with a Matcher it describes an expected piece of behaviour in the application.
The matcher(expected) expression is what we call a Matcher. It does a boolean comparison with the expected value passed in vs. 
the actual value passed to the expect function, if they are false the spec fails.

5. Jasmine comes with a few pre-built matchers. can you tell me that matchers

=> 
expect(array).toContain(member);
expect(fn).toThrow(string);
expect(fn).toThrowError(string);
expect(instance).toBe(instance);
expect(mixed).toBeDefined();
expect(mixed).toBeFalsy();
expect(mixed).toBeNull();
expect(mixed).toBeTruthy();
expect(mixed).toBeUndefined();
expect(mixed).toEqual(mixed);
expect(mixed).toMatch(pattern);
expect(number).toBeCloseTo(number, decimalPlaces);
expect(number).toBeGreaterThan(number);
expect(number).toBeLessThan(number);
expect(number).toBeNaN();
expect(spy).toHaveBeenCalled();
expect(spy).toHaveBeenCalledTimes(number);
expect(spy).toHaveBeenCalledWith(...arguments);


6. What is beforeAll,afterAll,beforeEach and afterEach
=> 
beforeAll:
This function is called once, before all the specs in a test suite (describe function) are run.
afterAll:
This function is called once after all the specs in a test suite are finished.
beforeEach:
This function is called before each test specification (it function) is run.
afterEach:
This function is called after each test specification is run.

7. What is jest
8. Difference between jest and karma.




LitElement and WebComponent
1. What is lit element
=>
LitElement is a simple base class for creating fast, lightweight web components that work in any web page with any framework. 
LitElement uses lit-html to render into shadow DOM, and adds API to manage properties and attributes

2. What is web components?
=> Web Components is a suite of different technologies allowing you to create reusable custom elements
with their functionality encapsulated away from the rest of your code and utilize them in your web apps.


3. Why web component ?
=> we all know that reusing code as much as possible is a good idea. This has traditionally not been so easy for custom markup structures
think of the complex HTML (and associated style and script) you’ve sometimes had to write to render custom UI controls, 
and how using them multiple times can turn your page into a mess if you are not careful. 

Reusability
Maintainability
Productivity
Composability
Following web standard




Storybook:

1. What is storybook in angular
=> Storybook runs alongside your app in development mode. It helps you build UI components isolated from the business logic and context of your app.


Karza Technologies:

What is view encapsulation ? explain in details with its types (non, emulated, Native. The default value is ViewEncapsulation.Emulated )

What is shadow dom, shadow root 
=> Shadow Root: is the root of the DOM subtree containing the shadow DOM nodes. 
  It is a special node, which creates the boundary between the normal DOM nodes and the Shadow DOM nodes. 
  It is this boundary, which encapsulates the Shadow DOM nodes from any JavaScript or CSS code on the consuming page.
	Shadow DOM: Shadow DOM refers to the ability of the browser to include a subtree of DOM elements into the rendering of a document, 
	but not into the main document DOM tree
	
What are change detection strategy in angular ?
=> Angular provides two strategies for Change Detection. In its default strategy, whenever any data is mutated or changed, 
Angular will run the change detector to update the DOM. In the onPush strategy, Angular will only run the change detector when a new reference is passed to @Input () data.
Whether it is a network request or user event, change detection will be performed by Angular. 
Depending on the increase in the components of the apps and complexity, ChangeDetectorRef in Angular 7 will end up doing more work.
When it comes to specific components, we can set ChangeDetectionRef strategy to OnPush.

What is singleton service in angular ?
=> A singleton service is a service instance that is shared across components. 
Providing a singleton service There are two ways to make a service a singleton in Angular: 
Declare root for the value of the @Injectable () providedIn property

If possible, How to create multiple service instances ?
What is closure and what is the use case of using it ?
What is event loop in javascript ?
What is event bubbling in js ?
=. A button is clicked and the event is directed to the button
If an event handler is set for that object, the event is triggered
If no event handler is set for that object, the event bubbles up (like a bubble in water) to the objects parent

What is diff bet cookie and local storage ?
=> Cookies and local storage serve different purposes. Cookies are mainly for reading server-side, whereas local storage can only be read by the client-side. Apart from saving data, 
a big technical difference is the size of data you can store, and as I mentioned earlier localStorage gives you more to work with.

How the angular application should behave on page reload ? => location.reload();

On page reload, do we need to login again ? => no
what is SPA ?
what is PWA ? progressive web apps 
=. A progressive web application is a type of application software delivered through the web, built using common web technologies including HTML, CSS and JavaScript. 
It is intended to work on any platform that uses a standards-compliant browser, including both desktop and mobile devices

what is web workers ? any example

what is let and const.

can we modify an array created using const ? yes we can modify an array/object created using const.  const a = [1,2,3]; a.pop(); a.push();

what is the diff between ngAfterViewInit and ngAfterContentInit ?
=> ngAfterContentInit : This is called after components external content has been initialized. 
ngAfterViewInit : This is called after the component view and its child views has been initialized.

JWT token ? how to manage to store the token in case of page refresh. => inside HttpOnly cookie



Scenario based questions:
- How to check the users active time on the form ?
- How can we calculate, how much time user has spent on a form actively and idle ?  
=> By creating directive to check the time spent.
- Can we modify the DOM using web workers ?
- If there are 2 components without having any relation between them, how can we share the data if there are only 2 fields to share ?
=> a. using shared service    b. Using parameterised routes
 

Absolute Analytics questions:
- What are authGuards ? how to create custom guards.
- 

flatMap: not preserving the order of items, works asynchronously
switchMap: unsubscribing from previous observable after emitting new one
concatMap: preserving the order of items, works synchronously

What is pollyfill.js and why it is used ?
what is sourceMap ?
what is viewChild ? 
Way of sharing data between components ? If there is no any relation, how can you achieve it using shared service ?
How the second component & Header component knows that data has been changed from the the first component ?
How to call multiple api's at a time using observables ?
How to call multiple api's at a time without using observables ?
What are the ways to call an api in javascript ? (one is Ajax and what is the other)

Hexaware:
ES6
- What is temporal deadzone
- Difference between weakmap and ES6 map
- How to swap variable using object destructuring
- Difference between spread operator and rest operator
- Difference between Fetch method and XMLHTTP calls => 
	 Fetch makes it easier to make asynchronous requests and handle responses better than with the older XMLHttpRequest . 
   ... The main difference between Fetch and XMLHttpRequest is that the Fetch API uses Promises, hence avoiding callback
- Difference between set and weakmap
- What is proxy in ES6
- How const value is garbage collected ?

Angular:
- What is Hashlocation and Pathlocation strategies ?
- Injector tree and injector bubbling
- Custom pipe  (000-123)
- Custom form validation
- ngFor and ngForOf
- forOf and forIn
- forRoot method
- Object destructuring
- jasmine and Karma
- Rest API
- difference between ng-class and ng-style

CSS:
- Tweening in css
- Opecity
- gradient: Gradient Backgrounds. CSS gradients let you display smooth transitions between two or more specified colors. 
	CSS defines two types of gradients: Linear Gradients (goes down/up/left/right/diagonally) Radial Gradients (defined by their center)
- Types of gradients
- CSS Specificity
- Flexbox model
- Margin and padding
- Responsive web design
- Bootstrap class loader
- Types of layout in bootstrap: Fluid and Fixed


Things to be read:
- Lexical scope
- 

Xorient:
- new concepts in angular9
- breaking changes in angular 9 while upgrading
- how to make 
shadowdom => Simply put, the Shadow DOM brings Encapsulation to HTML Elements. Using the Shadow DOM, markup, styles, and behaviors are scoped to 
the element and do not clash with other nodes of the DOM. The Shadow DOM is part of Web Components, which encapsulates styles and login of the element.

authentication, 
absolute and relative position 
where to store token ? which is secure way ? which specific cookie is useful to store the token?
=> The JWT needs to be stored inside an httpOnly cookie, a special kind of cookie that’s only sent in HTTP requests to the server, 
and it’s never accessible (both for reading or writing) from JavaScript running in the browser.


how to achieve multi-threading in js => using web workers
event loop 
cors issue
post and put and patch diff
check objects equality (total number of properties, then key name )



- How to implement the auto running of videos like facebook ? What are the properties to achieve this ?
- How to implement a css like a windows calender ?
- How to implement the virtual scrolling like facebook ? will it call api on every time page scrolls ?
- What is the impact of lazy loading in angular application on SEO ?
- what is server side rendering of application ?
- How interceptors can be implemented ? Can we use multiple interceptors in a single application ? Yes
- How to call multiple api's at a time ? 
- What are the map operators ?
- Use of map, reduce, filters, mergemap, forkjoin, switchMap
- What is zone.js ? What if I removed the zone.js from angular ? Will change detection works in that case ?
=> Yes, Zone and NgZone is used to automatically trigger change detection as a result of async operations. 
	But since change detection is a separate mechanism it can successfully work without Zone and NgZone .
- What are change detection strategies ? which one has advantages ?
- What is the diff between ng-content and ng-template ? Which one has advantages ?
- what is the significance of this keyword in arrow functions ? 
=> In regular functions the this keyword represented the object that called the function, which could be the window, the document, a button or whatever.
	With arrow functions the this keyword always represents the object that defined the arrow function.
- Does array functions works in aot build ? if not, then how it works ? => no, it doesnt work. It converts in to js.
- Things to consider while code review ?
- Angular performance optimization techniques ?
- what configuration has to change to disable change detection globally ?
- How to write a test cases for private or protected functions ?

==================================================================================================

Practical Question - 

1. FizzBuzz problem -
   1. input devisible by 3 ==> Fizz
   2. input devisible by 5 ==> Buzz
   3. input devisible by both 3 & 5 ==> FizzBuzz
   4. input not a number ==> Not a Number
   5. input not devisible by 3 or 5 ==> input only

Solution - 
 function fizzBuzz(input){
 if (typeof input !== 'number')
     return 'Not a number'
     
     if((input % 3 === 0) && (input % 5 === 0))
       return 'FizzBuzz';
       
    if((input % 3 === 0))
       return 'Fizz';  
    
    if((input % 5 === 0))
       return 'Buzz';
       
       return input;
}

let output = fizzBuzz(7);
console.log(output);




======================================================================================================================================
JS questions-

let num = 45; // o/p =>9

let num = 45;
console.log(num.toString().split(''));
let arr = num.toString().split('');
let sum = 0;
arr.forEach(element => {
  element = parseInt(element);
  sum += element;
});
console.log('sum', sum)
--------------------------------------------------------------------

let a = 4; 
let b = 5;  // without using + 9

const getSum = (a,b) => b ? getSum(a ^ b, (a & b) << 1) : a;

let str = 'Deepak Marathe'; => reverse string without using split and join  

let aar1 = [0,1,0,1];
let arr2 = [1,0,1,0]; //merge 3 ways



Angular interview questions -

polyfills.js
 => Polyfills in angular are few lines of code which make your application compatible for different browsers. 
    The code we write is mostly in ES6(New Features: Overview and Comparison) and is not compatible with IE or firefox and needs some environment setups before being able to be viewed or used in these browsers.

vendor.js
=> The vendor.js file is generated during the build process of an Angular application. It contains all the external libraries and dependencies that your application relies on. 
   These can include frameworks like Angular itself, as well as third-party libraries like RxJS, Angular Material, or Bootstrap



dependencies
=> Dependencies are the packages that are required for your application to run properly.



dev-dependencies
=> devDependencies are the packages that are required for development and testing purposes only




directives 


component




All directives are components 






All components are Directives




pre loading




i18n 


web worker



service worker 


SPA 


JWT 


Lay Loading 


Async Pipe 


Observable 


Callback Queue 


Dependency Injection




[12/8 1:08 PM] Vaibhav Jain


@Input 


@Output 


@Viewchild 


@HostBinding 


@HostListner 


Service




{



'firstName' : 'Vaibhav', 


'lastName' : 'Jain' 


}




/user




Observable 


subscribe

=========================================================================================================================================
Array - 
1. revers the each oword from string - 
==> Ans - a) let str = 'I love my india';
  let str = 'string ko reverse kro';

let newString = ''

let result = str.split(' ').map((w) => {
    console.log(w.split('').reverse().join(''))
    return  w.split('').reverse().join('');
})
console.log('result - ', result.join(' '));
---------------------------------------------------------------------------------------------------------
2. How to check given number is an integer or not? 
==> a) Number.isInteger(10) // true

    b) let num = 10.2;

function checkIsInteger(input) {
  console.log(input);
  if (input % 1 === 0) {
    console.log(`${num} is integer`)
  } else {
    console.log(`${num} is not an integer!`)
  }
}

checkIsInteger(num);
------------------------------------------------------------------------------------------------------------
3. Write a function for reverse a number like 12 ==> 21.
==> let num = 12345;

function reverseNumber(input){
  console.log(Number(input.toString().split('').reverse().join('')), );
 
}

reverseNumber(num)
------------------------------------------------------------------------------------------------------------------------------
count char -  
function charCount(str) {
  let value = str.split('');
  let obj = {};
  value.forEach((ele) => {
     
    if (obj.hasOwnProperty(ele) === false) {
        obj[ele] = 1;
    } else {
        obj[ele]++;
    }
  })
  
  return obj;
}

console.log(charCount('apple'));
result = { a: 1, p: 2, l: 1, e: 1 }

------------------------------------------------------------------------------------------------------------------------------

retrive element 

function retriveElement(arr, num = 1){
    for (let i = 0; i < num; i++) {
        console.log('arr', arr[i])
    }
}


retriveElement([1, 2, 3, 4 ,5], 3);
result - arr 1
arr 2
arr 3

---------------------------------------------------------------------------------------------------------------------------------

Find the max element from arr - 3 ways -
//Find max elemenyt from array - 
let arr = [2,4,16,8,10];
let max = 0;

//1. solution  - With Math.max

// let result = Math.max(...arr);
// console.log(`Result with Math.max is - ${result}`);

//2. Solution 2 - for loop -

// for(let i = 0; i <= arr.length; i++ ){
//   if (arr[i] > max) {
//       max = arr[i]
//   }
// }
// console.log('max - ', max);

//3. Solution - With reduce method -

// let result = arr.reduce(function(acc, curr) {
//     if (curr > acc)
//       acc = curr;
//  return acc;
// }, 0);

// console.log('Result', result);


