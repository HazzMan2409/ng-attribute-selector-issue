# NgCssAttributeSelectorIssue

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.0.5.

## Bug Reproduction

To reproduce the bug, run the following steps:

1. Run `ng serve` to serve the project.
2. Open the app and inspect the button element in the app component.
3. Notice that in its CSS selector there is an _ngcontent attribute on the input element.
4. Run `ng build` to build the project.
5. Open the main[hash].js file in the `dist/` directory.
6. Search for the CSS selector in the app component (you can search for `input[type=search]`).
7. Notice that in the selector there is no _ngcontent attribute on the input element.
