# Uncommon HTML Bug: Incorrect innerHTML usage

This repository demonstrates a subtle bug related to using `innerHTML` in JavaScript with HTML. The primary issue lies in trying to access and manipulate a non-existent element which leads to an error.

## Bug Description
The code attempts to modify the `innerHTML` property of an element ('nonExistentElement') that doesn't exist in the HTML document.  This will throw an error in the browser's developer console, halting script execution and preventing other intended changes from taking effect (e.g., appending text to 'myDiv').

## How to Reproduce
1. Open `bug.html` in a web browser.
2. Inspect the browser's developer console (usually by pressing F12).
3. You'll see an error message related to the `nonExistentElement`.
4. Observe that only the initial text within 'myDiv' is displayed; the second `innerHTML` addition does not occur because of the previous error.