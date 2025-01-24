# Uncommon HTML Bug: Content Disappears After Button Click

This repository demonstrates a subtle bug in HTML/JavaScript where clearing the innerHTML of a div element unintentionally leads to missing content.  The bug is easy to make and hard to spot because it doesn't throw errors. The focus is on how easily a developer can accidentally remove content without adding it back and the importance of checking for unintended side effects.

## Bug Description
The `bug.html` file contains a simple HTML page with a div and a button. When the button is clicked, the innerHTML of the div is set to an empty string, effectively clearing its content.  However, no new content is added.  This results in a blank div after clicking the button.

## Solution
The `bugSolution.html` file fixes the bug by adding new content to the div after it's been cleared.  This ensures that the div never truly becomes empty.

## How to Reproduce
1. Open `bug.html` in your web browser.
2. Click the button.
3. Observe that the div becomes empty.
4. Open `bugSolution.html` to see the corrected version.