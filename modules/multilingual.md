<!--
{
"name" : "multilingual",
"version" : "0.1",
"title" : "Multilingual Drupal 8",
"description" : "There is an amazing set of new features and improvements in Drupal 8 core, and I'm going through them one by one so you get to know what is coming and also I can highlight the issues that you can still help with to make these better. I believe Drupal 8 will be a huge release for multilingual, but it can always be even better of course.",
"freshnessDate" : 2015-12-01
}
-->

# Foreword

The best teacher of multilingual stuff is the leader of the Drupal 8 Multilingual Initiative (D8MI in short), Gábor Hojtsy. As he said:

> There is an amazing set of new features and improvements in Drupal 8 core, and I'm going through them one by one so you get to know what is coming and also I can highlight the issues that you can still help with to make these better. I believe Drupal 8 will be a huge release for multilingual, but it can always be even better of course.

<!-- @section -->

# Language first

Good news first: translation is no longer a magic ball, but a first-class citizen.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jun-11/drupal-8-multilingual-tidbits-1-language-first", "text" : "I have seen that I can use my own language right away from the installer, yay!", "title" : "Language first", "description" : "Since it's inception, the heroic efforts of people on the initiative resulted in hundreds of issues resolved but there are always more to perfect. We have made huge advances in terms of multilingual support in Drupal 8 thanks to all these changes and you can still help to make it perfect", "imageUrl" : "http://hojtsy.hu/files/Drupal8Installer.png" -->

<!-- @task,  "text" : "Try installing Drupal 8 in a non-English language." -->

<!-- @section -->

# More core modules

First-class citizens like translation need their own core modules.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jun-12/drupal-8-multilingual-tidbits-2-more-core-modules", "text" : "I have learned that I can achieve more using less modules", "title" : "More core modules", "description" : "Drupal 8 has more core modules handling language related features, yet less requirement for contributed modules to be installed for the most important tasks", "imageUrl" : "http://hojtsy.hu/files/Drupal8MultilingualSystem.png" -->

# Simple language setup, optional English

All languages are first-class citizens, English is not an exception any more.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jun-17/drupal-8-multilingual-tidbits-3-simple-language-setup-optional-english", "text" : "I have understood that English became optional", "title" : "Simple language setup, optional English", "description" : "This part will be about the simple language setup features provided by Language module, which is the base for every other language feature", "imageUrl" : "http://hojtsy.hu/files/Drupal8LanguagesList_0.png" -->

<!-- @task,  "text" : "Try disabling English on your multilingual Drupal 8 site." -->

# Highly flexible detection options

How should the system know what language we want the texts to be displayed in?

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jun-19/drupal-8-multilingual-tidbits-4-highly-flexible-detection-options", "text" : "I have seen how flexible and convenient the language detection is", "title" : "Highly flexible detection options", "description" : "The Drupal 8 language detection and selection options are located the same place they were in Drupal 7 but almost all options got some improvement", "imageUrl" : "http://hojtsy.hu/files/Drupal8LanguageDetectionList_0.png" -->

# Almost limitless language assignment

Given that translation is a first-class citizen, all others should behave accordingly.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jun-21/drupal-8-multilingual-tidbits-5-almost-limitless-language-assignment", "text" : "I have learned that almost everything knows its own language by now", "title" : "Almost limitless language assignment", "description" : "In Drupal 8, one of our most important goals was to make everything know its language as far and wide as possible", "imageUrl" : "http://hojtsy.hu/files/Drupal8ContentLanguageConfig.png" -->

<!-- @task,  "text" : "Poke around Drupal 8 to see how to set a language for different entities like nodes, blocks, views, etc." -->

# Easier right to left styling

Are you writing from right to left? Fear not, Drupal has support for your language as well.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jul-02/drupal-8-multilingual-tidbits-6-easier-right-left-styling", "text" : "I have understood that my site can easily be bidirectional", "title" : "Easier right to left styling", "description" : "One of the strongly supported language features of Drupal is right to left (RTL) language support. For some Drupal core versions, introducing an RTL language on the site is easy", "imageUrl" : "http://hojtsy.hu/files/Drupal8InstallerRTL_0.png" -->

<!-- @task,  "text" : "Enable a right-to-left language on your Drupal 8 site like Hebrew." -->

<!-- @section -->

# Blocks and views

We can use our multilingual tools to reuse and select the building blocks of a page based on the current language.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jul-09/drupal-8-multilingual-tidbits-7-blocks-and-views", "text" : "I have seen that blocks' and views' language-awareness has increased", "title" : "Blocks and views", "description" : "Once you have detailed language information on content, configuration, etc, which is now widely possible in Drupal 8, you can use this data to pull out content for specific languages", "imageUrl" : "http://hojtsy.hu/files/Drupal8ViewsLanguageFilter_0.png" -->

<!-- @task,  "text" : "Set up different custom blocks for different languages." -->

<!-- @section -->

# Transliteration

Having characters in your language's set that are hard to work with (eg. on the filesystem)? Core can convert them to safer ones for you.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jul-17/drupal-8-multilingual-tidbits-8-transliteration", "text" : "I have learned how convenient is the builtin transliteration system", "title" : "Transliteration", "description" : "One thing that was not yet covered is built-in transliteration support. Yes, you read that right. Drupal 8 includes a powerful backend system for transliteration and it even uses it for machine name generation on the frontend", "imageUrl" : "http://hojtsy.hu/files/Drupal8TransliterationHu.png" -->

<!-- @task,  "text" : "Create a content type with an 'áccéntéd' name to see transliteration in action." -->

<!-- @section -->

# Deployment friendly automated downloads

Managing multiple languages in multiple environments of multiple sites got a multitude easier.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jul-23/drupal-8-multilingual-tidbits-9-deployment-friendly-automated-downloads", "text" : "I have understood that translation staging became finally possible", "title" : "Deployment friendly automated downloads", "description" : "The new version separates the responsibilities for the base language layer (Language module) from the software's translation (Interface Translation module), and largely expands on the features of the interface translation capability", "imageUrl" : "http://hojtsy.hu/files/gabor_photo_large.jpg" -->

<!-- @task,  "text" : "Make sure you know where the intermediate .po files are stored." -->

<!-- @section -->

# Context specific text translation APIs

Increased flexibility with regards to multilingualism comes with increased complexity.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-jul-24/drupal-8-multilingual-tidbits-10-context-specific-text-translation-apis", "text" : "I have seen some parts of the wood of the translation APIs", "title" : "Context specific text translation APIs", "description" : "Prior Drupal versions had the rule that you should use t() and format_plural() with little exceptions. Drupal 8 has much more complexity in this area, which may be a bliss or a curse depending on how you look at it", "imageUrl" : "http://hojtsy.hu/files/Drupal7MenuToDrupal8Figure.png" -->

# String customizations tracked

Good news: you will not lose your precious custom translations.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-aug-13/drupal-8-multilingual-tidbits-11-string-customizations-tracked", "text" : "I have learned that my custom translations are kept", "title" : "String customizations tracked", "description" : "We know that not everybody is happy with the community translations proper. So another key feature we included in Drupal 8 is custom translation tracking", "imageUrl" : "http://hojtsy.hu/files/Drupal8StringExportOptions.png" -->

# English can now be translated to

Since English is no longer an exception amongst other languages, it can be a translation target.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-aug-20/drupal-8-multilingual-tidbits-12-english-can-now-be-translated", "text" : "I have understood that I do not need hacks to have custom English strings", "title" : "English can now be translated to", "description" : "By default, if you have English configured, it is not available as a translation target. However, you are only one checkbox away from enabling that feature", "imageUrl" : "http://hojtsy.hu/files/Drupal8EditEnglish_0.png" -->

# Much improved software translation UI

Your translation experience became a whole lot more streamlined.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-aug-20/drupal-8-multilingual-tidbits-13-much-improved-software-translation-ui", "text" : "I have seen the highly convenient translation interface", "title" : "Much improved software translation UI", "description" : "We cut out two unnecessary steps and brought in a very quick translation experience instead which even shows you which translations you changed as you go along", "imageUrl" : "http://hojtsy.hu/files/Drupal8TranslationForm.png" -->

<!-- @task,  "text" : "Have a custom English translation of some UI and configuration texts." -->

<!-- @section -->

# Intro to content and configuration

There are a number of theories behind all this multilingualism.

<!-- @link, "url" : "http://hojtsy.hu/blog/2013-sep-13/drupal-8-multilingual-tidbits-14-intro-content-and-configuration", "text" : "I have learned about the motivational principles behind translation improvements", "title" : "Intro to content and configuration", "description" : "We still have two major categories of improvements to cover, namely content and configuration language and translation. Before we move on to the details, I wanted to post an introduction because there are very similar motivations and guiding principles around the improvements", "imageUrl" : "http://hojtsy.hu/files/ConfigContent.jpg" -->

<!-- @section -->

# Configuration translation basics

To make use of all this jazz, everything should be prepared for it.

<!-- @link, "url" : "http://hojtsy.hu/blog/2014-may-19/drupal-8-multilingual-tidbits-15-configuration-translation-basics", "text" : "I have understood that internationalization is no longer an option, but a must", "title" : "Configuration translation basics", "description" : "The biggest value for non-English and multilingual sites in Drupal 8 of the configuration changes is that now a common system is used to manage your site name, email text settings through to views, field settings, entity form displays, etc. We can introduce language and translation support in a way that modules will need to plan with. It is not just an optional contributed add-on but a core feature", "imageUrl" : "http://hojtsy.hu/files/Drupal8ConfigTranslationLanguageStructure.png" -->

# Configuration translation development

Preparation for translatability (also known as internationalization or i18n in short) starts with the coding and translation of configuration.

<!-- @link, "url" : "http://hojtsy.hu/blog/2014-may-26/drupal-8-multilingual-tidbits-16-configuration-translation-development", "text" : "I have seen how to mark pieces of configuration as translatable and how to provide translations for them", "title" : "Configuration translation development", "description" : "We'll cover how can developers integrate with configuration translation", "imageUrl" : "http://hojtsy.hu/files/ConfigSchemaCheatSheet1.5.jpg" -->

<!-- @task,  "text" : "Translate a configuration item like the name of a vocabulary into a different, non-English language." -->

<!-- @section -->

# Content translation basics

Once configuration is translated, we are ready to delve into content translation.

<!-- @link, "url" : "http://hojtsy.hu/blog/2015-jan-27/drupal-8-multilingual-tidbits-17-content-translation-basics", "text" : "The difference between content and configuration became a bit clearer to me", "title" : "Content translation basics", "description" : "If you also need content translation support, all you need to do is to enable the Content translation module and have multiple languages configured. The same screen can be used to configure content translatability that you already used to configure content language defaults", "imageUrl" : "http://hojtsy.hu/files/Drupal8ContentFields.png" -->

# Core content translation workflow

Most complex systems provide different ways to achieve the same results. You should know what method core supports for content translation.

<!-- @link, "url" : "http://hojtsy.hu/blog/2015-nov-10/drupal-8-multilingual-tidbits-18-core-content-translation-workflow", "text" : "I have learned how to translate content in a core-supported way", "title" : "Core content translation workflow", "description" : "What do we do to translate content?", "imageUrl" : "http://hojtsy.hu/files/Drupal8ContentAdminTranslations.png" -->

# Content translation development

And the circle is closed: once the content is translated, coders should know how to work with it.

<!-- @link, "url" : "http://hojtsy.hu/blog/2015-nov-11/drupal-8-multilingual-tidbits-19-content-translation-development", "text" : "I have understood that it became easier to work with translated content, even from the code", "title" : "Content translation development", "description" : "Drupal 8's entity API handles entities as full fledged objects. Translations of entities may be requested from this object and returned as a reusable entity object as well, which can be treated the same way as the original entity that we loaded", "imageUrl" : "http://hojtsy.hu/files/gabor_photo_large.jpg" -->

<!-- @task,  "text" : "Translate a node into a different, non-English language." -->

<!-- @section -->

# Combination use cases with content and menus

This multilingualism is quite puzzling, isn't it? Well, every puzzle has its own solution, even if it is admittedly a partial one.

<!-- @link, "url" : "http://hojtsy.hu/blog/2015-nov-18/drupal-8-multilingual-tidbits-20-combination-use-cases-content-and-menus", "text" : "I can finally click translatable pieces together to have a smoothly-working multilingual site", "title" : "Combination use cases with content and menus", "description" : "Content shows up with some shipped interface elements, local configuration and content. Menus contain elements from code, content and configuration. It is good to know how these pieces relate so you can translate every piece and know the right place to do it", "imageUrl" : "http://hojtsy.hu/files/Drupal8MenuInSidebar.png" -->

<!-- @task,  "text" : "Prepare the menu on your site as Gábor did." -->
