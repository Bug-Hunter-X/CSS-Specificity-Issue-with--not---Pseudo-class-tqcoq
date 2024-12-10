# CSS Specificity Issue with :not() Pseudo-class

This repository demonstrates a subtle bug related to CSS specificity when using the `:not()` pseudo-class.  The issue arises from the way specificity is calculated when `:not()` is combined with other selectors.  The unexpected behavior can lead to unintended styling changes.

## Bug Description
The provided CSS code snippet shows a scenario where the specificity of the selector matching the `.box:not(.red)` class unexpectedly affects other elements that should remain unaffected. This leads to unintended styling changes and can be difficult to debug.

## Solution
The solution involves carefully considering specificity and potentially restructuring the CSS selectors to achieve the desired outcome without unintended consequences. See `bugSolution.css` for a possible fix.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected styling of the blue box.  The blue box should be blue, but due to the bug, it's yellow.