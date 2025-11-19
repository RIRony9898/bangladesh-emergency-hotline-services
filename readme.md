# Bangladesh Emergency Hotline Services

## Description
“The Bangladesh Emergency Hotline Number website is a useful resource that allows users to easily find contact numbers for various government and non-government services.”

## Answers to Questions

#### What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

- `getElementById`: Selects a single element by its unique ID attribute.
- `getElementsByClassName`: Selects all elements with a specific class name.
- `querySelector`: Selects the first element that matches a CSS selector.
- `querySelectorAll`: Selects all elements that match a CSS selector.

#### How do you create and insert a new element into the DOM?

To create and insert a new element:

1. Create the element using `document.createElement('tagName')`.
2. Set attributes or content if needed (e.g., `element.textContent = 'Hello';`).
3. Insert it into the DOM using methods like:
   - `parentElement.appendChild(newElement)` to add as the last child.
   - `parentElement.insertBefore(newElement, referenceElement)` to insert before a specific element.
   - `parentElement.append(newElement)` for modern browsers to append multiple.

#### What is Event Bubbling and how does it work?

Event Bubbling is a phase in the event propagation process where an event starts from the target element and bubbles up through its ancestors in the DOM tree. When an event occurs on an element, it first triggers on that element (target phase), then bubbles up to the parent, grandparent, and so on, until it reaches the document root. This allows parent elements to handle events from child elements.

#### What is Event Delegation in JavaScript? Why is it useful?

Event Delegation is a technique where instead of attaching event listeners to individual elements, you attach a single listener to a parent element. The listener checks the event target to determine which child element triggered the event and handles it accordingly. It's useful because:

- It reduces the number of event listeners, improving performance.
- It works for dynamically added elements without needing to reattach listeners.
- It simplifies code maintenance.

#### What is the difference between preventDefault() and stopPropagation() methods?

- `preventDefault()`: Prevents the default action associated with the event from occurring. For example, it stops a form from submitting or a link from navigating. It doesn't affect event propagation.
- `stopPropagation()`: Stops the event from bubbling up the DOM tree. It prevents parent elements from receiving the event, but the default action still occurs unless `preventDefault()` is also called.
