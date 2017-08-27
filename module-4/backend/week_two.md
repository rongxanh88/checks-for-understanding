## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?
* Variable assignment and using const and let vs using var. Also, using arrow functions instead of anonymous function declaration which does not bind (this, arguments, or super). Also, classes are now used instead of factory functions. We then declare methods for the class without using the prototype syntax.

2. What's the difference between asynchronous and synchronous JavaScript?
* JS is a single threaded language and can only execute one thing at a time. The asynchronous part is provided by other apis that work with JS and the event loop. This allows for asynchronous JS, so we can write non-blocking code.

3. What are the four pillars of Object Oriented programming?
* Encapsulation, Abstraction, Polymorphism, and Inheritance.
4. What are some tools available in JavaScript to help you write object oriented code?
* Use class syntax and new Object declarations to help write OOP style.

5. What are some key concepts to be aware of when refactoring your JavaScript?
* Using `this` is very important and we can lose the context of `this` when refactoring. 

6. What's a callback function and what are some reasons when we use/need callback functions?
* We use a callback function as a declared method/function to apply to the current function in the call stack. We especially need this for using with event handlers.

7. What's the scope of variables in Javascript?
* Variables declared inside a block have only block scope. Variables declared outside the block are accessible globally. Variables declared without the use of const, let, or var are global variables no matter where they are declared. This is due to variable hoisting.

8. What's the difference between `==` and `===` in JavaScript?
* === also tests for type equality.

9. Why do front end frameworks exist?
* In order to organize and help with writing applications. We wouldn't use raw ruby to write a backend. We use the Rails framework.

#### Review  

10. Why do people say "HTTP is stateless"?
* Servers don't retain the state of your interaction with the page. We usually have to store some session or cookie data to tell the server what state we are in.

11. Describe a RESTful API.
* RESTful APIs follow the 7 HTTP verbs as well as using nouns in the URL to declare what you are accessing. An example is "GET localhost:3000/companies/1/jobs/1" which tells us that we are trying to access one single job that belongs to a particular company.

12. What are some main characteristics of a team following an agile workflow?
* Having a daily standup. Talk about what you did yesterday, what you are going to do today, and if anything is blocking your progress.

13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
* Advantage - we don't have to store a person's credentials and we don't have to fully roll our own authentication.
* Disadvantage - we obtain access to user data that isn't relavent to our app.
