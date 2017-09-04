## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?
* Node is simply server side javascript that runs on Chrome's V8 javascript engine. Node allows us to run JS without the browser!
2. What is Express? Why is Express similar to in the Ruby world?
* Express is similar to Sinatra, in that it is a backend framework which we can build that is lightweight and allows for tons of customization. It is unopinionated, so we have to make our own standards in coding in Express.
3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
```javascript
const express = require('express');
const path    = require('path');
const router  = express.Router();

const foodController = require('../controllers/foodController.js');

router.get('/', foodController.foodList);
```
4. What do we use Knex for?
* Knex is a tool we use to help us connect to our data store. It is not a full ORM, but it does have similarities to Active Record. Generally, it is used for writing SQL in our JS code.
5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?
* We built a routes file which acted as a sort of middleware, which routed requests to the controllers. The controllers then make calls to the models to access the DB.
6. How do you execute raw SQL in node?
* We write something along the lines of `knex.raw('SQL QUERY')` or if we have a database config, like this `database.raw(SQL QUERY)`.
7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
* Advantages include the faster interaction between user and the front end because the backend does less by not having to serve HTML up all the time. Also, having separate applications allow for more modular code bases. We have discreet code bases which are easier to maintain.

#### Review  

8. Describe DNS.
* Domain Naming System - This allows us to find websites by a domain name, rather than an IP address.
9. What does writing clean code mean to you?
* Writing code that is easy to read and understand as well as easy to maintain.
10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?
* Hotels - has many rooms and contains location data, number of rooms.
* Rooms - has a room number. Belongs to a single hotel. Can be reserved.
* Customers - Can reserve a room, and contains all a user's personal data.
