=== WooCommerce My Licences ===
Contributors:      sebsstudio, sebd86
Donate link:       http://www.sebastiendumont.com/donation/
Tags:              woocommerce, licence, software, api
Requires at least: 4.0
Tested up to:      4.2.2
Stable tag:        1.0.1
License:           GPLv2 or later
License URI:       http://www.gnu.org/licenses/gpl-2.0.html

WooCommerce My Licences is a simple shortcode plugin that allows you to display the end-users licence keys in a table.

== Description ==
> <strong>Required to Work</strong><br>
> This plugin requires the use of [WooCommerce Software Add-on](http://www.woothemes.com/products/software-add-on/)

WooCommerce My Licences is a simple shortcode plugin that allows you to display the end-users licence keys in a table.

With WooCommerce Software Add-on, each software product the customer has purchased, a licence key is given but only via email when the order is completed. You also don't have the option to deactivate your licence key. With this plugin, not only does the customer see all licence keys purchased but also lists which site or instant the licence has be activated on.

To use this shortcode, simply place the shortcode on page and any software your customers have purchased will have access to the licence keys once logged in on their account.

= Features =
 * Table listing all product licence keys. [ Product Name | Licence Key | Software Version | Activations | Licence Type ]
 * Each licence key will list activated sites or instants along with a deactivation button.
 * See how many activations the licence key has left.

= Contributing and reporting bugs =
You can contribute code to this plugin via GitHub: https://github.com/Sebs-Studio/WooCommerce-My-Licences and localizations via Transifex: https://www.transifex.com/projects/p/woocommerce-my-licences/

= Support =
Use the WordPress.org forums for [community support](https://wordpress.org/support/plugin/woocommerce-my-licences). If you spot a bug, you can of course log it on [Github](https://github.com/Sebs-Studio/WooCommerce-My-Licences/issues) instead where I can act upon it more efficiently.

If you need help with customization. Please consider [hiring me](http://www.sebastiendumont.com/hire-me/) to apply your website's customizations for this plugin.

Please also consider making a [donation](http://www.sebastiendumont.com/donation/) or [write a review](https://wordpress.org/support/view/plugin-reviews/woocommerce-my-licences?rate=5#postform).

**More information**

- Other [WordPress plugins](http://profiles.wordpress.org/sebsstudio/) by [Sebs Studio](http://www.sebs-studio.com/)
- Contact Sebastien on Twitter: [@sebsstudio](http://twitter.com/sebsstudio)
- If you're a developer yourself, follow or contribute to the [WooCommerce My Licences plugin on GitHub](https://github.com/Sebs-Studio/WooCommerce-My-Licences)

== Installation ==
Installing "WooCommerce My Licences" can be done either by searching for "WooCommerce My Licences" via the "Plugins > Add New" screen in your WordPress dashboard, or by using the following steps:

1. Download the plugin via WordPress.org
2. Upload the ZIP file through the 'Plugins > Add New > Upload' screen in your WordPress dashboard.
3. Activate the plugin through the 'Plugins' menu in WordPress.
4. Either create a new page or edit a previous one and insert the shortcode `[woocommerce_my_licences]`

== Frequently Asked Questions ==

= Q.1 How do I display the licence table? =

A.1 Simply place this shortcode anywhere you want.

`[woocommerce_my_licences]`

= Q.2 How can I display a products variation column? =

A.2 Simply display the shortcode like so.

`[woocommerce_my_licences variables="yes"]`

= Q.3 Do you have any action hooks I can use? =

A.3 Yes there are a few action hooks in place that can be used to display content before and after the licence table.

`add_action( 'woocommerce_before_my_licences', 'your_function_name' );`

`add_action( 'woocommerce_after_my_licences', 'your_function_name' );`

= Q.4 What about filters? =

A.4 There is a filter for displaying the variable type.

`apply_filters( 'wc_my_licences_type', $type )`

== Changelog ==

= 1.0.1 : 15th June 2015 =
* Improved the ability to enable the variable product column in the licence table.
* Removed commented out code that is not used.
* Removed closing PHP tags at the end of the files.
* Removed superglobal $GLOBALS directly in the main plugin file.
* Updated the text-domain name.
* Updated the name of the plugin class.
* Updated the README.md and readme.txt files.

= 1.0.0 : 15th April 2015 =
* Initial version

== Upgrade Notice ==
= 1.0.1 : 15th June 2015 =
* Security fixes, improvments and code clean-up.
