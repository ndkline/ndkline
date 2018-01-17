---
layout: "post"
title: "Internship Aggregate, UX, and AngularJS -- A Story on Blowing Minds"
date: "2016-10-13 10:32"
tags: "ColdFusion, AngularJS, Restful, API, Internship Aggregate, Zurb, Foundation"
---

## Reception of a New Tool

Lately I've been getting awesome feedback on my [Internship Aggregate](https://github.com/ndkline/rhs_intern_db) I launched at the end of summer. The students are telling faculty/staff in that unit how much they like the tool, how easy it is to use, etc. Basically they're confirming the UX has been improved significantly since the original ColdFusion service launched. Best part is, I could scale the new architecture to serve the whole University basically overnight.

Here's the kicker: The unit that requested it wanted it behind a login so no one outside their unit could use it or even see it. PSU bureaucracy at its finest.

Regardless, I'm very pleased with the application's reception amongst its users. Feel free to fork the project on [github](https://github.com/ndkline/rhs_intern_db).

## Technical Overview

I was brought into this project by our lead programmer when the request was made for the update to an internship database. They were wanting an update to the look and feel of the site, essentially a UX overhaul. The old application was built in ColdFusion at around the turn of the century, so needless to say it in fact did need a huge facelift.

We decided to retain the backend "CMS" portion of the application and expose the content via a RESTful API. Once we got that working, I took the front-end and Joe (the other programmer) took updating the backend. We were able to work incredibly well since the my front-end design is only dependent upon the API. It was one of the most fluid front-end/backend collaborations I've experienced.

The RESTful API and CMS were built in, or remained in, ColdFusion while I used AngularJS as a front-end framework and Zurb Foundation for scaffolding.
