Question 1
What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Answer 1
getElementById("id") finds one specific element using its unique ID.

getElementsByClassName("class") finds all elements that share the same class name. It gives you an HTMLCollection (a live list of elements).

querySelector("selector") finds the first element that matches a CSS selector (like class, id, tag, etc.).

querySelectorAll("selector") finds every element that matches a CSS selector and returns them as a NodeList.

Question 2
How do you create and insert a new element into the DOM?

Answer 2
First, make a new element using document.createElement("tagName").

Then, if you want, put some text or content inside it, like element.textContent = "Hello".

After that, place it into the page using something like parent.appendChild(element) or parent.insertBefore(element, anotherElement).

Question 3
What is Event Bubbling? How does it work?

Answer 3
Event bubbling means an event starts from the element you interact with and then travels upward through its parent elements.

For example, if you click a button inside a div, the click is handled by the button first, then the div, then the body, and keeps moving up.

Question 4
What is Event Delegation in JavaScript? Why is it useful?

Answer 4
Event delegation means attaching an event listener to a parent element instead of adding separate listeners to each child.

When something happens, you check which child triggered it.
This is helpful because it reduces code and also works for new elements added later.

Question 5
What is the difference between preventDefault() and stopPropagation()?

Answer 5
preventDefault() blocks the browser’s normal behavior.
Example: stopping a form from submitting or a link from opening.

stopPropagation() stops the event from moving up to parent elements during bubbling.