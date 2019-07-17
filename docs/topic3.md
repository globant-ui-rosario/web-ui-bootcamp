# Topic 3 - Javascript - DOM


**Documentation**

* Javascript variables and data structures

  - [Variables](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables)
  - [Numbers and operators](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Math)
  - [Strings in JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings)
  - [Useful string methods](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Useful_string_methods)
  - [Arrays](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays)

* Javascript control structures and functions

  - [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
  - [Looping code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)
  - [Functions](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)
  - [Introduction to events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

* JavaScript objects

  - [Object basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

* Client-side web APIs

  - [Introduction to web APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction)
  - [Manipulating documents](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Manipulating_documents)
  - [Fetching data from the server](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Fetching_data)
  - [Third party APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Third_party_APIs)


*Latest IE, Chrome and Firefox browser should be used. All exercises must be done with ECMAScript 6 syntax.*

**Practice**

1.A

  * Create a function that takes a word and validate if it's a palindrome. If the argument isn't valid display an alert showing:
  "The type: `<argument type>` isn't valid"

  * Modify the previous function to support any string (word and phrases). For example: "Eva, can I see bees in a cave?" (_Optional_)

1.B

  * Create a function that takes a day and a number _n_ and return the day after the _n_ days (for example `getDayAfter('Monday', 4)` will return 'Friday'). Show an alert if any argument is invalid with a meaningful message.

1.C

  * Create a `html` file with the correct doctype, header, meta, etc.

  * Add an interface for the palindrome function: create an `input type=text` that takes the string and a button to validate it. Print the result.

  * Add an interface for the getDayAfter function.

2.A

  * Create a file called `index.html` with the correct doctype, header, meta, etc.

  * Add a stylesheet to the HTML file and use it to center the texts of all `section` elements.

  * Add a hidden `section` with `Hello World` inside of it.

  * When the page finished loading the section must fade in.

  * Add a button below the section of your index page.

  * Create a function that showcases an alert message when called.

  * Attach a click event to the created button which calls the function previously created.

3.A

  * Copy the `index.html` defined in the previous exercise.

  * Create a function to get the response from [http://api.icndb.com/jokes/random](http://api.icndb.com/jokes/random) using XMLHttpRequest.

  * Add a button with a click event with this new function.

  * Write the response inside the `section` element.

  * Create a reusable function to perform AJAX calls using the `fetch` API and re-implement the previous function.

  * If a server error occurs `section` content must turn red.

  * Implement some mechanism to avoid getting the same joke. (_Optional_)

3.B

  * Create a function to get the response from [https://api.github.com/search/repositories](https://api.github.com/search/repositories) with parameters `q = 'JavaScript'`.

  * Showcase a list of repositories, provided by the service, in the right side of the screen.

  *  **Hint:** `ul` must be used to list the repositories.

  * Add an input with `type="text"` to perform a search for any value.

  * Perform the search when the user type a value in the input, use [Debounce](https://css-tricks.com/debouncing-throttling-explained-examples/) to improve the perfomance (_Optional_)

4.A  

  * Write a function that takes as input a matrix of data and outputs a DOM structure representing a table. Attach it to the body of a given page.

  * **Hint:** use `document.createElement`, `document.createTextNode`, and `Node.appendChild` methods.

**Extra documentation**

 - [devdocs.io](http://devdocs.io/)
 - [MDN Javascript Reference](https://developer.mozilla.org/en/JavaScript/Reference)
 - JSONP and CORS: [http://json-p.org/](http://json-p.org/) - [http://www.html5rocks.com/en/tutorials/cors/](http://www.html5rocks.com/en/tutorials/cors/)
 - Using Chrome console to debug JavaScript [https://developer.chrome.com/devtools/docs/console](https://developer.chrome.com/devtools/docs/console)
 - [Eloquent javascript](http://eloquentjavascript.net/)


[<- To index](../README.md#title) - [Topic 4 - Javascript - Design patterns ->](./topic4.md)
