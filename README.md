# Какие типы данных существуют в JavaScript?
<details>
<summary>Какие типы данных существуют в JavaScript?</summary>
<div>
 В Js 8 типов данных
  <ul>
    <li>
       <b>number</b> typeOf number. Целые и дробные.
    </li>
    <li>
      <b>bigint</b> typeOf bigint. Целые большие числа.
    </li>
    <li>
       <b>boolean</b> typeOf boolean.
    </li>
    <li>
       <b>string</b> typeOf string.
    </li>
    <li>
       <b>null</b> typeOf null. Неизвестное значение.
    </li>
    <li>
       <b>undefined</b> typeOf undefined. Не присвоенное значение.
    </li>
    <li>
       <b>object</b> typeOf object. Сложные структуры данных.
    </li>
    <li>
       <b>symblol</b> typeOf symblol. Для уникальных идентификаторов.
    </li>
  </ul>
</div>
</details>

# Eventloop Call stack Callback Queue WEB API 

<details>
<summary>Eventloop Call stack Callback Queue WEB API </summary>
<div>

<img src="https://raw.githubusercontent.com/YevhenShashnin/cheat_sheet/main/eventloopjs.png">
<p>Вначале выполняется весь синхронный код. В Callback Queue попадают события из WEB API. Из Callback Queue в Call stack попадают события, только если Call stack пустой. Eventloop все время находится в ожидании событий </p>
<p>memory heap ???</p>
<p><b>Call stack</b> first in - last out</p>
<p><b>Callback queue</b> first in - first out</p>
<p><b>WEB API</b> браузерные события</p>
 
</div>
</details>

# Micro macro tasks

<details>
<summary>Micro macro tasks</summary>
<div>
 micro
</div>
</details>

# Cheat sheet for react

<p><b>rfce</b> to define arrow function component</p>

# SOLID principles
<details>
 <summary>principles</summary>
 <ul>
    <li>
        S - the Single responsibility Principle
        <br/>
        class a class should do one thing and therefore it should have only a single reason to change
        antipatern GodObject
    </li>
    <li>
        O - Open - Closed Principle
        <br/>
        open to extansion and closed to modification
        <br/>
        modification mean changing the code of an existing class, and extension means adding new functionality.
    </li>
     <li>
        L - Liskov Substitution Principle
        <br/>
        The Liskov Substitution Principle states that subclasses should be substitutable for their base classes.
    </li>
     <li>
        I - Interface Segregation Principle
        <br/>
        Segregation means keeping things separated, and the Interface Segregation Principle is about separating the interfaces.
    </li>
     <li>
        D - Dependency Inversion Principle
        <br/>
        The Dependency Inversion principle states that our classes should depend upon interfaces or abstract classes instead of concrete classes and functions.
    </li>
 </ul>
</details>
 
# JS (ES 5)
 <details>
  <summary>Details</summary>
     <b>Loops</b>
     <ul>
         <li><b>while</b> statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement. </li>
         <li><b>for</b> statement creates a loop that consists of three optional expressions, enclosed in parentheses and separated by semicolons, followed by a statement (usually a block statement) to be executed in the loop.</li>
     </ul>
     <b>If else condition</b>
     <p>The if...else statement executes a statement if a specified condition is truthy. If the condition is falsy, another statement in the optional else clause will be executed.</p>
     <b>Switch construction</b>
     <p>The switch statement evaluates an expression, matching the expression's value against a series of case clauses, and executes statements after the first case clause with a matching value, until a break statement is encountered. The default clause of a switch statement will be jumped to if no case matches the expression's value.</p>
     <b>conditional (ternary) operator</b>
     <p>The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is truthy followed by a colon (:), and finally the expression to execute if the condition is falsy. This operator is frequently used as an alternative to an if...else statement.</p>
    <b>Interaction: alert, prompt, confirm</b>
     <ul>
         <li><b>alert</b><p>show modal window with text and button OK. User can't interact with the page, until press ok</p></li>
         <li>function <b>prompt</b> accepts two arguments: title and default(optional). Shows Modal with input that have default value.</li>
         <li><b>confirm</b>accepts question. Shows modal with two buttons OK(true) and CANCEL(false).</li>
     </ul>
     <b>strict vs none-strict comparison</b>
     <p>none strict comparison convert and compare operands that are of different types.</p>
     <b>Hoisting</b>
     <p>JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.</p>
     <b>Usage of "var". How does variable behave without "var"?</b>
<p>Variable without var became global variable. Also global variable can be deleted</p>
<b>stricty mode</b>
<p>'use strict' can be defined in two ways: globally and locally. Globally is two define it in first line of code. Locally means inside a function. </p>
<p>Benefits of strict mode:</p>
<ul>
    <li>Prevent accidental creation of global variables</li>
    <li>Prevent duplicating parameter names in a function</li>
    <li>Prevent writing to read-only properties</li>
    <li>variable can not be used before it is declared</li>
</ul>
<b>"eval is evil". Why?</b>
<p>The eval() function evaluates JavaScript code represented as a string and returns its completion value. </p>
<p>In eval’s case, the costs are performance, security, and difficulties in debugging.</p>
<ul>
    <li>Performance. Because it compiles the sting at runtime</li>
    <li>Security risks. Can be execute infinity loops or stolen some data</li>
    <li>Difficulties in debugging</li>
</ul>
<b>Garbage colector</b>
<p>Colects value that to net refered anymore</p>
 </details>
 
# Objects
 <details>
  <summary>Details</summary>
    Five ways to create objects

<ul>
    <li>
        <h5>Object literals</h5>
        <p>let obj = { obj: 'JS is great" }</p>
    </li>
    <li>
        <h5>New Operator  or Constructor</h5>
        <p>function Music(style) { this.style = style }</p>
        <p>let rap = new Music('rap')</p>
    </li>
    <li>
        <h5>Object create</h5>
        <p>let Car = { model: 'BMW' }</p>
        <p>let ElectricCar = Object.create(Car)</p>
    </li>
    <li>
        <h5>Class</h5>
        <p>class Car { constructor(model) { this.model = model } }</p>
        <p>let BMW = new Car('BMW')</p>
    </li>
    <li>
        <h5>Spread operators</h5>
        <p>You can use it when destructuring other object to create new</p>
        <p>You can use it in object literals</p>
    </li>
</ul>

<p>Here i need also say about defineProperty. You can use it in all 5 ways. It helps to define Property Descriptors (writable, enumerable, configurable) </p>
<p>let cat = { name: 'Mur' }</p>
<p>Object.defineProperty(cat, 'name', { writable: false, enumerable: true, configurable: false })</p>
<p>Object.defineProperty(car, "age", { writable: true, enumerable: true, configurable: false, value: 3 })</p>
<p>Changing the value of configurable can be done only once</p>
<p>Another important thing you should keep in mind is that even if the configurable is set to false, the writable can be changed from true to false - but not vice versa</p>
<p>You cannot delete a property for which the configurable is set to false. </p>
<p>If enumerable is false it won't be available in statements as fro..in loop</p>
<p>var cat = { name: 'foo', age: 9 }</p>
<p>console.log(cat.name); // foo </p>
<p>console.log('name' in cat); // true </p>
<p>To check if thew property enumerable you need to use propertyIsEnumerable method</p>
<p>var cat = { name: 'foo', age: 9 }</p>
<p>Object.defineProperty(cat, 'name', { enumerable: false });</p>
<p>console.log(cat.propertyIsEnumerable("name")); // false </p>
<b>Object-to-primitive</b>
            <p>
                The object-to-primitive conversion is called automatically by many built-in functions and operators that
                expect a primitive as a value.
            </p>
            <p>There are 3 types (hints) of it:</p>
            <ul>
                <li>"string" (for alert and other operations that need a string)</li>
                <li>"number" (for maths)</li>
                <li>"default" (few operators, usually objects implement it the same way as "number")</li>
            </ul>
            <p>The specification describes explicitly which operator uses which hint.</p>
            <p>The conversion algorithm is:</p>
            <ol>
                <li>Call obj[Symbol.toPrimitive](hint) if the method exists,</li>
                <li>Otherwise if hint is "string" try calling obj.toString() or obj.valueOf(), whatever exists.</li>
                <li>Otherwise if hint is "number" or "default" </li>
            </ol>
            <p>All these methods must return a primitive to work (if defined).</p>
            <p>
                In practice, it’s often enough to implement only obj.toString() as a “catch-all” method for string
                conversions that should return a “human-readable” representation of an object, for logging or debugging
                purposes.
            </p>
            <b>Ways to clone objects in JS</b>
<ul>
  <li>
    spread operatir shallow copy
    <p>const cloneFood = { ...food };</p>
  </li>
  <li>
    Object.assign shallow copy
    <p>also can do copy of properties to existing object</p>
    <p>const cloneFood = Object.assign({}, food);</p>
  </li>
    Using JSON deep copy (except Date Symbols, Infinity and functions )
    <p>const cloneFood = JSON.parse(JSON.stringify(food));</p>
  <li>
    Using library lodash deep copy
  </li>
  <li>
    structuredClone() deep copy
    <p>const clone = structuredClone(original);</p>
  </li>
</ul>
<b>Getters and Setters in Object</b>
<p>Give to us posibility to define methods in object that set and get value of it</p>
 </details>

