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

### Things TODO

1. Add WooCommerce support
2. Add Child theme support
3. Give options for activating other things
4. Show instructions on how to add composer to add plugins
5. Figure out exactly when its required to change this setting: WP_CONTENT_URL 
6. Maybe change the WP_ADMIN setting as well

### Moar automation

1. Auto-activate installed plugins
2. Auto-configure WP settings

### Thanks to

1. kalenjohnson/Composer-Wordpress
2. Scott Walkinshaw's "Using Composer with Wordpress" post http://roots.io/using-composer-with-wordpress/