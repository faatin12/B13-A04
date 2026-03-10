1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
ans:
getElementById selects Specific ID only and returns Single Element object
getElementsByClassName selects Class name(s) only and returns Live HTMLCollection
querySelector  selects Any CSS selector and returns	First matching Element
querySelectorAll selects Any CSS selector and returns Static NodeList

2. How do you create and insert a new element into the DOM?
ans:
Creation: Useing document.createElement('tagName'). we can usually add content via [.textContent] or classes via [.classList.add()].
Insertion: appendChild(): Adds the element as the last child of a parent.
prepend(): Adds it as the first child.
before() / after(): Places it as a sibling to another element.

3. What is Event Bubbling? And how does it work?
ans:
When an event happens on an element, it doesn't just stop there. It behaves like a bubble rising from the bottom of a pool.
How it works: clicking a button inside a <div>, the click event first triggers on the button, then moves up to the div, then to the body, and finally the document.

4. What is Event Delegation in JavaScript? Why is it useful?
ans:
Event Delegation is a pattern that uses Bubbling to its advantage. Instead of adding an event listener to 100 individual list items (<li>), you add one listener to their parent (<ul>).
useful for Memory Efficiency and Dynamic Content.

5. What is the difference between preventDefault() and stopPropagation() methods?
ans:
preventDefault(): Stops the browser's default behavior and stopPropagation(): Stops the event from bubbling further.

