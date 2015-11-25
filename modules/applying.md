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

<!-- @task, "text" : "I have created my own `hook_form_alter()` implementation." -->

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
