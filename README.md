# Uncommon HTML/JavaScript Bug: Non-Existent Element ID

This repository demonstrates a common yet easily overlooked bug in web development: attempting to manipulate a DOM element using a non-existent ID.  The bug arises from a mismatch between the JavaScript code attempting to access a particular element (using `document.getElementById()`) and the actual HTML structure, resulting in a `TypeError`.

## Bug Description
The `bug.html` file contains a simple HTML structure with a div element.  The associated JavaScript code incorrectly tries to change the `innerHTML` of a div element using an ID ("nonExistentDiv") that isn't present in the HTML.  This leads to a JavaScript error, preventing the intended content modification.

## Solution
The `bugSolution.html` file provides the corrected code.  It ensures that the JavaScript code correctly targets the existing element (`myDiv`) by using the correct ID.