# Uncommon HTML Error: Incorrect innerHTML usage

This repository demonstrates an uncommon error in HTML that arises from incorrectly using the `innerHTML` property with an array. When assigning an array to `innerHTML`, the browser does not automatically render the array elements as HTML.  Instead, it renders the array's string representation, which is not valid HTML.

## Bug Description
The bug occurs when attempting to add multiple HTML elements to a container using `innerHTML` and an array. The expected behavior is to have the HTML elements rendered in the container. However, the array is treated as a string, and the browser fails to interpret and render it properly, resulting in unexpected output.

## Solution
The solution involves joining the array elements into a single string before assigning it to `innerHTML`, thus providing the browser with correctly formatted HTML to interpret.