# Topic 3 - Javascript


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
  

*Latest IE, Chrome and Firefox browser should be used. All exercises must be done with ECMAScript 6 syntax.*

**Practice**

1.A

  * Create a function that takes a word and validate if it's a palindrome. If the argument isn't valid display an alert showing:
  "The type: <argument type> isn't valid"

  * Modify the previous function to support any string (word and phrases). For example: "Eva, can I see bees in a cave?"

1.B 

  * Create a function that takes a day and a number _n_ and return the day after the _n_ days (for example getDayAfter('Monday', 4) will return 'Friday'). Show an alert if any argument is invalid with a meaningful message.

  * 

2.A

  * Create a file called `index.html` with the correct doctype and some random content.

  * Add a stylesheet to the HTML file and use it to center the texts of all `section` elements.

  * Add a hidden `section` with `Hello World` inside of it.

  * When the page finished loading the section must fade in.

2.B 

  * Add an interface for the palindrome function: create an `input type=text` that takes the string and a button to validate it. Print the result.

  * Add an interface for the getDayAfter function.

3.  Data fetching

    *   Create a function to get the response from [http://api.icndb.com/jokes/random](http://api.icndb.com/jokes/random).

    *   Replace the button's click event with this new function.

    *   Write the response inside the `section` element.

    *   Create a reusable function to perform AJAX calls. This function must accept a `config` object and return an ES6 Promise.

    *   If a server error occurs `section` content must turn red.

    *   **Hint:** Use the XMLHttpRequest to fetch data from the service.

4.  Data fetching with parameters

    *   Create a function to get the response from [https://api.github.com/search/repositories](https://api.github.com/search/repositories) with parameters `q = 'JavaScript'`.

    *   Showcase a list of repositories, provided by the service, in the right side of the screen.

    *   **Hint:** `ul` must be used to list the repositories.

    *   Add an input with `type="text"` to perform a search for any value.

5.  W3C

    *   Validate your page using W3C validator: [https://addons.mozilla.org/en-US/firefox/addon/web-developer/](https://addons.mozilla.org/en-US/firefox/addon/web-developer/)

6.  DOM manipulation

    *   Write a function that takes as input a matrix of data and outputs a DOM structure representing a table. Attach it to the body of a given page.

    *   **Hint:** use `document.createElement`, `document.createTextNode`, and `Node.appendChild` methods.


[<- To index](../README.md#title) - [Topic 4 - Frameworks ->](./topic4.md)