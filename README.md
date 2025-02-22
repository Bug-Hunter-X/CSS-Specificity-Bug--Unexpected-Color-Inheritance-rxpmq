# CSS Specificity Bug: Unexpected Color Inheritance

This repository demonstrates a subtle CSS specificity bug that can lead to unexpected color inheritance in some browsers. The bug arises from a conflict between two CSS rules where a more general rule ends up overriding a more specific one.

## Bug Description
The bug manifests as incorrect color rendering. A paragraph element (`<p>`) nested inside a div element (`<div>`) should be blue according to the initial CSS rule; however, a more general rule applied to `<p>` element without parent overrides this behavior, resulting in the paragraph turning red instead of blue.

## Bug Solution
The solution involves increasing the specificity of the rule targeting the paragraph element within the `div`. Several ways to do this are presented in the `bugSolution.css` file. All are demonstrated below.

## How to reproduce
1. Clone this repository.
2. Open `index.html` in your browser.
3. Observe the incorrect color of the paragraph element.

## How to fix
1. Open `bugSolution.css`
2. Review and test the different solutions provided in the file.  These solutions address the specificity issue effectively.
