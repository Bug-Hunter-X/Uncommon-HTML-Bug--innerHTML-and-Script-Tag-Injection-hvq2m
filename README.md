# Uncommon HTML Bug: innerHTML and Script Tag Injection

This repository demonstrates an uncommon bug related to using `innerHTML` in HTML to insert a `<script>` tag.  Directly injecting script tags using `innerHTML` is generally unsafe and can lead to unexpected behavior or security vulnerabilities. The bug showcases this issue and provides a solution.

## Bug Description

The `bug.html` file contains a `<div>` element and a JavaScript snippet that attempts to use `innerHTML` to add a `<script>` tag. This approach is problematic because it doesn't properly handle the context of the injected script, potentially leading to unexpected code execution or XSS vulnerabilities.

## Solution

The `bugSolution.html` file demonstrates the correct approach, using standard DOM methods to add a new script element, ensuring proper execution and preventing security risks.  This is significantly safer and more reliable.