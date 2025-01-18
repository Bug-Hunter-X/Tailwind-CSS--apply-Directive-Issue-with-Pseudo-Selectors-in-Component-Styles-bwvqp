# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles containing pseudo-selectors (like `:hover`, `:focus`, etc.) when used within a component's style tag.

## Bug Description

When using `@apply` with a class that includes a pseudo-selector inside a component's `<style>` tag, the expected styles aren't applied in the intended context (e.g., on hover, focus, etc.).

## Reproduction Steps

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that hovering over the button doesn't change its background color as expected.

## Solution

The solution is to move the styling to the component's class attribute instead of using `@apply` with pseudo-selectors inside the `<style>` tag.

See `bugSolution.html` for the corrected code.