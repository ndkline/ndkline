---
layout: "post"
title: "CETC Alpha Launch"
date: "2016-09-27 12:40"
tags: "Drupal, d7, drupal 7, Plone, RESTful, CETC, Carrara Education Technology Center, CMS, Headless"
---

The Carrara Education Technology Center is proud to announce the Alpha launch of it's website found at [cetc.ed.psu.edu](https://cetc.ed.psu.edu/).

Since my start with the Carrara Education Technology Center, or CETC, I have been tasked with designing and developing a new web presence for the College of Education. If you visit their [current site](ed.psu.edu) and explore a little bit, you will notice it's rather challenging to navigate to information that would be desirable to most types of people that would visit the site, students, faculty, prospective students, etc... It's easy to drill down into content and get lost. Content is also slow to be written, edited, and published. The technical side of our infrastructure is even worse; We run Plone on Windows servers with a caching Varnish (Linux) server. This is a gross simplification of our current stack, however the point I'm making is that the bar of entry on any of our projects is rather steep for most developers.

To solve these issues I decoupled our website's public views and CMS to focus on the content creation process. I nixed Plone and our expensive Windows servers for [Drupal](https://www.drupal.org/) 7 and comparatively Linux servers. Within Drupal I was able to rapidly define content creation workflows for our staff and expose the data via [RESTful services](https://en.wikipedia.org/wiki/Representational_state_transfer). By splitting the CMS and public views apart, I am able to focus development on either backend and front-end. The backend would be Drupal and front-end will be in [AngularJS](https://angularjs.org/), [ReactJS](https://facebook.github.io/react/), or another front-end JavaScript framework.

The CETC website will serve as the Drupal portion of the previously described stack. Any other site we build will consume the content via the RESTful service. As we grow our content, I will be able to build a specialized team around this architecture. The backend team will work within Drupal and front-end team will focus on AngularJS/ReactJS.
