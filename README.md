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
