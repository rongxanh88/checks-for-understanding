## Week Four - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's your favorite project management tool?
* I like waffle for its simplicity and the fact that I already understand the context of the stories that I am writing. It would be a different story is someone else wrote the story and I'm on a 5-6 person team, then I think Pivotal Tracker is a much better tool.

2. Why do we create staging environments?
* We can create a staging environment by setting up another branch ('staging') and deploy that as part of a pipeline. The idea is to setup the staging app with production data or something close to it so we can test our changes before pushing it to production where clients and users will see the changes.

3. What are the characteristics of a good README (in your opinion)?
* A good README will have a good descripttion of what repo is for and what problem it solves. The readme will run you through the setup, list any current bugs and how to deal with them, and will describe usage. If this readme describes a gem, it needs to have short code examples to describe its use.

4. What's one main improvement you're going to make to your code regarding accessibility issues?
* I want to fix tab indexing so that someone can navigate the website without using their mouse.

5. What are some basic security concerns to be aware of when building applications?
* Cross-site scripting, SQL injection attacks, any attack that is made through the vulnerability of not using SSL encryption: man-in-then-middle, replay, etc.

6. Why is continuous integration helpful/important?
* Continuous integration helps debug well tested code by making sure that the code written works on other environments, not just yours. This gives us immediate feedback which we can use to debug our code while we still have context of what was written. CI also prevents the huge problems that arise when trying to integrate everyone's feature changes.

7. What are some continuous integration tools?
* Travis CI is a simple config based tool. There are tools like Jenkins which allow a lot more customization.

#### Review  

8. What are some characteristics of "good" git workflow?
* Constant pulling down from the latest staging/master branch so we can have updated code. Then git rebasing our changes onto master and doing local integration and running of tests to make sure that our code works with everything else. This is where CI is important, because we need to know that the code we pull down works so we can debug our own problems, not someone else's.

* After integrating on our machine, we want to push up and create a PR, listing detailed changes, migrations, TODOs. The idea is to make it easy for our code reviewer to look at our code.

9. What are the four fundamental concepts of object oriented programming?
* Encapsulation, Inheritance, Polymorphism, abstraction.

10. What's a module in Ruby and what's the difference between a class and a module?
* A module in Ruby helps to encapsulate code and syntax so that it does not interfere with other parts of our code. It is similar to a class in structure but modules cannot inherit from other modules like a class can inherit from another class. Modules do allow mixins which helps to built composition or add in functionality to our file.
