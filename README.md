# Oxygen Theme Enabler #

A WordPress plugin that makes it possible to use the active WordPress theme when [Oxygen](http://oxygenbuilder.com/) is active.

This plugin adds a new setting page which can be accessed at Oxygen > Theme Enabler.

Here, you can select whether you want to use the theme or Oxygen for most of your site's pages.

![Screenshot](https://d.pr/i/7Vy1LI+ "Screenshot")

You will need to edit the following line in `plugin.php` file of the plugin and enter your if conditional:

```
return is_page( 'contact' ); // enter your if condition here. Reference: https://codex.wordpress.org/Conditional_Tags
```

Replace `is_page( 'contact' )` with the conditional depending on where you want to use the theme/Oxygen.

A few valid examples:

`is_page( array( 42, 'about-me', 'About Me And Joe' ) )`

`is_front_page()`

`is_woocommerce()`

[Reference](https://codex.wordpress.org/Conditional_Tags)

## Installation ##

1. Ensure that Oxygen is installed and active.
2. Click on the `Download ZIP` button at the right to download the plugin.
3. Go to Plugins > Add New in your WordPress admin. Click on Upload Plugin and browse for the zip file.
4. Activate the plugin.

## Changelog ##

### 1.0.2 - November 15, 2019 ###
* pages set to use the theme will now work.
* pages set to use Oxygen will not load theme assets anymore.
* URLs having `ct_builder=true` i.e., Oxygen editor have been excluded from the plugin so they load.

### 1.0.1 - November 07, 2019 ###
* Simplified the return statement

### 1.0.0 - August 06, 2018 ###
* Initial Release

## Others ##

Donate link: [https://www.paypal.me/sridharkatakam](https://www.paypal.me/sridharkatakam)
