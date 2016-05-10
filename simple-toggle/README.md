# Toggle a UI element (alternate between show/hide) with a button

*Dean Attali, July 2015*

Sometimes you want to toggle a section of the UI every time a button is clicked. Since each time a button is clicked, its value is increased by 1, you can use that to toggle an element: place the element inside a `conditionalPanel()`, and in the `condition`, check for the value of the button modulo 2 (to check if the button has been pressed an even or odd number of times). This is the most basic toggling behaviour. If you want anything more advanced, you can use the `toggle()` function from the [shinyjs](https://github.com/daattali/shinyjs) package.