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
 </details>


