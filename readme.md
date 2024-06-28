# WordPress Most Used Functions

## Introduction
This repository contains a collection of the most frequently used WordPress functions, filters, and actions, organized by category for easy reference.

## How to Use
Browse the categories to find the functions you need. Each category contains a set of functions with descriptions, usage examples, and best practices.
| Function Name                | Description                                                                                     | Parameters                           |
|------------------------------|-------------------------------------------------------------------------------------------------|--------------------------------------|
| **General Functions**        |                                                                                                 |                                      |
| `wp_enqueue_script()`        | Enqueues a script.                                                                              | `$handle` (string), `$src` (string), `$deps` (array), `$ver` (string|bool|null), `$in_footer` (bool) |
| `wp_enqueue_style()`         | Enqueues a stylesheet.                                                                          | `$handle` (string), `$src` (string), `$deps` (array), `$ver` (string|bool|null), `$media` (string) |
| `get_template_part()`        | Loads a template part into a template.                                                          | `$slug` (string), `$name` (string|null) |
| `get_header()`               | Loads the header template.                                                                      | None                                 |
| `get_footer()`               | Loads the footer template.                                                                      | None                                 |
| `wp_redirect()`              | Redirects to another page or URL.                                                               | `$location` (string), `$status` (int) |
| `esc_html()`                 | Escapes text for HTML output.                                                                   | `$text` (string)                     |
| `esc_attr()`                 | Escapes text for use in an HTML attribute.                                                      | `$text` (string)                     |
| `esc_url()`                  | Escapes a URL for use in HTML attributes or redirects.                                          | `$url` (string)                      |
| `current_time()`             | Retrieves the current time based on specified type.                                              | `$type` (string), `$gmt` (bool)      |
| **Sanitization Functions**   |                                                                                                 |                                      |
| `esc_html()`                 | Escapes HTML for safe output.                                                                    | `$text` (string)                     |
| `esc_attr()`                 | Escapes an attribute value for safe output.                                                      | `$text` (string)                     |
| `esc_url()`                  | Escapes a URL for safe output.                                                                   | `$url` (string)                      |
| `esc_textarea()`             | Escapes a textarea string for safe output.                                                       | `$text` (string)                     |
| `sanitize_text_field()`      | Sanitizes a string from user input or from the database.                                          | `$str` (string)                      |
| `sanitize_email()`           | Sanitizes an email address.                                                                      | `$email` (string)                    |
| `sanitize_file_name()`       | Sanitizes a filename replacing whitespace and a few other characters with dashes.                | `$filename` (string)                 |
| `wp_kses_post()`             | Sanitizes content for allowed HTML tags for post content.                                         | `$data` (string)                     |
| `wp_filter_post_kses()`      | Sanitizes content for allowed HTML tags for post content, applying filters.                       | `$data` (string)                     |
| `wp_kses_data()`             | Sanitizes content for allowed HTML tags for general content.                                       | `$data` (string)                     |
| `wp_kses()`                  | Sanitizes content for allowed HTML tags, based on context.                                        | `$data` (string), `$allowed_html` (array) |
| **Validation Functions**     |                                                                                                 |                                      |
| `is_email()`                 | Validates an email address.                                                                     | `$email` (string)                    |
| `is_user_logged_in()`        | Checks if the current visitor is a logged-in user.                                              | None                                 |
| `is_admin()`                 | Checks if the current request is for an administrative interface page.                          | None                                 |
| `current_user_can()`         | Checks if the current user has a specific capability.                                           | `$capability` (string)               |
| `wp_verify_nonce()`          | Verifies that a nonce is correct and unexpired.                                                 | `$nonce` (string), `$action` (int|string) |
| `check_admin_referer()`      | Verifies the AJAX request to prevent processing requests external of the blog.                  | `$action` (int|string), `$query_arg` (string) |
| `check_ajax_referer()`       | Verifies the AJAX request to prevent processing requests external of the blog.                  | `$action` (int|string), `$query_arg` (false|string), `$die` (bool) |
| `current_user_can_for_blog()`| Checks if the current user has a specific capability for a given site.                          | `$blog_id` (int), `$capability` (string) |
| `has_cap()`                  | Checks if the user has a specific capability.                                                   | `$capability` (string)               |
| `validate_file()`            | Validates a file name and path for security reasons.                                             | `$file` (string), `$allowed_files` (array) |
| `wp_validate_auth_cookie()`  | Validates authentication cookies.                                                               | `$cookie` (string), `$scheme` (string) |
| `wp_validate_redirect()`     | Validates a URL for use in a redirect.                                                          | `$location` (string), `$default` (string) |
| `validate_username()`        | Validates a username.                                                                           | `$username` (string)                 |
| `is_serialized()`            | Checks if data is serialized.                                                                   | `$data` (mixed), `$strict` (bool)    |
| `is_serialized_string()`     | Checks if a string is serialized.                                                               | `$data` (string)                     |
| `is_ssl()`                   | Determines if SSL is used.                                                                      | None                                 |
| `is_multisite()`             | Determines if Multisite is enabled.                                                             | None                                 |
| `is_main_site()`             | Determines if the current site is the main site.                                                | `$site_id` (int|null)                |
| `wp_validate_boolean()`      | Validates a boolean variable.                                                                   | `$value` (mixed)                     |
| **Filters**                  |                                                                                                 |                                      |
| `the_title`                  | Filters the post title.                                                                         | `$title` (string), `$id` (int)       |
| `the_content`                | Filters the post content.                                                                       | `$content` (string)                  |
| `the_excerpt`                | Filters the post excerpt.                                                                       | `$excerpt` (string)                  |
| `wp_title`                   | Filters the text of the page title.                                                             | `$title` (string), `$sep` (string), `$seplocation` (string) |
| `wp_nav_menu_items`          | Filters the HTML list content for navigation menus.                                              | `$items` (string), `$args` (object)  |
| `wp_list_pages`              | Filters the HTML output of list pages.                                                           | `$output` (string), `$args` (array)  |
| `the_author`                 | Filters the display name of the author.                                                         | `$display_name` (string)             |
| `comment_text`               | Filters the comment text.                                                                       | `$comment_text` (string), `$comment` (WP_Comment) |
| `get_avatar`                 | Filters the avatar.                                                                             | `$avatar` (string), `$id_or_email` (mixed), `$size` (int), `$default` (string), `$alt` (string) |
| `get_search_form`            | Filters the search form HTML.                                                                   | `$form` (string)                     |
| `the_date`                   | Filters the date a post was published.                                                          | `$the_date` (string), `$d` (string), `$post` (WP_Post) |
| `the_time`                   | Filters the time a post was published.                                                          | `$the_time` (string), `$d` (string), `$post` (WP_Post) |
| `bloginfo`                   | Filters the output of blog information.                                                         | `$output` (string), `$show` (string) |
| `wp_mail_from`               | Filters the email address to send from.                                                         | `$from_email` (string)               |
| `wp_mail_from_name`          | Filters the name to associate with the "from" email address.                                     | `$from_name` (string)                |
| `pre_get_posts`              | Allows altering the main query before it is executed.                                            | `$query` (WP_Query)                  |
| `wp_get_attachment_image_src`| Filters the image src result.                                                                   | `$image` (array|false), `$attachment_id` (int), `$size` (string|array), `$icon` (bool) |
| `the_category`               | Filters the list of categories for a post.                                                      | `$thelist` (string), `$separator` (string), `$parents` (string) |
| `the_tags`                   | Filters the list of tags for a post.                                                            | `$tag_list` (string), `$before` (string), `$sep` (string), `$after` (string) |
| `excerpt_length`             | Filters the length of the excerpt.                                                              | `$length` (int)                      |
| `excerpt_more`               | Filters the "read more" excerpt string.                                                         | `$more` (string)                     |
| `upload_mimes`               | Filters the list of allowed mime types and file extensions.                                      | `$mimes` (array)                     |
| `widget_text`                | Filters the content of the text widget.                                                         | `$text` (string), `$instance` (array) |
| `wp_generate_attachment_metadata` | Filters the attachment meta data.                                                            | `$metadata` (array), `$attachment_id` (int) |
| `term_links-post_tag`        | Filters the term links for the post tags.                                                       | `$term_links` (array), `$taxonomy` (string) |
| **Actions**                  |                                                                                                 |                                      |
| `init`                       | Fires after WordPress has finished loading but before any headers are sent.                      | None                                 |
| `wp_enqueue_scripts`         | Fires when scripts and styles are enqueued.                                                      | None                                 |
| `wp_head`                    | Fires within the `<head>` section of the theme.                                                  | None                                 |
| `wp_footer`                  | Fires before the closing `</body>` tag of the theme.                                             | None                                 |
| `admin_init`                 | Fires as an admin screen or script is being initialized.                                         | None                                 |
| `admin_menu`                 | Fires before the administration menu loads in the admin.                                          | None                                 |
| `admin_notices`              | Fires after all administrative notices have been added.                                          | None                                 |
| `save_post`                  | Fires when a post or page is updated.                                                           | `$post_id` (int), `$post` (WP_Post), `$update` (bool) |
| `wp_insert_post`             | Fires once a post has been saved.                                                               | `$post_id` (int), `$post` (WP_Post), `$update` (bool) |
| `delete_post`                | Fires before a post or page is deleted.                                                         | `$post_id` (int)                     |
| `transition_post_status`     | Fires when a post's status is changed.                                                          | `$new_status` (string), `$old_status` (string), `$post` (WP_Post) |
| `wp_login`                   | Fires after a user has successfully logged in.                                                   | `$user_login` (string), `$user` (WP_User) |
| `wp_logout`                  | Fires after a user has logged out.                                                               | None                                 |
| `user_register`              | Fires after a new user has been registered.                                                      | `$user_id` (int)                     |
| `profile_update`             | Fires after a user updates their profile.                                                        | `$user_id` (int), `$old_user_data` (WP_User) |
| `delete_user`                | Fires immediately before a user is deleted.                                                      | `$user_id` (int), `$reassign` (int|null) |
| `wp_ajax_{action}`           | Used to hook into a custom AJAX action for logged-in users.                                      | None                                 |
| `wp_ajax_nopriv_{action}`    | Used to hook into a custom AJAX action for logged-out users.                                     | None                                 |
| `wp_loaded`                  | Fires once WordPress, all plugins, and the theme are fully loaded and instantiated.               | None                                 |
| `template_redirect`          | Fires before determining which template to load.                                                 | None                                 |
| `wp_before_admin_bar_render` | Fires before the admin bar is rendered.                                                          | None                                 |
| `wp_after_admin_bar_render`  | Fires after the admin bar is rendered.                                                           | None                                 |
| `comment_post`               | Fires immediately after a comment is inserted into the database.                                 | `$comment_id` (int), `$comment_approved` (int|string) |
| `edit_comment`               | Fires immediately after a comment is updated in the database.                                    | `$comment_id` (int)                  |
| `delete_comment`             | Fires immediately before a comment is deleted from the database.                                 | `$comment_id` (int)                  |
| `wp_set_comment_status`      | Fires immediately after the comment status is changed in the database.                            | `$comment_id` (int), `$comment_status` (string) |
| `widgets_init`               | Fires after all default WordPress widgets have been registered and the user has hooked into the register process. | None                                 |
| `customize_register`         | Fires when Customizer options are being registered.                                               | `$wp_customize` (WP_Customize_Manager) |
| `customize_preview_init`     | Fires when Customizer preview is initialized.                                                     | None                                 |
| `switch_theme`               | Fires before the theme is switched.                                                              | `$new_name` (string), `$new_theme` (WP_Theme) |
| `after_switch_theme`         | Fires after the theme is switched.                                                               | None                                 |
| `wp_upgrade`                 | Fires immediately after the core upgrade process is complete.                                     | `$wp_version` (string)               |
| `activated_plugin`           | Fires after a plugin has been activated.                                                         | `$plugin` (string), `$network_wide` (bool) |
| `deactivated_plugin`         | Fires after a plugin has been deactivated.                                                       | `$plugin` (string), `$network_wide` (bool) |
| `register_sidebar`           | Fires after a sidebar has been registered.                                                       | `$sidebar` (array)                   |
| `wp_create_user`             | Fires immediately after a new user is created.                                                   | `$user_id` (int), `$userdata` (array) |
| `lostpassword_post`          | Fires before the lost password form is submitted.                                                 | None                                 |
| `retrieve_password`          | Fires before a new password is retrieved.                                                        | `$user_login` (string)               |
| `password_reset`             | Fires after the user has reset their password.                                                   | `$user` (WP_User), `$new_pass` (string) |
| `import_start`               | Fires at the start of an import.                                                                | None                                 |
| `import_end`                 | Fires at the end of an import.                                                                  | None                                 |
| `wp_scheduled_delete`        | Fires when WordPress's scheduled task for deleting old trash posts runs.                         | None                                 |
| `clean_post_cache`           | Fires immediately after the post's cache is cleaned.                                             | `$post_id` (int)                     |
| `save_post_{post_type}`      | Fires when a post of a specific post type is updated.                                            | `$post_id` (int), `$post` (WP_Post), `$update` (bool) |

## Contribution
Feel free to contribute by adding new functions or improving existing ones. Please follow the contribution guidelines in `CONTRIBUTING.md`.
