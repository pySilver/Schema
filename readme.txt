=== Schema ===
Contributors: hishaman, schemapress
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=NGVUBT2QXN7YL
Tags: schema, schema.org, json, json-ld, google, seo, structured data, markup, search engine, search, rich snippets, social, post, page, plugin, wordpress, content, article, news, search results, site name, knowledge graph, social, social profiles, keywords, meta-tags, metadata, tags, categories, optimize, ranking, search engine optimization, search engines, serp, sitelinks, google sitelinks, sitelinks search box, google sitelinks search box, semantic, structured, canonical, custom post types, post type, title, terms, media, images, thumb, featured, url, video, video markup, video object, VideoObject, video schema, audio object, AudioObject, audio schema, audio, sameAs, about, contact, amp, mobile
Requires at least: 3.0
Tested up to: 4.6.1
Stable tag: 1.6.1

Get the next generation of Schema Structured Data to enhance your WordPress site presentation in Google search results.

== Description ==

Like Schema plugin? Consider leaving a [5 star review](https://wordpress.org/support/plugin/schema/reviews/).

Super fast, light-weight plugin for adding schema.org structured data markup in recommended JSON-LD format automatically to WordPress sites.

Enhanced Presentation in Search Results By including structured data appropriate to your content, your site can enhance its search results and presentation.

Check out the [Plugin Homepage](http://schema.press/) for more info and [documentation](http://schema.press/docs/).


**What is Schema markup?**

Schema markup is code (semantic vocabulary) that you put on your website to help the search engines return more informative results for users. So, Schema is not just for SEO reasons, it’s also for the benefit of the searcher. 

**Schema Key Features**

* Easy to use, set it and forget it, with minimal settings. 
* Enable Schema types at once per custom post type or post category.
* Provide a valid markup, test it in Google Structured Data Testing Tool.
* Output JSON-LD format, the most recommended by Google.
* Can reuse data saved in post meta that is created by other plugins.
* Extensible, means you can extend its functionality via other plugins, extensions or within your Theme’s functions.php file.

**Plugin Extensions**

* [Schema Review](https://wordpress.org/plugins/schema-review/): extend Schema functionality by adding review and rating Structured Data functionality for Editors and Authors. 

**Supported Google/Schema Markups**

* [Knowledge Graph](https://developers.google.com/structured-data/customize/overview)
 * [Logos](https://developers.google.com/structured-data/customize/logos)
 * [Company Contact Numbers](https://developers.google.com/structured-data/customize/contact-points)
 * [Social Profile Links](https://developers.google.com/structured-data/customize/social-profiles)

* Style Your Search Results:
 * [Enable Sitelinks Search Box](https://developers.google.com/structured-data/customize/logos)
 * [Show Your Site Name in Search](https://developers.google.com/structured-data/site-name)

**Supported Schema Types**
 
* Creative Works
 * [Article](https://schema.org/Article) enabled on Pages
  * [BlogPosting](https://schema.org/BlogPosting) enabled on Posts
  * [NewsArticle](https://schema.org/NewsArticle)
  * [Report](https://schema.org/Report)
  * [ScholarlyArticle](https://schema.org/ScholarlyArticle)
  * [TechArticle](https://schema.org/TechArticle)

* [Blog](https://schema.org/Blog) to markup Blog posts list page.
* [CollectionPage](https://schema.org/CollectionPage) to markup Categories.
* [AboutPage](https://schema.org/AboutPage) to markup the About page.
* [ContactPage](https://schema.org/ContactPage) to markup the Contact page.
* [Person](https://schema.org/Person) enabled on Author pages
* [VideoObject](https://schema.org/VideoObject) enable automatically on all videos embedded with oEmbed. Supports VideoPress, YouTube, TED, Vimeo, Dailymotion, and Vine.
* [AudioObject](https://schema.org/AudioObject) enable automatically on all audio embedded with oEmbed. Supports SoundCloud, and Mixcloud.

**Supported Plugins**

 * Yoast SEO
 * AMP plugin
 * WPRichSnippets
 * The SEO Framework
 * Visual Composer

**Supported Themes**

 * Genesis 2.x 
 * Thesis 2.x
 * Divi

**Developers?**

Feel free to [fork the project on GitHub](https://github.com/schemapress/Schema) and submit your contributions via pull request.

== Installation ==

1. Upload the entire `schema` folder to the `/wp-content/plugins/` directory
2. DO NOT change the name of the `schema` folder
3. Activate the plugin through the 'Plugins' menu in WordPress
4. Navigate to the `Schema > Settings` menu to configure the plugin

== Frequently Asked Questions ==

= The plugin isn't working or have a bug? =

Post detailed information about the issue in the [support forum](http://wordpress.org/support/plugin/schema) and we will work to fix it.

= Knowledge Graph is not showing? =

The plugin meant to validate markup in Google Structured Data Testing Tool, we don’t have control over the actual display of Knowledge Graph.

= I see an error in Google Structure Data Testing Tool =

This could be for the following reasons:

 * Image error: This is a missing WordPress Featured image, try to upload a Featured image.
 * Logo error: This is a missing Publisher logo, it can be set in the plugin settings page, Schema > Settings > General > Publisher Logo.

= Compatible with Yoast SEO? =

Yes, Schema plugin will detect Yoast SEO plugin and it will not output any markup on the front page of your site, this means all Knowledge Graph and Site Search output will be generated by Yoast SEO.

= Compatible with AMP plugin? =

Yes, Schema plugin will detect AMP plugin and output a more complete and valid schema.org markup.

== Screenshots ==
1. Knowledge Graph settings tab.
2. Create new schema type screen.
3. Create post meta fields with Post Meta Box generator feature.
4. Google Structured Data Testing Tool.

== Changelog ==

= 1.6.1 =
* Fixed hide VideoObject and AudioObject meta boxes if not enabled in settings.
* Added new hook schema_wp_do_after_settings_updated.
* Added new function schema_wp_json_delete_cache to flush cached json-ld post meta.
* Added flush cached json-ld post meta whenever plugin settings got updated.

= 1.6 =
* Fixed exclude post was not working properly.
* Fixed cached post meta timestamp should be deleted on post save.
* Fixed Schema post type label value.
* Fixed Schema post types was not created on plugin activation.
* Fixed schema reference post meta was not saved for scheduled posts.
* Enhanced gravatar validation function.
* Enhanced Blog markup performance by pulling data from cached post meta.
* Added missing BlogPosting description in Blog page markup.
* Added sameAs markup to BlogPosting property in Blog page markup.
* Added sameAs markup to About page.
* Added sameAs markup to Contact page.
* Added new filter schema_blog_output to allow dev extend markups.
* Added new filter schema_about_page_output to allow dev extend markups.
* Added new filter schema_contact_page_output to allow dev extend markups.
* Added missing post meta to the plugin uninstall function.
* Added new function for recursive array search to admin functions file.
* Modified readme.txt file.

= 1.5.9.9 =
* Fixed category id on category pages.
* Fixed a notice on VideoObject function.
* Fixed Schema JSON-LD not updating by flushing cache on schema type save.
* Added Schema property sameAs core extension.
* Added delete Schema JSON-LD post meta on plugin uninstall.
* Added delete Schema Exclude post meta on plugin uninstall.

= 1.5.9.8 =
* Fixed missing translation in category title.
* Added new filter to schema_category_json to extend category markup.
* Added new function to clear/delete schema json post meta value on post save.
* Added support for schema.org sameAS property for category pages.
* Added new custom taxonomy meta fields class.  
* Added new admin link to the plugin About page. 
* Corrected names of some functions, and renamed files.
* Modified readme.txt file.

= 1.5.9.7 =
* Fixed slow performance by reducing number of queries made by the plugin.
* Fixed post meta generator, empty meta box display.
* Fixed an error on post save, global post variable needed to be called.
* Enhanced overall performance by caching JSON-LD array in post meta. 
* Enhanced author output, now it has been added as a core extension.
* Added new settings to control AudioObject, VideoObject, and Comments.
* Cleaned up some code and moved admin and other functions to its own files.
* Pumped WordPress version, checked and tested with 4.6.1 release.

= 1.5.9.6 =
* Added new extension support for AudioObject.
* Added missing translation to Schema VideoObject settings.
* Enhanced plugin activation process.
* Enhanced update post meta reference.
* Added deprecated functions to its own file.
* Corrected words in the Contextual Help screen.
* Updated the welcome screen.
* Updated the readme.txt file. 

= 1.5.9.5 =
* Fixed post meta generator missing description. 
* Fixed Publisher logo image, image url was not used correctly in some cases.
* Updated plugin settings text fields with placeholder info.
* Updated plugin settings page screenshot.
* Pumped WordPress version, checked and tested with 4.6 release.
* Modified readme.txt file, added link to updated plugin documentation page.

= 1.5.9.4 =
* Fixed capabilities issue, plugin settings was not saving properly.
* Modified readme.txt file, added more info to the FAQ section.

= 1.5.9.3 =
* Added new integration file for Visual Composer plugin.
* Added save new setting field to save the upgraded from version on plugin install. 
* Added new filter schema_output_blog_post.
* Added new filter schema_output_category_post.
* Added new filter schema_wp_exclude.
* Added size class for post meta field with the type of number.
* Added new Contextual Help tab to the plugin settings page.
* Added new filters and hooks to allow developers to extend the settings page.
* Added new features for extensions, now it supports licenses and auto upgrades. 
* Added new settings field for Publisher Logo.
* Fixed schema markup for Publisher Logo. 
* Fixed schema markup for Organization Logo.
* Enhanced preview image display in plugin settings, set width to 300px.
* Enhanced wording in plugin settings page and simplified settings fields.

= 1.5.9.2 =
* Removed the Disable SiteLinks Search Box feature, not needed in the plugin.
* Removed the Content tab within the plugin settings page.
* Enhanced the plugin settings page, rearranged settings in a simpler way.

= 1.5.9.1 =
* Fixed a warning notice when saving drafts in editor, editing posts was not possible.

= 1.5.9 =
* Fixed query conflicts on category pages by creating a secondary loop.
* Fixed category description, apply strip_tags function to remove HTML tags.
* Added check to prevent processing code in backend when runs category schema.
* Added new Post Meta Box feature.
* Added a new schema_wp_filter_content filter.
* Added new integration filter function for Divi theme.
* Use wp_strip_all_tags instead of strip_tags for short content.
* Updated plugin screenshots, added a new screenshot for post meta box feature.
* Corrected a typo in plugin settings page.
* Modified readme.txt file, corrected link to support forum and some typos.  

= 1.5.8 =
* Fixed datePublished and dateModified markups, make sure it is in ISO 8601 format.
* Fixed Preview button was not showing in edit screen.
* Extended the plugin settings extensibility with new repeatable field type.
* Enhanced post meta wording and fixed typos.
* Modified readme.txt file, corrected link to support forum and some typos.  

= 1.5.7 =
* Added support for schema type CollectionPage for Categories.
* Added new filter schema_wp_types to override or extend options.
* Added new filter schema_wp_publisher to override publisher array.
* Added new filter schema_wp_author to override author array.
* Added new function schema_wp_do_post_meta to allow adding custom post meta boxes.
* Added new function to return Author array.

= 1.5.6 =
* Fixed a notice on front end caused when admin bar menu is called.
* Added new post meta box for Schema exclusions, turn off Schema on specific posts.
* Added new integration for SEO Framework plugin.
* Modified search_term to search_term_string search variable in SiteLinks Search Box.
* Enhanced WPRichSnippets integration, put code on its own file.
* Enhanced Yoast SEO integration, put code on its own file.
* Enhanced functions naming to prevent any possible conflict with Schema Removal.
* Updated the plugin welcome page.
* Modified readme.txt file.

= 1.5.5 =
* Fixed a fatal error when Genesis is not the active Theme.

= 1.5.4 =
* Added admin notification for feedback.
* Added support for Schema type Blog, markup blog post list.
* Added new function to retrieve post comments.
* Added admin bar menu item for easy Structured Data testing access.
* Added a check if WPRichSnippets plugin is active, remove its admin bar menu.
* Added integration with Genesis Framework.
* Enhanced Media function, check for images in content if Featured image not found.
* Enhanced plugin wording in menu, change Schema Types to read Types, make it simple.
* Updated the plugin welcome page.
* Modified readme.txt file.

= 1.5.3 =
* Added better support for enabled AMP post types.
* Added support Schema for comment to markup comments in Article types.
* Added support Schema for commentCount markup to Article types.
* Added new filter to override default comments number to include in markups.
* Added better support for author, now include description and gravatar. 
* Added support for author sameAs for social profiles if provided in user account.
* Added GNU GENERAL PUBLIC LICENSE file.
* Added README.md

= 1.5.2 =
* Fixed a warning on 404 and search result pages.
* Added new schema type AboutPage, core extension for the about page.
* Added new schema type ContactPage, core extension for the contact page.
* Added new settings under the Content tab to select About and Contact pages.
* Updated the plugin welcome page.
* Modified readme.txt file.

= 1.5.1 =
* Fixed an error, AMP was not working because a call to wrong function.
* Fixed wrong Class name for post meta creation.
* Fixed schema output when set a static page as Front page. 
* Fixed a bug in WPRichSnippets integration on pages that includes VideoObject.
* Added several checks not to process oEmbed unless an embedded video is in content. 
* Tested with WordPress, version 4.5.3 release.
* Updated the plugin welcome page. 

= 1.5 =
* Fixed error caused on plugin activation.
* Fixed Schema post was saved as a draft.
* Added ability to filter the Schema JSON array schema_json.
* Added support for Schema VideoObject markups through oEmbed.
* Added new post meta box features for VideoObject with Schema type edit page.
* Added new post meta box features for completing missing video info.
* Modified wording in the Schema post type post meta.
* Modified the Publish button to read Save.

= 1.4.7 =
* Fixed admin notices by adding conditions to run the Auto Featured image script. 
* Added new ability to filter schema markups to work with post categories.
* Added new function to automatically save categories in Schema post meta.
* Added an alert on Schema post save when no Post Type is selected.
* Enhanced the default submit box on Schema post type and made cleaner. 
* Removed the Preview button from Create Schema meta box.
* Modified the Publish button in Create Schema meta box to read “Create Schema”.
* Updated the plugin welcome page.
* Modified readme.txt file.

= 1.4.6 =
* Added ability to set Featured image automatically.
* Added back settings Content tab.
* Fixed post id in schema output function.
* Fixed admin notices.
* Modified readme.txt file.

= 1.4.5 =
* Added Person schema to author archive pages.
* Added schema keywords to BlogPosting.
* Added a new function to retrieve post first category to be set as articleSection.
* Now play nice with WPRichSnippets plugin, do not output schema if WPRS is enabled.
* Fixed notices in edit screen by running functions only on schema post type screen.

= 1.4.4 =
* Added support for schema specific type Article > Report.
* Added new filter schema_wp_cpt_enabled to override enabled post types array.
* Added new function to insert schema post ref on wp_insert_post.
* Added new function to insert meta post ref on schema type save.
* Added insert ref on plugin activation for post and page post types.
* Added delete ref on uninstall.
* Fixed media, do not output media if image width and height are not presented. 

= 1.4.3 =
* Fixed media output, do not output media if image url is not presented. 

= 1.4.2 =
* Fixed invalid Thesis post image url, make sure url is a valid one.

= 1.4.1 =
* Fixed avoid running schema output on home page and archive pages.

= 1.4 =
* Introduced new way to output schema.
* Added new schema post type to allow users to create new Schema types.
* Added new post meta functions for easy creation.
* Added the ability to enable Schema.org markups on Post Type bases.
* Added automatically insert post and page schema types on plugin activation.
* Added new schema types, now Article can have sub types.
* Added a new function for media handling.
* Added new filter schema_output for overriding schema output array.
* Added integration for Thesis theme 2.x Post Image.
* Added check version, if below 1.4 run required functions on activation.
* Removed functions that has been used to output schema in version 1.3
* Removed the content tab from settings page. 
* Fixed uninstall.php issue, it was not working properly on multisite.
* Cleaned admin styles file.
* Enhanced the plugin Welcome page.
* Updated plugin screenshots.
* Modified readme.txt file.

= 1.3 =
* Added integration for AMP plugin, Schema will take over for better schema output handling.
* Enhanced JSON-LD output functions.

= 1.2 =
* Added new schema type BlogPosting.
* Switched blog posts schema to BlogPosting.
* Set schema for Article on page post type.
* Added new filters schema_blog_posting to override schema BlogPosting array output.
* Added new filters schema_article to override schema Article array output.
* Added new screenshot.
* Modified readme.txt file.

= 1.1.1 =
* Now play nicely with Yoast SEO plugin.
* Updated screenshot.
* Modified readme.txt file.

= 1.1 =
* Added new settings tab for content.
* Added support for schema type Article on blog posts.
* Fixed a bug within plugin settings functions.

= 1.0 =
* Initial Release

== Upgrade Notice ==

= 1.6.1 =
In this update, a bug got fixed and a couple of other enhancements which enhance plugin settings usability has been applied. Please, upgrade now to get these enhancements.

= 1.6 =
Several bug fixes and enhancement has been done in this release, plus a new extension release for Schema Review. Please, upgrade now to get these enhancements.

= 1.5.9.9 =
Several bug fixes and enhancement has been made to the plugin in this release, plus a new sameAs property for your content. Please, upgrade now to get these enhancements.

= 1.5.9.8 =
More enhancement has been made to the plugin in this release, plus a couple of new features. Please, upgrade now to get these enhancements.

= 1.5.9.7 =
This update includes enhancement to performance by caching JSON-LD output in post meta, this will reduce database queries and make your site loads faster. Please, upgrade now to get these enhancements. 

= 1.5.9.6 =
This update includes enhancement to plugin activation, support for schema.org AudioObject and more. Please, upgrade now to get these enhancements. 

= 1.5.9.5 =
This update has an important fix for Publisher logo and some other functions in the plugin. Please, upgrade now to get this fix. 

= 1.5.9.4 =
This update has an important fix for capabilities, plugin settings was not saving properly on newly installed sites. Please, upgrade now to get this fix. 

= 1.5.9.3 =
This update has several features and enhancements, fix for Publisher Logo image, and support for Visual Composer plugin. Please, upgrade now to get this fix. 

= 1.5.9.2 =
In this release, the disable SiteLinks Search Box feature has been removed, this feature was causing issues and having a bug. Please, upgrade now to get this fix. 

= 1.5.9.1 =
This release has a bug fix for a warning notice when saving drafts in editor, editing posts was not possible. Please update the plugin on your website to git this important fix.

= 1.5.9 =
In this release, reported bugs has been fixed. Also, new fixes and integration for Divi theme has been introduced. Please, update the plugin on your website now to get fixes and enhancements.

= 1.5.8 =
In this release, reported bugs has been fixed. Please, update the plugin on your website now to get fixes and enhancements.

= 1.5.7 =
In this release, a new Schema type CollectionPage has been added to empower your site Categories. Please, update the plugin on your website now to get the new enhancements.

= 1.5.6 =
In this release, new integration for SEO Framework plugin and other cool features has been introduced. Please, update the plugin on your website now to get the new enhancements.

= 1.5.5 =
Fixed a fatal error. Please, update the plugin on your website now to get the new enhancements.

= 1.5.4 =
In this release, a good set of enhancements has been added, also introduced new Schema type Blog, which markup your Blog posts page automatically. Also added integration for Genesis Framework. Please, update the plugin on your website now to get the new enhancements.

= 1.5.3 =
In this release, a better support added to AMP pages, now the plugin will work on post types enabled AMP pages if found, and present Schema type by ref post meta saved in each post. Also added support Schema markup for comments. Please, update the plugin on your website now to get the new enhancements.

= 1.5.2 =
New features introduced in this update release, fixed a minor warning on 404 pages. Please, update the plugin on your website now to get this fix and new features.

= 1.5.1 =
Fixed a fatal error on AMP posts, also another fix for VideoObject. Please, update the plugin on your website now to get this fix and other enhancements.

= 1.5 =
Fixed a fatal error on plugin activation, added VideoObject support and more awesome enhancements. Please, update the plugin on your website now to get this fix and other enhancements.

= 1.4.8 =
Fixed an important bug within the plugin, Schema post was saved as draft and no way to set is as publish.Please, update the plugin on your website now to get this fix and other enhancements.

= 1.4.6 =
Added ability to set Featured image automatically when creating or editing a post. Added back settings Content tab. Fixed admin notices and bugs. A few minor code/ documentation tweaks, updated readme.txt file with new details. Please, update the plugin on your website now to get bug fixes, enhancements and new cool features in this release. 