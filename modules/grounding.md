<!--
{
"name" : "grounding",
"version" : "0.1",
"title" : "Grounding",
"description" : "Without proper foundation, every house will collapse",
"freshnessDate" : 2015-11-24,
"license" : "CC BY 4.0"
}
-->

# Foreword

Without proper foundation, every house will collapse. If you don't know some basics about Drupal 8, you may be able to knock together even a skyscraper of a really popular module, but there is a chance it will collapse under the pressure of bugs, or simply misinterpretations.

<!-- @section -->

# Digging up the treasure

Before getting deeper, you should read these articles and/or comments.

## A generic introduction to object oriented programming in PHP

Any Drupal 8 coder should have some basic OOP knowledge.

<!-- @link, "url" : "https://drupalwatchdog.com/volume-3/issue-1/object-oriented-programming-101", "text" : "I have removed the dust from my OOP knowledge", "title" : "Object Oriented Programming 101", "description" : "This Drupal Watchdog article is a great introduction to OOP in PHP" -->

## Design Patterns

You will find your place in any community easier if you know what patterns to follow.

<!-- @link, "url" : "http://www.phptherightway.com/pages/Design-Patterns.html", "text" : "I have read about the Factory, Singleton, Strategy, Front Controller and MVC patterns", "description" : "There are numerous ways to structure the code and project for your web application, and you can put as much or as little thought as you like into architecting. But it is usually a good idea to follow common patterns" -->

## Drupal 8 Modules: A New World in Module Writing

As we are "getting off the island" of Drupal-only development, we should be aware that most of our tools "were not invented here".

<!-- @link, "url" : "https://drupalwatchdog.com/volume-3/issue-2/drupal-8-modules", "text" : "I have learned that a lot of things changed, but this will make my life easier", "title" : "Drupal 8 Modules: A New World in Module Writing", "description" : "This article will be more about the patterns you need to use during Drupal 8 development than how to fit the various pieces together" -->

## Getting Started - Background & Prerequisites (Drupal 8)

You should know about some background information as well.

<!-- @link, "url" : "https://www.drupal.org/node/2182165", "text" : "I have understood that this documentation page is a useful starting point that I can make use of later", "title" : "Getting Started - Background & Prerequisites (Drupal 8)", "description" : "Drupal 8 leverages a number of advanced PHP language features and sophisticated 3rd party libraries in order to present 3rd party developers with the most advanced API of any CMS available", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

## How I learned Drupal 8

It is always a good idea to learn from others watching how they use their tools.

<!-- @link, "url" : "https://dev.acquia.com/blog/how-i-learned-drupal-8", "text" : "I have learned about some useful resources and tools", "title" : "How I learned Drupal 8", "description" : "In this post, Alejandro Garza will share his experience on trying to learn Drupal 8 during its alpha stage, talk about some of the challenges of keeping up with the ongoing changes while trying to learn it, and end with some tips and resources which proved useful for him" -->

<!-- @task, "text" : "Update your working environment and make sure it really helps you in coding with autocompletion, class exploration, PSR-4 compliant code navigation, etc." -->

<!-- @section -->

# Getting more intimate with Drupal 8

Now that you know some basics, let's start building your Drupal 8 house. Or career.

## The structure of Drupal 8

Drupal 8 has its roots in Drupal and Symfony as well.

<!-- @link, "url" : "https://cipix.nl/understanding-drupal-8-part-1-general-structure-framework", "text": "I have understood the relation between Symfony 2 and Drupal 8", "title" : "The structure of Drupal 8", "description" : "We'll have a look at the general structure of the Drupal 8 framework, especially in relation to the Symfony2 components" -->

## The Service Container

The service container helps us with quite some housekeeping work.

<!-- @link, "url" : "https://cipix.nl/understanding-drupal-8-part-2-service-container", "text": "I have understood why is it good to rely on a container", "title" : "The Service Container", "description" : "Learn about the service container and how it is used in Drupal 8: it is very important to know about it before learning about routing" -->

## Routing

We think this is one of the most useful resources about Drupal 8 out there.

<!-- @link, "url" : "https://cipix.nl/understanding-drupal-8-part-3-routing", "text": "I have interiorized some gory details of Drupal 8's heart: the routing system", "title" : "Routing", "description" : "Now it is a good idea to get an understanding on how a request is handled by Drupal 8" -->

## Dependency injection in Drupal 8

As there are a multitude of tools in our house, there should be an automated way to keep up with the relationships between them.

<!-- @link, "url" : "http://blog.openlucius.com/en/blog/dependency-injection-drupal-8-introduction", "text": "I have learned about the different types of dependency injection", "title" : "Dependency injection in Drupal 8, an introduction.", "description" : "For all new developers we should explain exactly what dependency injection is" -->

## A Peek at Traits in Drupal 8

Although traits are not widely used in Drupal 8, you should know what to avoid about them.

<!-- @link, "url" : "https://drupalize.me/blog/201503/dependency-injection-traits-drupal-8", "text" : "I will not use Traits for dependency injection", "title" : "A Peek at Traits in Drupal 8", "description" : "Have you ever gone to the grocery store and bought something that you already had in your pantry? Sometimes I forget to peek into the dark corners of my cupboard before heading out to the store" -->

## Dependency Injection Example

Theory should be followed by practice.

<!-- @link, "url" : "https://www.drupal.org/node/2116767#comment-10503230", "text" : "I have understood the simplest example of dependency injection", "title" : "Dependency Injection Example", "description" : "Let's assume we need to format current date according to Drupal regional and language settings. We can achieve this by injecting `date.formatter` core service to perform date formating", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

## Services and dependency injection in Drupal 8

Services are dependable, so you should depend on them instead of direct usage, when it is possible.

<!-- @link, "url" : "https://www.drupal.org/node/2133171", "text" : "I have learned that using services directly may be worse than dependency injection", "title" : "Services and dependency injection in Drupal 8", "description" : "Drupal 8 introduces the concept of services to decouple reusable functionality and makes these services pluggable and replaceable by registering them with a service container" -->

## Plugins

The first article should onboard you for working with plugins.

<!-- @link, "url" : "https://drupalize.me/blog/201407/drupal-8-plugins-explained", "text" : "I have seen what are those awesome plugins", "title" : "Drupal 8 Plugins Explained", "description" : "As you start down the road of learning Drupal 8 module development, one of the first new Drupalisms that you're likely to encounter are plugins" -->

The second article describes how plugins work in more detail.

<!-- @link, "url" : "https://drupalize.me/blog/201409/unravelling-drupal-8-plugin-system", "text" : "I have understood that the plugin system is awesome in general", "title" : "Unravelling the Drupal 8 Plugin System", "description" : "Plugins play an important role in Drupal 8, and understanding how the entire plugin system works will help us better understand how, when, where, and why we use plugins" -->

## Annotations-based plugins

See how the system becomes aware of those deeply-buried plugin classes.

<!-- @link, "url" : "https://www.drupal.org/node/1882526", "text" : "I have learned how my code is driven by my comments", "title" : "Annotations-based plugins", "description" : "Most of the plugins in Drupal 8 will use annotations to register themselves and describe their metadata" -->

<!-- @task, "text" : "Navigate around the source code of core to be familiar with the structure and all those new things like service container, routing, dependency injection, plugins and annotations." -->

<!-- @section -->

# Bored of typing that much code all the day?

Type tirelessly around the clock, you should not, Yoda said, as there's a new hope: a tool that helps in scaffolding.

<!-- @link, "url" : "http://drupalconsole.com/", "text" : "I have read about this new scaffolding tool", "title" : "Drupal Console", "description" : "The Drupal Console is a suite of tools that you run on a command line interface (CLI) to generate boilerplate code and interact with a Drupal 8 installation" -->

<!-- @task, "text" : "Add Drupal Console to your toolchain." -->
