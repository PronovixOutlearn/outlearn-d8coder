<!--
{
"name" : "applying",
"version" : "0.1",
"title" : "Applying the gathered knowledge",
"description" : "Let's start using that knowledge",
"homepage" : "https://www.drupal.org/node/2182165",
"freshnessDate" : 2015-11-25,
"license" : "CC BY 4.0"
}
-->

# Foreword

Let's start using that knowledge you have collected, built and learned. We know Drupal is quite a complex system, and this complexity has even increased with the new release, but bear with us for reading about some details.

<!-- @section -->

# Breadcrumbs That Work

Non-working breadcrumbs will get consumed by birds. Working breadcrumbs are good for spiders, too.

<!-- @link, "url" : "https://www.palantir.net/blog/d8ftw-breadcrumbs-work", "text" : "I have seen how effective the new breadcrumb system is", "title" : "D8FTW: Breadcrumbs That Work", "description" : "Breadcrumbs have long been the bane of every Drupal developer's existence. In simple cases, they work fine out of the box. Once you get even a little complex, though, they get quite unwieldy", "imageUrl" : "https://www.palantir.net/sites/default/files/styles/blogpost-mainimage/public/blog/images/d8-ftw-template.png?itok=Gv5DvJkB" -->

<!-- @task, "text" : "Add a custom breadcrumb to your Hello World! module." -->

<!-- @section -->

# Custom page with menu item and custom access check

Adding a custom access checker for a page needs a bit more work now.

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/access.md", "text" : "I have learned how to create a custom access check service", "title" : "Custom access control to a page", "description" : "Display the user's name and email - but every user should be able to access only his/her own page" -->

<!-- @task, "text" : "Add a custom access check to your Hello World! module." -->

<!-- @section -->

# Forms and blocks

## Creating Custom Forms in Drupal 8

This is the "Hello other side of the World" example.

<!-- @link, "url" : "http://www.trellon.com/content/blog/how-create-custom-form-in-drupal-8", "text" : "I have seen the effectiveness of the Form API", "title" : "Creating Custom Forms in Drupal 8", "description" : "A gentle introduction to creating forms in Drupal 8, highlighting the differences and similarities to how you would do this in previous versions of the platform" -->

<!-- @task, "text" : "Create a custom form." -->

## A Look Inside Drupal 8's Block Plugin API

Any and all pages on a Drupal 8 site are built with blocks. Yes, the main page content is a block, too.

<!-- @link, "url" : "https://drupalize.me/blog/201404/look-inside-drupal-8s-block-plugin-api", "text" : "I have learned how easy is creating a custom block", "title" : "A Look Inside Drupal 8's Block Plugin API", "description" : "This blog post takes a look at how a module developer might create custom blocks in Drupal 8" -->

<!-- @task, "text" : "Create a custom block." -->

## Building a Drupal 8 Module: Blocks and Forms

What about having a form in a block? There is [example code](https://github.com/upchuk/d8-demo-modules/tree/master/demo) for that.

<!-- @link, "url" : "http://www.sitepoint.com/building-drupal-8-module-blocks-forms/", "text" : "I have understood how to make a block configurable", "title" : "Building a Drupal 8 Module: Blocks and Forms", "description" : "In this tutorial we are going to go a bit further and we will create a custom block that returns some configurable text. After that, we will create a simple form used to print out user submitted values to the screen" -->

## How to Build Multi-step Forms in Drupal 8

Single pages, single forms, single-page forms are easy, but what about a multi-step form?

<!-- @link, "url" : "http://www.sitepoint.com/how-to-build-multi-step-forms-in-drupal-8/", "text" : "I have seen that creating a base class for a common functionality is a good idea", "title" : "How to Build Multi-step Forms in Drupal 8", "description" : "We are going to look at building a multistep form in Drupal 8. For brevity, the form will have only two steps in the shape of two completely separate forms. To persist values across these steps, we will use functionality provided by Drupal’s core for storing temporary and private data across multiple requests" -->

## Changing forms by `hook_form_alter()`

Form alteration has not changed too much since Drupal 7. You should add a `hook_form_alter()` implementation to your `.module` file, and the only difference in its signature is the same as with the form builder, validate and submit functions: the `$form_state` is no longer an array but a [`\Drupal\Core\Form\FormStateInterface`](https://api.drupal.org/api/drupal/core%21lib%21Drupal%21Core%21Form%21FormStateInterface.php/interface/FormStateInterface/8) object.

<!-- @task, "text" : "Create your own hook_form_alter() implementation." -->

## Using AJAX forms in Drupal 8

We all know AJAX can make our lives nicer, although a bit more complicated in some cases. And no, it's not about the football club nor the cleaner.

<!-- @link, "url": "http://www.sitepoint.com/using-ajax-forms-drupal-8/", "text" : "I have learned that AJAXifying forms got even more powerful", "title" : "Using AJAX forms in Drupal 8", "description" : "A clean way of using the Drupal 8 Ajax API without writing a single line of JavaScript code", "imageUrl" : "http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2014/07/1404316515drupal8wide-1024x332.png" -->

<!-- @task, "text" : "AJAXify your custom form without writing JavaScript code." -->

<!-- @section -->

# Custom tables and displaying/saving data (basic Schema API)

Want a basic phonebook? Here's one.

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/phonebook.md", "text" : "I have seen how cumbersome could be knocking a phonebook together", "title" : "Old-fashioned phonebook", "description" : "List all the entries in a sortable, pagered page; use the same form for adding and editing entries; protect deletion against CSRF without forms" -->

It would be easier if we could use Views, at least for the listing part, wouldn't it? Well, that part is not written yet.

<!-- @task, "text" : "Submit a pull request that adds Views integration for the old-fashioned phonebook." -->

<!-- @section -->

# Long-running tasks

## Batch API

Hate context switches? Get things done in batches!

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/d8/d8batch/README.md", "text" : "I have learned that I don't have to learn the Batch API again", "title" : "D8 Batch API example", "description" : "This module is basically a demonstration of how can you import feed sources from a CSV file to Drupal" -->

## Queue API

Okay, we couldn't find the description of the code Daniel Sipos has published, but the example is great nonetheless. When a node is created as unpublished, it gets added to a queue. That queue can be processed in two ways: by submitting a form, which triggers running the `manual_node_publisher` worker, or by running cron, which triggers the `cron_node_publisher` worker. Both extend the [`NodePublishBase`](https://github.com/upchuk/d8-demo-modules/blob/master/npq/src/Plugin/QueueWorker/NodePublishBase.php) which is not recognized as a queue worker plugin since it does not have the required annotation. In the case of `cron_node_publisher` worker the runtime is limited to 10 seconds by its annonation.

<!-- @link, "url" : "https://github.com/upchuk/d8-demo-modules/tree/master/npq/src", "text" : "I have understood that Queue API workers are annotated plugins", "title" : "Node Publish Queue module", "description" : "Demo module illustrating the Queue API in Drupal 8" -->

<!-- @task, "text" : "Submit a pull request that creates a form which lets one add phonebook entries from a CSV file using either the Batch or the Queue API." -->

<!-- @section -->

# Mail API

Sending a mail is pretty much the same, although we're using a service now.

<!-- @link, "url" : "http://code.tutsplus.com/tutorials/using-and-extending-the-drupal-8-mail-api-part-1--cms-23419", "text" : "I have learned the basics of mailing", "title" : "Using and Extending the Drupal 8 Mail API, Part 1: Sending and Altering", "description" : "In the first part we will create a custom email template that gets used for sending emails to the current user when s/he saves a new Article node. Additionally, we will see how others can alter that template in order to allow for HTML rendering of the email body instead of the default plain text", "imageUrl" : "https://thumbsplus.tutsplus.com/uploads/users/34/posts/23419/preview_image/drupal.png" -->

We can even replace the Drupal mail manager service with one that uses a 3rd-party service. Confusing, isn't it?

<!-- @link, "url" : "http://code.tutsplus.com/tutorials/using-and-extending-the-drupal-8-mail-api-part-2--cms-23484", "text" : "I have seen how to use an external service for sending mail", "title" : "Using and Extending the Drupal 8 Mail API, Part 2: Using an external service", "description" : "Look at how we can use the Mail API to extend the default behaviour. The purpose is to use an external service as a means for email delivery", "imageUrl" : "https://thumbsplus.tutsplus.com/uploads/users/34/posts/23419/preview_image/drupal.png" -->

<!-- @task, "text" : "Submit a pull request that sends an email when the name of a new phonebook entry is an email, informing the recipient of being added to the site." -->

<!-- @section -->

# Migration

Two years into the development of Drupal 8, Dries Buytaert announced that Drupal 8.0 might ship without an upgrade path – that's how migration comes into the picture.

<!-- @link, "url" : "https://drupalwatchdog.com/volume-4/issue-1/migrate-overview", "text" : "I have understood there are no `hook_update_N()` implementations any longer for major version upgrades", "title" : "Migrate Overview", "description" : "This unorthodox decision was made to support substantial improvements in Drupal’s major version upgrade process by introducing a robust new sub-system based on the popular contributed modules Migrate and Migrate D2D", "imageUrl" : "https://drupalwatchdog.com/sites/default/files/images/web/4.1-migrateoverview.jpg" -->

A good Drupal coder should have a starting point for migration-related documentation, too.

<!-- @link, "url" : "https://drupalwatchdog.com/volume-4/issue-1/migrate-api", "text" : "I have learned the core of the Migration API", "title" : "Migrate API: Technically speaking", "description" : "The migrate API works with plugins and stores the configuration for those plugins in a configuration entity. There are a number of plugin types offered: source, process, and destination are the most important", "imageUrl" : "https://drupalwatchdog.com/sites/default/files/images/web/4.1-migrate-api.jpg" -->

<!-- @section -->

# Configuration Management Initiative (CMI)

Configuration management has some roots in the Drupal 7 era.

<!-- @link, "url" : "http://nuvole.org/blog/2014/jun/06/configuration-management-drupal-7-drupal-8", "text" : "I have seen the relation between CMI (in core) and Features (as a contrib module)", "title" : "Configuration Management: Drupal 7 to Drupal 8", "description" : "Nuvole gave two talks about the current status of Configuration Management in Drupal 8 at European Drupal events in 2014. Developers attending the events were mostly interested in how the future Drupal 8 Configuration Management capabilities will compare to Drupal 7, with and without the Features module", "imageUrl" : "http://nuvole.org/profiles/nuvole/themes/cloudy/images/users/user-andrea.png" -->

Forms may have their initial configuration values in `.settings.yml` files.

<!-- @link, "url" : "https://docs.acquia.com/articles/drupal-8-configuration-forms-and-cmi", "text" : "I have understood the basics of the Config Management", "title" : "Configuration forms and CMI", "description" : "This lesson introduces both a special type of form called a configuration form and the Configuration Management Initiative (CMI), which describes the effort made to gather the multiple sources of configuration information and functions in Drupal 7 into a single system in Drupal 8", "imageUrl" : "https://www.acquia.com/sites/default/files/d8ultimateguide_301x177.jpg" -->

<!-- @task, "text" : "Submit a pull request that sends an email to a configurable address when a new phonebook entry is created." -->

Configuration has its own entities.

<!-- @link, "url" : "https://docs.acquia.com/articles/drupal-8-configuration-and-config-object", "text" : "I have learned about config entities", "title" : "Configuration and the config object", "description" : "Drupal 8 provides a Config object that we can use to interact with the configuration. Some classes already have it available through dependency injection", "imageUrl" : "https://www.acquia.com/sites/default/files/d8ultimateguide_301x177.jpg" -->

Did we mention you should bookmark some resources, like this one?

<!-- @link, "url" : "https://www.drupal.org/developing/api/8/configuration", "text" : "I have bookmarked the Config API documentation page from d.o", "title" : "Configuration API in Drupal 8", "description" : "The configuration API provides a central place for modules to store configuration data. This data can be simple configuration like your site name, or more complex information managed with configuration entities, such as views and content types", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

You can add your own stuff to a configuration entity's form.

<!-- @link, "url" : "http://www.webomelette.com/drupal-8-custom-data-configuration-entities-using-thirdpartysettingsinterface", "text" : "I have seen how to properly hook into the forms of config entities (without hooks, actually)", "title" : "Custom data on configuration entites using the ThirdPartySettingsInterface", "description" : "We are going to look at how to use the ThirdPartySettingsInterface to add some extra data to existing configuration entities. For example, if you ever need to store some config together with a node type or a taxonomy vocabulary, there is a great way to do so using this interface", "imageUrl" : "http://www.webomelette.com/sites/default/files/pictures/picture-1-1439662760.jpg" -->

With the advent of CMI, all Drupal 8 developers should know the basics of the core-supported configuration workflow.

<!-- @link, "url" : "https://drupalwatchdog.com/volume-5/issue-2/configuration-workflow", "text" : "I have learned the basics of the config workflow", "title" : "Configuration workflow", "description" : "Large website projects involving multiple people in different roles face special challenges. The work needs to be coordinated and scheduled in such a way as to allow for parallel development of different parts of the project on different systems", "imageUrl" : "https://drupalwatchdog.com/sites/default/files/images/web/DW5.02-ConfigWorkflowGitStagingConfig.png" -->

Configuration workflow (ie. how to export config, move it around with git, import it on the other instance, etc.) will be covered later.

<!-- @task, "text" : "Bookmark some CMI-related resources yourself for later usage." -->

<!-- @section -->

# Fields: types, widgets, formatters, pseudo fields

## Writing custom fields in Drupal 8

Learning the Field API should start with the easiest things like custom fields and formatters.

<!-- @link, "url": "http://capgemini.github.io/drupal/writing-custom-fields-in-drupal-8/", "text" : "I have written at least one custom formatter", "title" : "Writing custom fields in Drupal 8", "description" : "Fields are the data entry points to a web application. Usually, they provide HTML elements and may be responsible for any manipulation of data before it goes into and comes out of the application", "imageUrl" : "http://capgemini.github.io/images/FieldsDrupalCampLondon2015-005.jpg" -->

<!-- @task, "text" : "Write a field formatter that replaces *text between asterisks* with bold text when a single-line text field is rendered." -->

## Creating pseudo-fields in Drupal 8

The second step in learning the Field API is working with pseudo fields.

<!-- @link, "url": "http://www.webomelette.com/creating-pseudo-fields-drupal-8", "text" : "I have understood how to create a custom pseudo field", "title" : "Creating pseudo-fields in Drupal 8", "description" : "Pseudo-fields are simple display fields that you can control from the display settings of a particular entity type", "imageUrl" : "http://www.webomelette.com/sites/default/files/pictures/picture-1-1439662760.jpg" -->

<!-- @section -->

# Caching

## Cache API

Drupal 8 has a much-improved Cache API, which needs some deeper understanding from the coder, but has great advantages for everybody.

<!-- @link, "url": "https://api.drupal.org/api/drupal/core%21core.api.php/group/cache/8", "text" : "I have learned how elaborated the new Cache API is", "title" : "Cache API", "description" : "The Cache API is used to store data that takes a long time to compute. Caching can either be permanent or valid only for a certain timespan, and the cache can contain any type of data", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

## Cache API in Drupal 8

Such a multitude of new functions should have their dedicated part in the handbook.

<!-- @link, "url": "https://www.drupal.org/developing/api/8/cache", "text" : "I have shed some more light to the details of the new Cache API", "title" : "Cache API in Drupal 8", "description" : "The Cache API is much improved in Drupal 8. The sections on this handbook page go into more detail on each feature", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

## Cacheability of render arrays

Yeah, you read it right: you should stop providing HTML as the return values of your page controller. How do you know the result will be rendered in a browser?

<!-- @link, "url": "https://www.drupal.org/developing/api/8/render/arrays/cacheability", "text" : "I have understood that I should provide caching-related information in the render arrays", "title" : "Cacheability of render arrays", "description" : "Render arrays determine what is shown to the user. Therefore, arrays also determine how cacheable a response is", "imageUrl" : "https://www.drupal.org/files/drupal%208%20logo%20isolated%20CMYK%2072.png" -->

<!-- @task, "text" : "Submit a pull request to the phonebook example that lets the phonebook index page be cached as long as it is possible." -->

<!-- @section -->

# Events and event subscribers

A lot of hooks became obsolete as Drupal 8 has switched to Symfony and its event dispatcher approach.

<!-- @link, "url": "http://www.sitepoint.com/drupal-8-hooks-symfony-event-dispatcher/", "text" : "I have seen how some hooks got replaced by Symfony events", "title" : "Drupal 8 Hooks and the Symfony Event Dispatcher", "description" : "The both loved and hated hook system is getting slowly replaced. Plugins and annotations are taking away much of the need for info hooks and the Symfony Event Dispatcher component is replacing some of the invoked hooks", "imageUrl" : "http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2014/10/1412889376drupal8wide.png" -->

<!-- @task, "text" : "Replace the code that sends a mail to a configurable address when a new phonebook entry is created with a Symfony event so other modules can act on it as well." -->

<!-- @section -->

# Working with entities

## Entity queries and loading entities

The EntityFieldQuery became more sophisticated than ever.

<!-- @link, "url": "https://docs.acquia.com/articles/drupal-8-entity-queries-and-loading-entities", "text" : "I have replaced my EFQ autocompletion with this new entity query in my editor", "title" : "Entity queries and loading entities", "description" : "Querying entities has changed since Drupal 7 because EntityFieldQuery has been replaced by the core service called entity.query which can instantiate a query object for a specified entity type", "imageUrl" : "https://www.acquia.com/sites/default/files/d8ultimateguide_301x177.jpg" -->

<!-- @section -->

# Views in core

## Creating a custom Views field in Drupal 8

That's correct: Views became part of core! You should learn how to code around custom Views fields.

<!-- @link, "url": "http://www.webomelette.com/creating-custom-views-field-drupal-8", "text" : "I have learned how easy it is to create a custom Views field", "title" : "Creating a custom Views field in Drupal 8", "description" : "At the end of this tutorial, you will be able to add a new field to any node based View which will flag (by displaying a specific message) the nodes of a particular type (configurable in the field configuration). Although I will use nodes, you can use this example to create custom fields for other entities as well", "imageUrl" : "http://www.webomelette.com/sites/default/files/pictures/picture-1-1439662760.jpg" -->

## Creating a custom Views filter in Drupal 8

So you should learn how to code around custom Views filters.

<!-- @link, "url": "http://www.webomelette.com/creating-custom-views-filter-drupal-8", "text" : "I have learned how easy it is to create a custom Views filter", "title" : "Creating a custom Views filter in Drupal 8", "description" : "How can we create a custom filter you can then add to the View in the UI and influence the results based on that", "imageUrl" : "http://www.webomelette.com/sites/default/files/pictures/picture-1-1439662760.jpg" -->

<!-- @task, "text" : "Update your pull request for providing Views integration for the old-fashioned phonebook so the index page can be built with Views and it can have filters as well." -->
