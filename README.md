# CSS Float Issue: Unexpected Behavior with Unset Parent Width

This repository demonstrates a common issue encountered when using the `float` property in CSS without specifying the width of the parent container.  The problem arises because floating elements are removed from the document flow, potentially causing unexpected layout behavior if the parent container's dimensions are not defined. 

The `bug.css` file contains the problematic CSS code, and `bugSolution.css` provides a solution.

## Problem

The initial CSS attempts to make two divs occupy 50% width each using `float:left`. However, without defining the parent container's width, the divs' widths might not be rendered correctly across different browsers.

## Solution

The solution involves explicitly defining the width of the parent container or using a different layout technique that doesn't rely on floats, such as flexbox or grid.