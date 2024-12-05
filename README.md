# CSS Specificity Gotcha: Nested Selectors and Unexpected Inheritance

This repository demonstrates a subtle issue related to CSS specificity and inheritance. The problem arises when dealing with nested selectors and how inherited styles interact with explicitly applied styles.

## Bug Description

The core problem lies in understanding how CSS specificity works with nested elements.  A common assumption is that a more specific selector (e.g., `.special div`) will *always* override a less specific selector (e.g., `div`). However, this is not always true when inheritance comes into play. The specificity of inherited styles matters and can lead to unexpected outcomes.

## How to Reproduce

1. Clone the repository.
2. Open `bug.css` and `solution.css`.
3. Observe the differences between the expected and actual styling in the `bug.css` file and see the fixed styling in `solution.css`.

## Solution

The solution involves a deeper understanding of CSS specificity and sometimes requires restructuring your CSS to ensure that your desired style overrides are applied correctly.  Consult the solution in the `solution.css` file for a possible fix.

## Lessons Learned

This example highlights the importance of thoroughly testing CSS styles and understanding how specificity and inheritance interact in complex layouts.  Don't rely on assumptions about selector precedence; instead, explicitly test and debug your styles to avoid unexpected visual issues.