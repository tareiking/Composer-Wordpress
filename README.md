## TK-COMPOSER-WP
==============

1. Removed rmccue/requests and wp-cli from dependency list
2. Added roots/roots repo to dependency list

### Important

In order for roots theme to work, you may have to edit 'WP_CONTENT_DIR' found in wp-config to add the path of your app.
Example:

 <code>
	define( 'WP_CONTENT_URL', 'http://' . $_SERVER['HTTP_HOST'] . '/tk-composer-wp/app' );
 </code>

Was changed from:

<code>
	define( 'WP_CONTENT_URL', 'http://' . $_SERVER['HTTP_HOST'] . '/app' );
</code>


### Thanks to

1. kalenjohnson/Composer-Wordpress
2. Scott Walkinshaw's "Using Composer with Wordpress" post http://roots.io/using-composer-with-wordpress/