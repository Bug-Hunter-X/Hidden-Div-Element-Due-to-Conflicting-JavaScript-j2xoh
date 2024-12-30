# Hidden Div Element Bug

This repository demonstrates a subtle bug where a div element is hidden by JavaScript, even though it's initially visible in the HTML. This can lead to accessibility problems if JavaScript is disabled or fails to load properly.

## Bug Description

The `bug.html` file contains a div element with some text.  A JavaScript script immediately sets the `display` style of the div to `none`, making it invisible. This is problematic because users with JavaScript disabled will not see the content of the div.

## Solution

The `solution.html` file demonstrates a corrected approach.  The div element is left visible, and its visibility is controlled through a conditional check that evaluates if Javascript is present. This is done by utilizing an onload event and providing a fallback if Javascript is disabled. 

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the div element is hidden, even if JavaScript is enabled.
4. Open `solution.html` to see the fixed version.
