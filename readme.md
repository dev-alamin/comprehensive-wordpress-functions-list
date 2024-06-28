# WordPress Most Used Functions

## Introduction
This repository contains a collection of the most frequently used WordPress functions, filters, and actions, organized by category for easy reference.

## How to Use
Browse the categories to find the functions you need. Each category contains a set of functions with descriptions, usage examples, and best practices.

## Categories
- [General Functions](#general-functions)
- [Validation Functions](#validation-functions)
- [Filters](#filters)
- [Actions](#actions)
- [Custom Post Types](#custom-post-types)
- [Security Functions](#security-functions)
- [Database Functions](#database-functions)
- [API Functions](#api-functions)

### general-functions.md

# General Functions
Certainly! Here's how you can format your markdown file to present each function as a code block with its description and parameters:

```markdown
## get_template_directory()

```php
<?php
// Retrieves the absolute path to the template directory.
get_template_directory();
?>
```
**Description:** Retrieves the absolute path to the template directory.  
**Parameters:** None  

---

## get_stylesheet_directory()

```php
<?php
// Retrieves the absolute path to the stylesheet directory.
get_stylesheet_directory();
?>
```
**Description:** Retrieves the absolute path to the stylesheet directory.  
**Parameters:** None  

---

## get_template_directory_uri()

```php
<?php
// Retrieves the URI of the template directory.
get_template_directory_uri();
?>
```
**Description:** Retrieves the URI of the template directory.  
**Parameters:** None  

---

## get_stylesheet_directory_uri()

```php
<?php
// Retrieves the URI of the stylesheet directory.
get_stylesheet_directory_uri();
?>
```
**Description:** Retrieves the URI of the stylesheet directory.  
**Parameters:** None  

---

## get_home_url($blog_id = null, $path = '', $scheme = null)

```php
<?php
// Retrieves the home URL for the current site.
get_home_url($blog_id = null, $path = '', $scheme = null);
?>
```
**Description:** Retrieves the home URL for the current site.  
**Parameters:**  
- `$blog_id` (int) Optional. Site ID. Default null.  
- `$path` (string) Optional. Path relative to the home URL. Default ''.  
- `$scheme` (string|null) Optional. Scheme to give the home URL context. Accepts 'http', 'https', or 'relative'. Default null.  

---

## get_site_url($blog_id = null, $path = '', $scheme = null)

```php
<?php
// Retrieves the site URL for the current site.
get_site_url($blog_id = null, $path = '', $scheme = null);
?>
```
**Description:** Retrieves the site URL for the current site.  
**Parameters:**  
- `$blog_id` (int) Optional. Site ID. Default null.  
- `$path` (string) Optional. Path relative to the site URL. Default ''.  
- `$scheme` (string|null) Optional. Scheme to give the site URL context. Accepts 'http', 'https', or 'relative'. Default null.  

---

## get_admin_url($blog_id = null, $path = '', $scheme = 'admin')

```php
<?php
// Retrieves the admin URL for the current site.
get_admin_url($blog_id = null, $path = '', $scheme = 'admin');
?>
```
**Description:** Retrieves the admin URL for the current site.  
**Parameters:**  
- `$blog_id` (int) Optional. Site ID. Default null.  
- `$path` (string) Optional. Path relative to the admin URL. Default ''.  
- `$scheme` (string) Optional. Scheme to give the admin URL context. Default 'admin'.  

---

## site_url($path = '', $scheme = null)

```php
<?php
// Retrieves the site URL.
site_url($path = '', $scheme = null);
?>
```
**Description:** Retrieves the site URL.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the site URL. Default ''.  
- `$scheme` (string|null) Optional. Scheme to give the site URL context. Accepts 'http', 'https', or 'relative'. Default null.  

---

## home_url($path = '', $scheme = null)

```php
<?php
// Retrieves the home URL.
home_url($path = '', $scheme = null);
?>
```
**Description:** Retrieves the home URL.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the home URL. Default ''.  
- `$scheme` (string|null) Optional. Scheme to give the home URL context. Accepts 'http', 'https', or 'relative'. Default null.  

---

## admin_url($path = '', $scheme = 'admin')

```php
<?php
// Retrieves the admin URL.
admin_url($path = '', $scheme = 'admin');
?>
```
**Description:** Retrieves the admin URL.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the admin URL. Default ''.  
- `$scheme` (string) Optional. Scheme to give the admin URL context. Default 'admin'.  

---

## includes_url($path = '', $scheme = null)

```php
<?php
// Retrieves the URL to the includes directory.
includes_url($path = '', $scheme = null);
?>
```
**Description:** Retrieves the URL to the includes directory.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the includes URL. Default ''.  
- `$scheme` (string|null) Optional. Scheme to give the includes URL context. Accepts 'http', 'https', or 'relative'. Default null.  

---

## content_url($path = '')

```php
<?php
// Retrieves the URL to the content directory.
content_url($path = '');
?>
```
**Description:** Retrieves the URL to the content directory.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the content URL. Default ''.  

---

## plugins_url($path = '', $plugin = '')

```php
<?php
// Retrieves the URL to the plugins directory or to a specific plugin.
plugins_url($path = '', $plugin = '');
?>
```
**Description:** Retrieves the URL to the plugins directory or to a specific plugin.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the plugins URL. Default ''.  
- `$plugin` (string) Optional. The plugin file path to be relative to. Default ''.  

---

## wp_upload_dir($time = null, $create_dir = true, $refresh_cache = false)

```php
<?php
// Retrieves an array containing the current upload directory's path and URL.
wp_upload_dir($time = null, $create_dir = true, $refresh_cache = false);
?>
```
**Description:** Retrieves an array containing the current upload directory's path and URL.  
**Parameters:**  
- `$time` (string|int|null) Optional. Time to determine the upload subdirectory. Default null.  
- `$create_dir` (bool) Optional. Whether to check and create the uploads directory. Default true.  
- `$refresh_cache` (bool) Optional. Whether to refresh the cache. Default false.  

---

## get_the_ID()

```php
<?php
// Retrieves the ID of the current item in the WordPress Loop.
get_the_ID();
?>
```
**Description:** Retrieves the ID of the current item in the WordPress Loop.  
**Parameters:** None  

---

## get_the_title($post = 0)

```php
<?php
// Retrieves the title of a specified post.
get_the_title($post = 0);
?>
```
**Description:** Retrieves the title of a specified post.  
**Parameters:**  
- `$post` (int|WP_Post) Optional. Post ID or post object. Default 0.  

---

## get_the_permalink($post = 0)

```php
<?php
// Retrieves the permalink for a specified post.
get_the_permalink($post = 0);
?>
```
**Description:** Retrieves the permalink for a specified post.  
**Parameters:**  
- `$post` (int|WP_Post) Optional. Post ID or post object. Default 0.  

---

## the_content($more_link_text = null, $strip_teaser = false)

```php
<?php
// Displays the content of the current post.
the_content($more_link_text = null, $strip_teaser = false);
?>
```
**Description:** Displays the content of the current post.  
**Parameters:**  
- `$more_link_text` (string|null) Optional. Content for when there is more text. Default null.  
- `$strip_teaser` (bool) Optional. Whether to strip the teaser content before the more text. Default false.  

---

## get_the_content($more_link_text = null, $strip_teaser = false)

```php
<?php
// Retrieves the content of the current post.
get_the_content($more_link_text = null, $strip_teaser = false);
?>
```
**Description:** Retrieves the content of the current post.  
**Parameters:**  
- `$more_link_text` (string|null) Optional. Content for when there is more text. Default null.  
- `$strip_teaser` (bool) Optional. Whether to strip the teaser content before the more text. Default false.  

---

## wp_nav_menu($args = [])

```php
<?php
// Displays a navigation menu.
wp_nav_menu($args = []);
?>
```
**Description:** Displays a navigation menu.  
**Parameters:**  
- `$args` (array) Optional. Array of arguments for displaying the navigation menu. Default empty array.  

---

## get_search_query($escaped = true)

```php
<?php
// Retrieves the contents of the search query variable.
get_search_query($escaped = true);
?>
```
**Description:** Retrieves the contents of the search query variable.  
**Parameters:**  
- `$escaped` (bool) Optional. Whether to escape the search query. Default true.  

---

## is_user_logged_in()

```php
<?php
// Checks if the current visitor is a logged-in user.
is_user_logged_in();
?>
```
**Description:** Checks if the current visitor is a logged-in user.  
**Parameters:** None  

---

## wp_logout()

```php
<?php
// Logs the current user out.
wp_logout();
?>
```
**Description:** Logs the current

 user out.  
**Parameters:** None  

---

## wp_login_url($redirect = '', $force_reauth = false)

```php
<?php
// Retrieves the login URL.
wp_login_url($redirect = '', $force_reauth = false);
?>
```
**Description:** Retrieves the login URL.  
**Parameters:**  
- `$redirect` (string) Optional. URL to redirect to after logging in. Default ''.  
- `$force_reauth` (bool) Optional. Whether to force reauthorization. Default false.  

---

## wp_logout_url($redirect = '')

```php
<?php
// Retrieves the logout URL.
wp_logout_url($redirect = '');
?>
```
**Description:** Retrieves the logout URL.  
**Parameters:**  
- `$redirect` (string) Optional. URL to redirect to after logging out. Default ''.  

---

## wp_register($before = '', $after = '', $echo = true)

```php
<?php
// Displays the "Site Admin" and "Register" links.
wp_register($before = '', $after = '', $echo = true);
?>
```
**Description:** Displays the "Site Admin" and "Register" links.  
**Parameters:**  
- `$before` (string) Optional. Text to display before the links. Default ''.  
- `$after` (string) Optional. Text to display after the links. Default ''.  
- `$echo` (bool) Optional. Whether to display or return. Default true.  

---

## wp_tag_cloud($args = '')

```php
<?php
// Displays a tag cloud.
wp_tag_cloud($args = '');
?>
```
**Description:** Displays a tag cloud.  
**Parameters:**  
- `$args` (array|string) Optional. Arguments to display the tag cloud. Default empty string.  

### validation-functions.md

# Validation Functions

## is_email($email)
**Description:** Validates an email address.  
**Parameters:**  
- `$email` (string) Email address to validate.  

## is_user_logged_in()
**Description:** Checks if the current visitor is a logged-in user.  
**Parameters:** None  

## is_admin()
**Description:** Checks if the current request is for an administrative interface page.  
**Parameters:** None  

## current_user_can($capability)
**Description:** Checks if the current user has a specific capability.  
**Parameters:**  
- `$capability` (string) Capability to check.  

## wp_verify_nonce($nonce, $action = -1)
**Description:** Verifies that a nonce is correct and unexpired.  
**Parameters:**  
- `$nonce` (string) Nonce to verify.  
- `$action` (int|string) Optional. The action name. Default -1.  

## check_admin_referer($action = -1, $query_arg = '_wpnonce')
**Description:** Verifies the AJAX request to prevent processing requests external of the blog.  
**Parameters:**  
- `$action` (int|string) Optional. Action nonce. Default -1.  
- `$query_arg` (string) Optional. Nonce query parameter. Default '_wpnonce'.  

## check_ajax_referer($action = -1, $query_arg = false, $die = true)
**Description:** Verifies the AJAX request to prevent processing requests external of the blog.  
**Parameters:**  
- `$action` (int|string) Optional. Action nonce. Default -1.  
- `$query_arg` (false|string) Optional. Key to check for the nonce. Default false.  
- `$die` (bool) Optional. Whether to die if the nonce is invalid. Default true.  

## current_user_can_for_blog($blog_id, $capability)
**Description:** Checks if the current user has a specific capability for a given site.  
**Parameters:**  
- `$blog_id` (int) Site ID.  
- `$capability` (string) Capability to check.  

## has_cap($capability)
**Description:** Checks if the user has a specific capability.  
**Parameters:**  
- `$capability` (string) Capability to check.  

## validate_file($file, $allowed_files = [])
**Description:** Validates a file name and path for security reasons.  
**Parameters:**  
- `$file` (string) File path.  
- `$allowed_files` (array) Optional. List of allowed files. Default empty array.  

## wp_validate_auth_cookie($cookie = '', $scheme = '')
**Description:** Validates authentication cookies.  
**Parameters:**  
- `$cookie` (string) Optional. If specified, will validate the specified cookie. Default ''.  
- `$scheme` (string) Optional. Authentication scheme. Default ''.  

## wp_validate_redirect($location, $default = '')
**Description:** Validates a URL for use in a redirect.  
**Parameters:**  
- `$location` (string) The URL to validate.  
- `$default` (string) Optional. Default URL to return if `$location` is not valid. Default ''.  

## validate_username($username)
**Description:** Validates a username.  
**Parameters:**  
- `$username` (string) Username to validate.  

## is_serialized($data, $strict = true)
**Description:** Checks if data is serialized.  
**Parameters:**  
- `$data` (mixed) Data to check.  
- `$strict` (bool) Optional. Whether to be strict about the end of the string. Default true.  

## is_serialized_string($data)
**Description:** Checks if a string is serialized.  
**Parameters:**  
- `$data` (string) String to check.  

## is_ssl()
**Description:** Determines if SSL is used.  
**Parameters:** None  

## is_multisite()
**Description:** Determines if Multisite is enabled.  
**Parameters:** None  

## is_main_site($site_id = null)
**Description:** Determines if the current site is the main site.  
**Parameters:**  
- `$site_id` (int|null) Optional. Site ID to check. Default null.  

## wp_validate_boolean($value)
**Description:** Validates a boolean variable.  
**Parameters:**  
- `$value` (mixed) Value to validate.

### filters.md

# Filters

## the_title
**Description:** Filters the post title.  
**Parameters:**  
- `$title` (string) The post title.  
- `$id` (int) The post ID.  

## the_content
**Description:** Filters the post content.  
**Parameters:**  
- `$content` (string) The post content.  

## the_excerpt
**Description:** Filters the post excerpt.  
**Parameters:**  
- `$excerpt` (string) The post excerpt.  

## wp_title
**Description:** Filters the text of the page title.  
**Parameters:**  
- `$title` (string) The page title.  
- `$sep` (string) The separator.  
- `$seplocation` (string) The location of the separator (left or right).  

## wp_nav_menu_items
**Description:** Filters the HTML list content for navigation menus.  
**Parameters:**  
- `$items` (string) The HTML list content for the menu items.  
- `$args` (object) An object containing wp_nav_menu() arguments.  

## wp_list_pages
**Description:** Filters the HTML output of list pages.  
**Parameters:**  
- `$output` (string) The HTML output of list pages.  
- `$args` (array) An array of arguments.  

## the_author
**Description:** Filters the display name of the author.  
**Parameters:**  
- `$display_name` (string) The author's display name.  

## comment_text
**Description:** Filters the comment text.  
**Parameters:**  
- `$comment_text` (string) The comment text.  
- `$comment` (WP_Comment) The comment object.  

## get_avatar
**Description:** Filters the avatar.  
**Parameters:**  
- `$avatar` (string) The avatar image tag.  
- `$id_or_email` (mixed) The Gravatar to retrieve.  
- `$size` (int) The size of the avatar.  
- `$default` (string) URL to a default image to use if no avatar is available.  
- `$alt` (string) Alternative text to use in the avatar image tag.  

## get_search_form
**Description:** Filters the search form HTML.  
**Parameters:**  
- `$form` (string) The search form HTML output.  

## the_date
**Description:** Filters the date a post was published.  
**Parameters:**  
- `$the_date` (string) The formatted date.  
- `$d` (string) The date format.  
- `$post` (WP_Post) The post object.  

## the_time
**Description:** Filters the time a post was published.  
**Parameters:**  
- `$the_time` (string) The formatted time.  
- `$d` (string) The time format.  
- `$post` (WP_Post) The post object.  

## bloginfo
**Description:** Filters the output of blog information.  
**Parameters:**  
- `$output` (string) The blog information.  
- `$show` (string) The type of information to retrieve.  

## wp_mail_from
**Description:** Filters the email address to send from.  
**Parameters:**  
- `$from_email` (string) The email address.  

## wp_mail_from_name
**Description:** Filters the name to associate with the "from" email address.  
**Parameters:**  
- `$from_name` (string) The name associated with the "from" email address.  

## pre_get_posts
**Description:** Allows altering the main query before it is executed.  
**Parameters:**  
- `$query` (WP_Query) The WP_Query instance (passed by reference).  

## wp_get_attachment_image_src
**Description:** Filters the image src result.  
**Parameters:**  
- `$image` (array|false) The image src result array or false if no image is available.  
- `$attachment_id` (int) Image attachment ID.  
- `$size` (string|array) Size of image.  
- `$icon` (bool) Whether the image should be treated as an icon.  

## the_category
**Description:** Filters the list of categories for a post.  
**Parameters:**  
- `$thelist` (string) List of categories.  
- `$separator` (string) Separator used between categories.  
- `$parents` (string) How to display category parents.  

## the_tags
**Description:** Filters the list of tags for a post.  
**Parameters:**  
- `$tag_list` (string) List of tags.  
- `$before` (string) String to use before tags.  
- `$sep` (string) Separator used between tags.  
- `$after` (string) String to use after tags.  

## excerpt_length
**Description:** Filters the length of the excerpt.  
**Parameters:**  
- `$length` (int) The number of words in the excerpt.  

## excerpt_more
**Description:** Filters the "read more" excerpt string.  
**Parameters:**  
- `$more` (string) The string shown within the more link.  

## upload_mimes
**Description:** Filters the list of allowed mime types and file extensions.  
**Parameters:**  
- `$mimes` (array) Mime types keyed by the file extension regex corresponding to those types.  

## widget_text
**Description:** Filters the content of the text widget.  
**Parameters:**  
- `$text` (string) The widget content.  
- `$instance` (array) The current widget instance's settings.  

## wp_generate_attachment_metadata
**Description:** Filters the attachment meta data.  
**Parameters:**  
- `$metadata` (array) An array of attachment meta data.  
- `$attachment_id` (int) Current attachment ID.  

## term_links-post_tag
**Description:** Filters the term links for the post tags.  
**Parameters:**  
- `$term_links` (array) An array of term links.  
- `$taxonomy` (string) Taxonomy name.  

### actions.md

# Actions

## init
**Description:** Fires after WordPress has finished loading but before any headers are sent.  
**Parameters:** None  

## wp_enqueue_scripts
**Description:** Fires when scripts and styles are enqueued.  
**Parameters:** None  

## wp_head
**Description:** Fires within the `<head>` section of the theme.  
**Parameters:** None  

## wp_footer
**Description:** Fires before the closing `</body>` tag of the theme.  
**Parameters:** None  

## admin_init
**Description:** Fires as an admin screen or script is being initialized.  
**Parameters:** None  

## admin_menu
**Description:** Fires before the administration menu loads in the admin.  
**Parameters:** None  

## admin_notices
**Description:** Fires after all administrative notices have been added.  
**Parameters:** None  

## save_post
**Description:** Fires when a post or page is updated.  
**Parameters:**  
- `$post_id` (int) Post ID.  
- `$post` (WP_Post) Post object.  
- `$update` (bool) Whether this is an existing post being updated.  

## wp_insert_post
**Description:** Fires once a post has been saved.  
**Parameters:**  
- `$post_id` (int) Post ID.  
- `$post` (WP_Post) Post object.  
- `$update` (bool) Whether this is an existing post being updated.  

## delete_post
**Description:** Fires before a post or page is deleted.  
**Parameters:**  
- `$post_id` (int) Post ID.  

## transition_post_status
**Description:** Fires when a post's status is changed.  
**Parameters:**  
- `$new_status` (string) New post status.  
- `$old_status` (string) Old post status.  
- `$post` (WP_Post) Post object.  

## wp_login
**Description:** Fires after a user has successfully logged in.  
**Parameters:**  
- `$user_login` (string) User's username.  
- `$user` (WP_User) User object.  

## wp_logout
**Description:** Fires after a user has logged out.  
**Parameters:** None  

## user_register
**Description:** Fires after a new user has been registered.  
**Parameters:**  
- `$user_id` (int) User ID.  

## profile_update
**Description:** Fires after a user updates their profile.  
**Parameters:**  
- `$user_id` (int) User ID.  
- `$old_user_data` (WP_User) Object containing user's data prior to update.  

## delete_user
**Description:** Fires immediately before a user is deleted.  
**Parameters:**  
- `$user_id` (int) User ID.  
- `$reassign` (int|null) ID of the user to reassign posts and links to. Default null.  

## wp_ajax_{action}
**Description:** Used to hook into a custom AJAX action for logged-in users.  
**Parameters:** None  

## wp_ajax_nopriv_{action}
**Description:** Used to hook into a custom AJAX action for logged-out users.  
**Parameters:** None  

## wp_loaded
**Description:** Fires once WordPress, all plugins, and the theme are fully loaded and instantiated.  
**Parameters:** None  

## template_redirect
**Description:** Fires before determining which template to load.  
**Parameters:** None  

## wp_before_admin_bar_render
**Description:** Fires before the admin bar is rendered.  
**Parameters:** None  

## wp_after_admin_bar_render
**Description:** Fires after the admin bar is rendered.  
**Parameters:** None  

## comment_post
**Description:** Fires immediately after a comment is inserted into the database.  
**Parameters:**  
- `$comment_id` (int) Comment ID.  
- `$comment_approved` (int|string) 1 if the comment is approved, 0 if not, 'spam' if spam.  

## edit_comment
**Description:** Fires immediately after a comment is updated in the database.  
**Parameters:**  
- `$comment_id` (int) Comment ID.  

## delete_comment
**Description:** Fires immediately before a comment is deleted from the database.  
**Parameters:**  
- `$comment_id` (int) Comment ID.  

## wp_set_comment_status
**Description:** Fires immediately after the comment status is changed in the database.  
**Parameters:**  
- `$comment_id` (int) Comment ID.  
- `$comment_status` (string) New comment status.  

## widgets_init
**Description:** Fires after all default WordPress widgets have been registered and the user has hooked into the register process.  
**Parameters:** None  

## customize_register
**Description:** Fires when Customizer options are being registered.  
**Parameters:**  
- `$wp_customize` (WP_Customize_Manager) WP_Customize_Manager instance.  

## customize_preview_init
**Description:** Fires when Customizer preview is initialized.  
**Parameters:** None  

## switch_theme
**Description:** Fires before the theme is switched.  
**Parameters:**  
- `$new_name` (string) Name of the new theme.  
- `$new_theme` (WP_Theme) WP_Theme instance of the new theme.  

## after_switch_theme
**Description:** Fires after the theme is switched.  
**Parameters:** None  

## wp_upgrade
**Description:** Fires immediately after the core upgrade process is complete.  
**Parameters:**  
- `$wp_version` (string) Current WordPress version.  

## activated_plugin
**Description:** Fires after a plugin has been activated.  
**Parameters:**  
- `$plugin` (string) Path to the plugin file relative to the plugins directory.  
- `$network_wide` (bool) Whether to enable the plugin for all sites in the network or just the current site. Default false.  

## deactivated_plugin
**Description:** Fires after a plugin has been deactivated.  
**Parameters:**  
- `$plugin` (string) Path to the plugin file relative to the plugins directory.  
- `$network_wide` (bool) Whether to disable the plugin for all sites in the network or just the current site. Default false.  

## register_sidebar
**Description:** Fires after a sidebar has been registered.  
**Parameters:**  
- `$sidebar` (array) Arguments for the registered sidebar.  

## wp_create_user
**Description:** Fires immediately after a new user is created.  
**Parameters:**  
- `$user_id` (int) User ID.  
- `$userdata` (array) Array of user data.  

## lostpassword_post
**Description:** Fires before the lost password form is submitted.  
**Parameters:** None  

## retrieve_password
**Description:** Fires before a new password is retrieved.  
**Parameters:**  
- `$user_login` (string) User login or email.  

## password_reset
**Description:** Fires after the user has reset their password.  
**Parameters:**  
- `$user` (WP_User) User object.  
- `$new_pass` (string) New user password.  

## import_start
**Description:** Fires at the start of an import.  
**Parameters:** None  

## import_end
**Description:** Fires at the end of an import.  
**Parameters:** None  

## wp_scheduled_delete
**Description:** Fires when WordPress's scheduled task for deleting old trash posts runs.  
**Parameters:** None  

## clean_post_cache
**Description:** Fires immediately after the post's cache is cleaned.  
**Parameters:**  
- `$post_id` (int) Post ID.  

## save_post_{post_type}
**Description:** Fires when a post of a specific post type is updated.  
**Parameters:**  
- `$post_id` (int) Post ID.  
- `$post` (WP_Post) Post object.  
- `$update` (bool) Whether this is an existing post being updated.

### custom-post-types.md

# Custom Post Types

## register_post_type($post_type, $args = [])
**Description:** Registers a custom post type.  
**Parameters:**  
- `$post_type` (string) Post type key.  
- `$args` (array) Optional. Array of arguments for registering a custom post type.  

## unregister_post_type($post_type)
**Description:** Unregisters a custom post type.  
**Parameters:**  
- `$post_type` (string) Post type key.  

## register_taxonomy($taxonomy, $object_type, $args = [])
**Description:** Registers a taxonomy for a post type.  
**Parameters:**  
- `$taxonomy` (string) Taxonomy key.  
- `$object_type` (array|string) Object type or array of object types for the taxonomy object.  
- `$args` (array) Optional. Array of arguments for registering a taxonomy.  

## unregister_taxonomy($taxonomy)
**Description:** Unregisters a taxonomy.  
**Parameters:**  
- `$taxonomy` (string) Taxonomy key.  

## register_taxonomy_for_object_type($taxonomy, $object_type)
**Description:** Adds an already registered taxonomy to an object type.  
**Parameters:**  
- `$taxonomy` (string) Taxonomy key.  
- `$object_type` (string) Object type key.  

## unregister_taxonomy_for_object_type($taxonomy, $object_type)
**Description:** Removes a taxonomy from an object type.  
**Parameters:**  
- `$taxonomy` (string) Taxonomy key.  
- `$object_type` (string) Object type key.  

## get_post_type($post = null)
**Description:** Retrieves the post type of the current post or of a given post.  
**Parameters:**  
- `$post` (int|WP_Post|null) Optional. Post ID or post object. Default null.  

## get_post_types($args = [], $output = 'names', $operator = 'and')
**Description:** Retrieves a list of registered post types.  
**Parameters:**  
- `$args` (array) Optional. An array of key-value arguments to match against the post type objects. Default empty array.  
- `$output` (string) Optional. The type of output to return. Accepts 'names' or 'objects'. Default 'names'.  
- `$operator` (string) Optional. Logical operation to perform. Accepts 'and' or 'or'. Default 'and'.  

## get_post_type_object($post_type)
**Description:** Retrieves the post type object.  
**Parameters:**  
- `$post_type` (string) Post type key.  

## post_type_exists($post_type)
**Description:** Checks if a post type is registered.  
**Parameters:**  
- `$post_type` (string) Post type key.  

## is_post_type_hierarchical($post_type)
**Description:** Determines whether the post type is hierarchical.  
**Parameters:**  
- `$post_type` (string) Post type key.  

## get_post_type_archive_link($post_type)
**Description:** Retrieves the archive link for a post type.  
**Parameters:**  
- `$post_type` (string) Post type key.  

## get_post_type_labels($post_type_object)
**Description:** Retrieves an object with labels for the post type.  
**Parameters:**  
- `$post_type_object` (object) Post type object.  

## post_type_archive_title($prefix = '', $display = true)
**Description:** Displays or retrieves the post type archive title.  
**Parameters:**  
- `$prefix` (string) Optional. Prefix before the title. Default ''.  
- `$display` (bool) Optional. Whether to display or retrieve the title. Default true.  

## is_post_type_archive($post_types = '')
**Description:** Determines whether the query is for an existing post type archive page.  
**Parameters:**  
- `$post_types` (string|array) Optional. Post type or array of post types. Default ''.  

## has_term($term = '', $taxonomy = '', $post = null)
**Description:** Checks if the current post has any of the given terms.  
**Parameters:**  
- `$term` (int|string|array) Optional. Term ID, name, slug, or array of such. Default ''.  
- `$taxonomy` (string|array) Optional. Taxonomy name or array of names. Default ''.  
- `$post` (int|WP_Post|null) Optional. Post ID or object. Default null.  

Sure, here is a list of commonly used security functions in WordPress along with their descriptions and parameters:

### security-functions.md

# Security Functions

## wp_nonce_field($action = -1, $name = '_wpnonce', $referer = true, $echo = true)
**Description:** Generates and displays a nonce field for forms.  
**Parameters:**  
- `$action` (int|string) Optional. Action name. Default -1.  
- `$name` (string) Optional. Nonce name. Default '_wpnonce'.  
- `$referer` (bool) Optional. Whether to set the referer field for validation. Default true.  
- `$echo` (bool) Optional. Whether to display or return. Default true.  

## wp_nonce_url($actionurl, $action = -1, $name = '_wpnonce')
**Description:** Adds a nonce to a URL.  
**Parameters:**  
- `$actionurl` (string) URL to add nonce action.  
- `$action` (int|string) Optional. Nonce action name. Default -1.  
- `$name` (string) Optional. Nonce name. Default '_wpnonce'.  

## wp_create_nonce($action = -1)
**Description:** Creates a nonce.  
**Parameters:**  
- `$action` (int|string) Optional. Action name. Default -1.  

## wp_verify_nonce($nonce, $action = -1)
**Description:** Verifies that a nonce is correct and unexpired.  
**Parameters:**  
- `$nonce` (string) Nonce to verify.  
- `$action` (int|string) Optional. Action name. Default -1.  

## current_user_can($capability, ...$args)
**Description:** Checks if the current user has a specific capability.  
**Parameters:**  
- `$capability` (string) Capability name.  
- `...$args` (mixed) Optional. Additional arguments.  

## current_user_can_for_blog($blog_id, $capability, ...$args)
**Description:** Checks if the current user has a specific capability for a specific blog.  
**Parameters:**  
- `$blog_id` (int) Blog ID.  
- `$capability` (string) Capability name.  
- `...$args` (mixed) Optional. Additional arguments.  

## wp_hash_password($password)
**Description:** Hashes a password.  
**Parameters:**  
- `$password` (string) Password to hash.  

## wp_check_password($password, $hash, $user_id = '')
**Description:** Checks the password against the hashed password.  
**Parameters:**  
- `$password` (string) Plaintext password.  
- `$hash` (string) Hashed password.  
- `$user_id` (int|string) Optional. User ID. Default ''.  

## wp_salt($scheme = 'auth')
**Description:** Retrieves salt for the specified scheme.  
**Parameters:**  
- `$scheme` (string) Optional. Authentication scheme. Default 'auth'.  

## wp_generate_password($length = 12, $special_chars = true, $extra_special_chars = false)
**Description:** Generates a random password.  
**Parameters:**  
- `$length` (int) Optional. Length of the password. Default 12.  
- `$special_chars` (bool) Optional. Whether to include standard special characters. Default true.  
- `$extra_special_chars` (bool) Optional. Whether to include extra special characters. Default false.  

## wp_validate_auth_cookie($cookie = '', $scheme = '')
**Description:** Validates the authentication cookie.  
**Parameters:**  
- `$cookie` (string) Optional. Authentication cookie. Default ''.  
- `$scheme` (string) Optional. Authentication scheme. Default ''.  

## wp_set_auth_cookie($user_id, $remember = false, $secure = '')
**Description:** Sets the authentication cookie.  
**Parameters:**  
- `$user_id` (int) User ID.  
- `$remember` (bool) Optional. Whether to remember the user. Default false.  
- `$secure` (bool) Optional. Whether the authentication cookie should only be sent over HTTPS. Default ''.  

## wp_clear_auth_cookie()
**Description:** Clears the authentication cookie.  
**Parameters:** None  

## wp_verify_signature($data, $signature, $secret)
**Description:** Verifies the signature for given data.  
**Parameters:**  
- `$data` (string) Data to verify.  
- `$signature` (string) Signature to check.  
- `$secret` (string) Secret key used to generate the signature.  

## wp_generate_signature($data, $secret)
**Description:** Generates a signature for given data.  
**Parameters:**  
- `$data` (string) Data to sign.  
- `$secret` (string) Secret key to use for generating the signature.  

## wp_filter_nohtml_kses($data)
**Description:** Filters content and strips all HTML tags.  
**Parameters:**  
- `$data` (string) Content to filter.  

## wp_mail($to, $subject, $message, $headers = '', $attachments = [])
**Description:** Sends an email.  
**Parameters:**  
- `$to` (string|array) Recipient email address.  
- `$subject` (string) Email subject.  
- `$message` (string) Email message.  
- `$headers` (string|array) Optional. Email headers. Default ''.  
- `$attachments` (array) Optional. Files to attach. Default empty array.  

## sanitize_email($email)
**Description:** Sanitizes an email address.  
**Parameters:**  
- `$email` (string) Email address to sanitize.  

## is_email($email)
**Description:** Verifies that an email address is valid.  
**Parameters:**  
- `$email` (string) Email address to verify.  

## wp_safe_redirect($location, $status = 302, $x_redirect_by = 'WordPress')
**Description:** Performs a safe redirect to another URL.  
**Parameters:**  
- `$location` (string) URL to redirect to.  
- `$status` (int) Optional. HTTP status code. Default 302.  
- `$x_redirect_by` (string) Optional. Application doing the redirect. Default 'WordPress'.  

## remove_all_filters($tag, $priority = false)
**Description:** Removes all of the hooks from a filter.  
**Parameters:**  
- `$tag` (string) The filter to remove hooks from.  
- `$priority` (int|false) Optional. The priority number to remove. Default false.  

## remove_all_actions($tag, $priority = false)
**Description:** Removes all of the hooks from an action.  
**Parameters:**  
- `$tag` (string) The action to remove hooks from.  
- `$priority` (int|false) Optional. The priority number to remove. Default false.  

## wp_safe_remote_get($url, $args = [])
**Description:** Performs a safe remote GET request.  
**Parameters:**  
- `$url` (string) URL to request.  
- `$args` (array) Optional. Request arguments. Default empty array.  

## wp_safe_remote_post($url, $args = [])
**Description:** Performs a safe remote POST request.  
**Parameters:**  
- `$url` (string) URL to request.  
- `$args` (array) Optional. Request arguments. Default empty array.  

### database-functions.md

# Database Functions

## $wpdb
**Description:** The WordPress database access abstraction class. Use it to interact with the WordPress database.  
**Parameters:** None  

## $wpdb->get_var($query, $x = 0, $y = 0)
**Description:** Retrieves a single variable from the database.  
**Parameters:**  
- `$query` (string) SQL query.  
- `$x` (int) Optional. Column number to retrieve from. Default 0.  
- `$y` (int) Optional. Row number to retrieve from. Default 0.  

## $wpdb->get_row($query, $output = OBJECT, $y = 0)
**Description:** Retrieves an entire row from the database.  
**Parameters:**  
- `$query` (string) SQL query.  
- `$output` (string) Optional. Output type. One of OBJECT, ARRAY_A, or ARRAY_N. Default OBJECT.  
- `$y` (int) Optional. Row number to retrieve from. Default 0.  

## $wpdb->get_col($query, $x = 0)
**Description:** Retrieves a single column from the database.  
**Parameters:**  
- `$query` (string) SQL query.  
- `$x` (int) Optional. Column number to retrieve from. Default 0.  

## $wpdb->get_results($query, $output = OBJECT)
**Description:** Retrieves an entire result set from the database.  
**Parameters:**  
- `$query` (string) SQL query.  
- `$output` (string) Optional. Output type. One of OBJECT, ARRAY_A, or ARRAY_N. Default OBJECT.  

## $wpdb->insert($table, $data, $format = null)
**Description:** Inserts a row into a table.  
**Parameters:**  
- `$table` (string) Table name.  
- `$data` (array) Data to insert (column => value).  
- `$format` (array|string) Optional. Format for each field. Default null.  

## $wpdb->update($table, $data, $where, $format = null, $where_format = null)
**Description:** Updates a row in the table.  
**Parameters:**  
- `$table` (string) Table name.  
- `$data` (array) Data to update (column => value).  
- `$where` (array) Where clause (column => value).  
- `$format` (array|string) Optional. Format for each field. Default null.  
- `$where_format` (array|string) Optional. Format for each where clause. Default null.  

## $wpdb->delete($table, $where, $where_format = null)
**Description:** Deletes a row in the table.  
**Parameters:**  
- `$table` (string) Table name.  
- `$where` (array) Where clause (column => value).  
- `$where_format` (array|string) Optional. Format for each where clause. Default null.  

## $wpdb->prepare($query, $args)
**Description:** Prepares a SQL query for safe execution.  
**Parameters:**  
- `$query` (string) SQL query with placeholders.  
- `$args` (mixed) Arguments to replace placeholders.  

## $wpdb->query($query)
**Description:** Executes a SQL query.  
**Parameters:**  
- `$query` (string) SQL query.  

## $wpdb->escape($data)
**Description:** Escapes data for use in a SQL query.  
**Parameters:**  
- `$data` (string) Data to escape.  

## $wpdb->esc_like($text)
**Description:** Escapes text for use in a LIKE query.  
**Parameters:**  
- `$text` (string) Text to escape.  

## $wpdb->insert_id
**Description:** The ID generated for an AUTO_INCREMENT column by the previous query (usually INSERT).  
**Parameters:** None  

## $wpdb->prefix
**Description:** The table prefix for the WordPress tables in the database.  
**Parameters:** None  

## $wpdb->show_errors($show = true)
**Description:** Enables or disables showing of database errors.  
**Parameters:**  
- `$show` (bool) Optional. Whether to show errors. Default true.  

## $wpdb->hide_errors()
**Description:** Disables showing of database errors.  
**Parameters:** None  

## $wpdb->print_error()
**Description:** Prints the last database error.  
**Parameters:** None  

## $wpdb->last_error
**Description:** The last database error encountered.  
**Parameters:** None  

## $wpdb->last_query
**Description:** The last SQL query executed.  
**Parameters:** None  

## $wpdb->last_result
**Description:** The result set of the last query executed.  
**Parameters:** None  

### api-functions.md

# API Functions

## register_rest_route($namespace, $route, $args = [])
**Description:** Registers a REST API route.  
**Parameters:**  
- `$namespace` (string) The namespace for the REST route.  
- `$route` (string) The REST route.  
- `$args` (array) Optional. Arguments for the REST route registration. Default empty array.  

## rest_url($path = '')
**Description:** Retrieves the URL to the REST API endpoint.  
**Parameters:**  
- `$path` (string) Optional. Path relative to the REST API endpoint. Default ''.  

## rest_ensure_response($response)
**Description:** Ensures a REST API response is a response object (instance of WP_REST_Response).  
**Parameters:**  
- `$response` (mixed) The response to ensure.  

## is_wp_error($thing)
**Description:** Checks if a variable is a WP_Error object.  
**Parameters:**  
- `$thing` (mixed) The variable to check.  

## wp_send_json($response)
**Description:** Sends a JSON response back to an AJAX request.  
**Parameters:**  
- `$response` (mixed) The data to send as JSON.  

## wp_remote_get($url, $args = [])
**Description:** Performs an HTTP GET request using the WordPress HTTP API.  
**Parameters:**  
- `$url` (string) The URL for the request.  
- `$args` (array) Optional. Arguments for the request. Default empty array.  

## wp_remote_post($url, $args = [])
**Description:** Performs an HTTP POST request using the WordPress HTTP API.  
**Parameters:**  
- `$url` (string) The URL for the request.  
- `$args` (array) Optional. Arguments for the request. Default empty array.  

## wp_remote_request($url, $args = [])
**Description:** Performs an HTTP request using the WordPress HTTP API.  
**Parameters:**  
- `$url` (string) The URL for the request.  
- `$args` (array) Optional. Arguments for the request. Default empty array.  

## wp_remote_retrieve_body($response)
**Description:** Retrieves the body content from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_response_code($response)
**Description:** Retrieves the response code from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_response_message($response)
**Description:** Retrieves the response message from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_headers($response)
**Description:** Retrieves headers from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_cookies($response)
**Description:** Retrieves cookies from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_body_as_json($response)
**Description:** Retrieves the body content from a WP_Http_Response object as JSON.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_auth_response($response)
**Description:** Retrieves the authentication response from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_sslcertificates($response)
**Description:** Retrieves SSL certificates from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## wp_remote_retrieve_parsed_response($response)
**Description:** Retrieves the parsed response from a WP_Http_Response object.  
**Parameters:**  
- `$response` (WP_Http_Response|array) The HTTP response object or array.  

## Contribution
Feel free to contribute by adding new functions or improving existing ones. Please follow the contribution guidelines in `CONTRIBUTING.md`.
