1. Difference between getElementById, getElementsByClassName, querySelector / querySelectorAll

So basicaly,

getElementById → it select only one elemnt using id. Id is always uniqe so only one come.
getElementsByClassName → it return many elemnts (HTMLCollection) if same class used.
querySelector → it give first matching elemnt, but we can use css selector.
querySelectorAll → it give all matching elemnts (NodeList).

👉 shorty:
id = one
class = many
querySelector = flexiable but first only

2. How to create and insert a new element into DOM

We can do like this:
let div = document.createElement("div");
div.innerText = "Hello!";
document.body.appendChild(div);
First we create elemnt, then add text, then append it.

👉 flow is:
create → edit → insert

3. What is Event Bubbling?

Event bubbling means event go bottom to up.

Like if button inside div:

button click first
then div
then body

So event is bubbling up like bubble 😅

4. What is Event Delegation? Why useful?

Event delegation means we use one parent event insted of many childs.

Example:
we put event on parent and check which child clicked.

👉 useful because:

less code writting
better performence
work for dynamic elemnts also
5. Difference between preventDefault() and stopPropagation()
preventDefault() → stop default browser behaviour
(like form submit reload page)
stopPropagation() → stop event going to parent

👉 easy:
preventDefault = stop browser
stopPropagation = stop bubbling
