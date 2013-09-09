TK-COMPOSER-WP
==============

Initially Forked from: kalenjohnson/Composer-Wordpress

1. Removed rmccue/requests and wp-cli from dependency list
2. Added roots/roots repo to dependency list

## Important

In order for roots theme to work, you may have to edit 'WP_CONTENT_DIR' found in wp-config to add the path of your app.
 Example:

 <code>
	define( 'WP_CONTENT_URL', 'http://' . $_SERVER['HTTP_HOST'] . '/tk-composer-wp/app' );

	was changed from: 

	define( 'WP_CONTENT_URL', 'http://' . $_SERVER['HTTP_HOST'] . '/app' );

 </code>


Most of this is based on Scott Walkinshaw's "Using Composer with Wordpress" post.
http://roots.io/using-composer-with-wordpress/