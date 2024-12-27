# Tailwind CSS @apply Directive Bug

This repository demonstrates a bug related to Tailwind CSS's `@apply` directive and its interaction with pseudo-classes like `:hover`, `:focus`, and `:active`.  The `@apply` directive, when used with these pseudo-classes, only applies the base styles and ignores the pseudo-class-specific styles.

## Bug Reproduction

The `bug.html` file demonstrates the issue.  Notice that the hover effect on the button does not work as expected because the `@apply` directive only applies the base styles.

## Solution

The `solution.html` file shows the correct way to apply styles that include pseudo-classes, without using `@apply` directly to the hover class.  Instead, it applies the base class directly and the hover styles separately.