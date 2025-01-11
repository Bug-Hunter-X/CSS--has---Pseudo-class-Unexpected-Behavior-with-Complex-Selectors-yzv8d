# CSS :has() Pseudo-class Unexpected Behavior with Complex Selectors

This repository demonstrates an uncommon CSS bug related to the `:has()` pseudo-class when used with complex selectors involving `:nth-child()` and the general sibling combinator (`~`).  The bug manifests as inconsistent rendering across different browsers.

## Bug Description
The `:has()` pseudo-class, intended to target elements based on their descendants, exhibits unexpected behavior when combined with selectors that require a specific order or relationship between sibling elements.  The provided CSS demonstrates a scenario where this leads to inconsistent rendering.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in different browsers (e.g., Chrome, Firefox, Safari).
3. Observe the variations in styling of the `.container` element.

## Solution
The solution provided in `bugSolution.css` offers a workaround to achieve the intended styling behavior consistently across browsers.  It uses a more straightforward and less ambiguous approach.