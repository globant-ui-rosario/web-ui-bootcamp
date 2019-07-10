# Topic 4 - Javascript - Design patterns

In this Topic we will focus on learning how JavaScript approaches Object-Oriented programming and
some patterns to group related functionality together.

If you come from Java, or .NET you will find yourself a little bit lost at the beggining.
ECMAScript6 provides a layer of syntactic sugar over the previous version (5.1) that is expected to simplify the language.
But there aren't the classic classes from another Object-Oriented languages

**Documentation**

- [Object-oriented JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object-oriented_JS)
- [Object prototypes](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes)
- [Inheritance](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance)
- [ES6 Modules](https://ponyfoo.com/articles/es6-modules-in-depth)

**Extra documentation**

- Understand how *prototypes* works in ECMAScript 5.1 [http://yehudakatz.com/2011/08/12/understanding-prototypes-in-javascript/](http://yehudakatz.com/2011/08/12/understanding-prototypes-in-javascript/)

- Read the Chapter on JavaScript classes from [*Understanding ECMAScript6*](https://leanpub.com/understandinges6/read#leanpub-auto-classes)


**Practice**

1.  Creating classes

    *   Create a Movie Class with the following structure

        <table>
            <tr>
                <td>Movie</td>
            </tr>
            <tr>
                <td>
                    - title <br />
                    - year <br />
                    - duration
                </td>
            </tr>
            <tr>
                <td>
                    + constructor(name, year, duration) <br />
                    + play() <br />
                    + pause()<br />
                    + resume()
                </td>
            </tr>
        </table>

    *   Instantiate some of your favorite movies and play with them in the console.

    *   Create an Actor class with the following structure

        <table>
            <tr>
                <td>Actor</td>
            </tr>
            <tr>
                <td>
                    - name <br />
                    - age
                </td>
            </tr>
            <tr>
                <td>
                    + constructor(name, age)
                </td>
            </tr>
        </table>

    *   Create a class called EventEmitter with the following structure

        <table>
            <tr>
                <td>EventEmitter</td>
            </tr>
            <tr>
                <td>
                    + constructor()<br />
                    + on(eventName, callback) <br />
                    + emit(eventName)<br />
                    + off(eventName, callback)
                </td>
            </tr>
        </table>

        The `on` method will receive a eventName and a callback or **listener** that will be executed each time a that event is triggered.

        The `emit` method will trigger events to be consumed by other functions or objects.

        The `off` method will delete previously defined event listeners.

2.  Class heritage

    *   Make the Movie class a subclass of EventEmitter and use the inherited methods to publish `play`, `pause` and `resume` events when the related method is called.

3.  Working with classes

    *   Add a method to Movie as `addCast(cast)` that allows the addition of one or more Actors to a move. It must accept if provided more than one Actor at the same time.

        You should be able to do something like

        ```js
        const terminator = new Movie('Terminator I', 1985, 60);
        const arnold = new Actor('Arnold Schwarzenegger', 50);
        const actors = [
            new Actor('Paul Winfield', 50),
            new Actor('Michael Biehn', 50),
            new Actor('Linda Hamilton', 50)
        ];

        terminator.addCast(arnold);
        terminator.addCast(otherCast);
        ```

    *   Create a Logger class with the following structure

        <table>
            <tr>
                <td>Logger</td>
            </tr>
            <tr>
                <td>
                    + constructor()<br />
                    + log(info)
                </td>
            </tr>
        </table>

        After creating this class make an instance of Logger and make it listen to Movie's `play` event.

        As example you must end with something like

        ```js
        const terminator = new Movie('Terminator I', 1985, 60);

        ...

        terminator.play(); // output: The 'play' event has been emitted
        ```

4.  Mixins

    *   Create an object called social, defining the methods `share(friendName)` and `like(friendName)` that generates the following output `{friendName} likes/share {movieName}`.

        Then extend a movie with it to have access to this methods.

        You should end with something like

        ```js
        const ironman = new Movie(...);

        ...

        ironman.share('Mike Blossom');
        ```

        **Hint:** A mixin is not a class which will be instantiated later on. Use a way to extend some object methods into another object. Template literals might be useful to generate the required output.

5.  ES6 Modules

    *   Split all your classes into different files.

    *   Using babel create a single JS bundle.

    **Hint:** check out [this](https://babeljs.io/docs/usage/cli/)

[<- To index](../README.md#title) - [Topic 5 - Frameworks ->](./topic5.md)
