---
layout: post
title: "RESTful APIs"
date: "2017-03-20 14:17:07 -0400"
---

If you’re a front-end developer, chances are you’ve worked with an API, whether it’s RESTful or not is another story that will not be addressed here. What I will discuss is how elegantly RESTful architecture makes backend to front-end relationship an ideal structure for development.

As a front-end developer at Columbia University, I’ve had the pleasure of working with other developers’ APIs. Now, the API might not be considered RESTful that we were working with (a level 1 or 2 on the [Richardson Maturity Model](https://martinfowler.com/articles/richardsonMaturityModel.html)) but the structure is close enough. The project allowed for me to focus solely on the user experience and design of the client side experience without having to worry about server side template rendering, using [AngularJS](https://angularjs.org/) as the front-end framework.

The API I was connecting to was populated with dummy data while he worked on writing the backend logic. As he finished the results changed organically as it was committed and pushed. But how is this better than the typical server-side template processing?

Well, for one the API creates a clear distinction between front-end and backend. When the templates are processed on the server side, developers can step on each other’s toes. In Drupal, for example, the addition of a module can change how some results are written completely, making the front-end dev adjust their code.

Another bonus for RESTful APIs is versioning. If major changes occur to the structure of the API, you can progress to another version number without retiring the old API until you’re ready. While this can be done with most LAMP frameworks, it’s a more convoluted process and again, messy.

Processing the templates on the client side saves you server processing resources. For large scale applications, this can mean hundreds of dollars. It also gives you more flexibility with scaling, letting your resources focus on the computations and leaving the client to render the aesthetics.
