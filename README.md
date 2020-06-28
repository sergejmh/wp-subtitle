### WP Subtitle

Add subtitles (subheadings) to your pages, posts or custom post types.

The WP Subtitle plugin allows your pages and posts to contain a subtitle.  Also called a sub-heading, this this short line of text is meant to appear beneath a post's (or page's) title, but can be inserted in your template wherever you choose.

The subtitle can be inserted into your theme template files (or plugin) using the following API:

### Display The Subtitle

All parameters are optional. If 'post_id' is omitted then the current post ID in the loop is used.

PHP Code:

```
do_action( 'plugins/wp_subtitle/the_subtitle', array(
    'before'        => '<p class="subtitle">',
    'after'         => '</p>',
    'post_id'       => get_the_ID(),
    'default_value' => ''
) );
```

Output:

`<p class="subtitle">My Post Subtitle</p>`
