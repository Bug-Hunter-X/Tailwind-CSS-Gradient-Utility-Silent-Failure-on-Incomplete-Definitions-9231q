# Tailwind CSS Gradient Bug

This repository demonstrates a subtle bug in Tailwind CSS's gradient utility classes.  When defining a linear gradient using the `bg-gradient-to-*` utilities, omitting the second (or subsequent) color results in unexpected behavior.  Instead of throwing an error or warning, Tailwind silently defaults to the first color, rendering a solid color instead of a gradient.

## How to Reproduce

1.  Clone this repository.
2.  Open `bug.js` and examine the code.
3.  Note that the `div` element intended to have a gradient background only shows a solid blue color.
4.  Open `bugSolution.js` to see a corrected version that uses a proper gradient definition.

## Solution

Always ensure that you provide at least two colors when defining a gradient with Tailwind. If you intend to have a single color, use the standard background color utilities.