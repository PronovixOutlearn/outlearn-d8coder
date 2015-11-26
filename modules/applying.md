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

<!-- @section -->

# Custom page with menu item and custom access check

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/access.md", "text" : "I have learned how to create a custom access check service", "title" : "Custom access control to a page", "description" : "Display the user's name and email - but every user should be able to access only his/her own page" -->

<!-- @section -->

# Forms and blocks

## Creating Custom Forms in Drupal 8

<!-- @link, "url" : "http://www.trellon.com/content/blog/how-create-custom-form-in-drupal-8", "text" : "I have created my first Drupal 8 form", "title" : "Creating Custom Forms in Drupal 8", "description" : "A gentle introduction to creating forms in Drupal 8, highlighting the differences and similarities to how you would do this in previous versions of the platform" -->

## A Look Inside Drupal 8's Block Plugin API

<!-- @link, "url" : "https://drupalize.me/blog/201404/look-inside-drupal-8s-block-plugin-api", "text" : "I have learned how easy is creating a custom block", "title" : "A Look Inside Drupal 8's Block Plugin API", "description" : "This blog post takes a look at how a module developer might create custom blocks in Drupal 8" -->

## Building a Drupal 8 Module: Blocks and Forms

What about having a form in a block? There is [example code](https://github.com/upchuk/d8-demo-modules/tree/master/demo) for that.

<!-- @link, "url" : "http://www.sitepoint.com/building-drupal-8-module-blocks-forms/", "text" : "I have understood how to make a block configurable", "title" : "Building a Drupal 8 Module: Blocks and Forms", "description" : "In this tutorial we are going to go a bit further and we will create a custom block that returns some configurable text. After that, we will create a simple form used to print out user submitted values to the screen" -->

## How to Build Multi-step Forms in Drupal 8

<!-- @link, "url" : "http://www.sitepoint.com/how-to-build-multi-step-forms-in-drupal-8/", "text" : "I have seen that creating a base class for a common functionality is a good idea", "title" : "How to Build Multi-step Forms in Drupal 8", "description" : "We are going to look at building a multistep form in Drupal 8. For brevity, the form will have only two steps in the shape of two completely separate forms. To persist values across these steps, we will use functionality provided by Drupal’s core for storing temporary and private data across multiple requests" -->

## Changing forms by `hook_form_alter()`

Form alteration has not changed too much since Drupal 7. You should add a `hook_form_alter()` implementation to your `.module` file, and the only difference in its signature is the same as with the form builder, validate and submit functions: the `$form_state` is no longer an array but a [`\Drupal\Core\Form\FormStateInterface`](https://api.drupal.org/api/drupal/core%21lib%21Drupal%21Core%21Form%21FormStateInterface.php/interface/FormStateInterface/8) object.

<!-- @task, "text" : "Create your own `hook_form_alter()` implementation." -->

<!-- @section -->

# Custom tables and displaying/saving data (basic Schema API)

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/phonebook.md", "text" : "I have seen how cumbersome could be knocking a phonebook together", "title" : "Old-fashioned phonebook", "description" : "List all the entries in a sortable, pagered page; use the same form for adding and editing entries; protect deletion against CSRF without forms" -->

It would be easier if we could use Views, at least for the listing part, wouldn't it? Well, that part is not yet done.

<!-- @section -->

# Long-running tasks

## Batch API

<!-- TODO: Publish this as a blogpost on pronovix.com and reuse the content from there -->
<!-- @link, "url" : "https://github.com/boobaa/d7to8/blob/master/d8/d8batch/README.md", "text" : "I have learned that I don't have to learn the Batch API again", "title" : "D8 Batch API example", "description" : "This module is basically a demonstration of how can you import feed sources from a CSV file to Drupal" -->

## Queue API

Okay, we couldn't find the description of the code Daniel Sipos has published, but the example is great nonetheless. When a node is created as unpublished, it gets added to a queue. That queue can be processed in two ways: by submitting a form, which triggers running the `manual_node_publisher` worker, or by running cron, which triggers the `cron_node_publisher` worker. Both extend the [`NodePublishBase`](https://github.com/upchuk/d8-demo-modules/blob/master/npq/src/Plugin/QueueWorker/NodePublishBase.php) which is not recognized as a queue worker plugin since it does not have the required annotation. In the case of `cron_node_publisher` worker the runtime is limited to 10 seconds by its annonation.

<!-- @link, "url" : "https://github.com/upchuk/d8-demo-modules/tree/master/npq/src", "text" : "I have understood that Queue API workers are annotated plugins", "title" : "Node Publish Queue module", "description" : "Demo module illustrating the Queue API in Drupal 8" -->

<!-- @section -->

# Mail API

<!-- @link, "url" : "http://code.tutsplus.com/tutorials/using-and-extending-the-drupal-8-mail-api-part-1--cms-23419", "text" : "I have learned the basics of mailing", "title" : "Using and Extending the Drupal 8 Mail API, Part 1: Sending and Altering", "description" : "In the first part we will create a custom email template that gets used for sending emails to the current user when s/he saves a new Article node. Additionally, we will see how others can alter that template in order to allow for HTML rendering of the email body instead of the default plain text" -->

<!-- @link, "url" : "http://code.tutsplus.com/tutorials/using-and-extending-the-drupal-8-mail-api-part-2--cms-23484", "text" : "I have seen how to use an external service for sending mail", "title" : "Using and Extending the Drupal 8 Mail API, Part 2: Using an external service", "description" : "Look at how we can use the Mail API to extend the default behaviour. The purpose is to use an external service as a means for email delivery" -->

<!-- @section -->

# Migration

Two years into the development of Drupal 8, Dries Buytaert announced that Drupal 8.0 might ship without an upgrade path – that's how migration comes into the picture.

<!-- @link, "url" : "https://drupalwatchdog.com/volume-4/issue-1/migrate-overview", "text" : "I have understood there are no `hook_update_N()` implementations any longer for major version upgrades", "title" : "Migrate Overview", "description" : "This unorthodox decision was made to support substantial improvements in Drupal’s major version upgrade process by introducing a robust new sub-system based on the popular contributed modules Migrate and Migrate D2D" -->

<!-- @link, "url" : "https://drupalwatchdog.com/volume-4/issue-1/migrate-api", "text" : "I have learned the core of the Migration API", "title" : "Migrate API: Technically speaking", "description" : "The migrate API works with plugins and stores the configuration for those plugins in a configuration entity. There are a number of plugin types offered: source, process, and destination are the most important" -->

<!-- @section -->

# Configuration Management Initiative (CMI)

<!-- @link, "url" : "http://nuvole.org/blog/2014/jun/06/configuration-management-drupal-7-drupal-8", "text" : "I have seen the relation between CMI (in core) and Features (as a contrib module)", "title" : "Configuration Management: Drupal 7 to Drupal 8", "description" : "Nuvole gave two talks about the current status of Configuration Management in Drupal 8 at European Drupal events in 2014. Developers attending the events were mostly interested in how the future Drupal 8 Configuration Management capabilities will compare to Drupal 7, with and without the Features module" -->

<!-- @link, "url" : "https://docs.acquia.com/articles/drupal-8-configuration-forms-and-cmi", "text" : "I have understood the basics of the Config Management", "title" : "Configuration forms and CMI", "description" : "This lesson introduces both a special type of form called a configuration form and the Configuration Management Initiative (CMI), which describes the effort made to gather the multiple sources of configuration information and functions in Drupal 7 into a single system in Drupal 8" -->

<!-- @link, "url" : "https://docs.acquia.com/articles/drupal-8-configuration-and-config-object", "text" : "I have learned about config entities", "title" : "Configuration and the config object", "description" : "Drupal 8 provides a [Config object](https://api.drupal.org/api/drupal/core%21lib%21Drupal%21Core%21Config%21Config.php/class/Config/8) that we can use to interact with the configuration. Some classes already have it available through dependency injection" -->

<!-- @link, "url" : "https://www.drupal.org/developing/api/8/configuration", "text" : "I have bookmarked the Config API documentation page from d.o", "title" : "Configuration API in Drupal 8", "description" : "The configuration API provides a central place for modules to store configuration data. This data can be simple configuration like your site name, or more complex information managed with configuration entities, such as views and content types" -->

<!-- @link, "url" : "http://www.webomelette.com/drupal-8-custom-data-configuration-entities-using-thirdpartysettingsinterface", "text" : "I have seen how to properly hook into the forms of config entities (without hooks, actually)", "title" : "Custom data on configuration entites using the ThirdPartySettingsInterface", "description" : "We are going to look at how to use the ThirdPartySettingsInterface to add some extra data to existing configuration entities. For example, if you ever need to store some config together with a node type or a taxonomy vocabulary, there is a great way to do so using this interface" -->

<!-- @link, "url" : "https://drupalwatchdog.com/volume-5/issue-2/configuration-workflow", "text" : "I have learned the basics of the config workflow", "title" : "Configuration workflow", "description" : "Large website projects involving multiple people in different roles face special challenges. The work needs to be coordinated and scheduled in such a way as to allow for parallel development of different parts of the project on different systems" -->

Configuration workflow (ie. how to export config, move it around with git, import it on the other instance, etc.) will be covered on the upcoming sitebuilder path mode detailed.
