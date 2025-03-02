=== Prizm Image ===
Plugin Name: Prizm Image
Version: 2.4.3
Author: Accusoft
Contributors: Accusoft
Author URI: http://www.accusoft.com
Tags: images, image, attachments, attachment, jpeg, png, Prizm Image, smushit, performance
Requires at least: 3.5
Tested up to: 4.3.1
Stable tag: 2.4.3
License: MIT
License URI: https://raw.githubusercontent.com/edocr/edocr-document-viewer/master/LICENSE

The Prizm Image plugin lets you reduce the file size of your images by up to 70% while maintaining resolution and visual quality.


== Description ==

Google (and many other web experts) recommend optimizing web images to [improve website performance](https://developers.google.com/speed/docs/best-practices/payload#CompressImages).  Google has even gone so far as to include web [site speed as part of their search ranking](http://googlewebmastercentral.blogspot.com/2010/04/using-site-speed-in-web-search-ranking.html) algorithm.

The Prizm Image plugin helps to achieve web site performance by optimizing images while maintaining resolution and visual quality.  Compare our output to the popular Smush.It Plugin and you will see significant reduction in image sizes.  Also, Prizm Image has no size limit on the files that can submitted for reduction.

This plugin utilizes the [Accusoft Services Compress API](https://www.accusoft.com/products/accusoft-services/compression-api/) to optimize images for a WordPress website. It provides customizable options to do the following:

* Optimize JPEG compression
* Strip metadata from all JPEGs (except for copyrights)
* Convert between Progressive JPEGs and Sequential JPEGs
* Optimize PNGs
* Optimze GIFs

= User Registration =

You will need to [register for an Accusoft Services account](https://www.accusoft.com/portal#create-account) in order to obtain a free License Key to use the plugin. This is a free account for use up to 1000 compressed images per month. Plans start as low as $5 per month for additional image compressions.

= How does it work? =

There are three ways you can optimize images using your customized settings:

* Automatically on upload: Automatically optimize every image you add to the Media Library (unless you disable the Use Prizm Image on upload option in Settings > Media).
* Individually: Run existing images through the Prizm Image plugin. In the WordPress Media Library, click the Run Prizm Image link for any image you'd like to optimize.
* By Bulk: Optimize all images in the Media Library. In the Media > Bulk Prizm Image tab, click the Run all my images through Prizm Image right now button. Or, on the Media Library page, choose Bulk Prizm Image from the Bulk Actions drop down menu

= Configuration Settings =

Configure the plugin options in the Settings > Media tab as follows:

* Prizm Image License Key
  * Enter the License Key you have obtained by [registering Prizm Image](https://www.accusoft.com/portal#create-account)
* Select quality of reduced images
  * Lower Quality - Smaller File Size
  * Balanced Quality and File Size (default)
  * Higher Quality - Larger File Size
* Remove JPEG metadata
  * Select to remove JPEG metadata (except for copyright data) (default)
  * Deselect to preserve all metadata
* Select JPEG Mode
  * Convert Sequential JPEGs to Progressive JPEGs
  * Convert Progressive JPEGs to Sequential JPEGs
  * Do not change the JPEG mode (default)
* Use Prizm Image on upload?
  * Automatically process on upload (default)
  * Do not process on upload
* How many seconds should we wait for a response from Prizm Image?
  * Specify the number of seconds to wait (120 seconds is the default setting)
* Enable debug processing
  * Select to display additional troubleshooting information
  * Deselect to not display additional troubleshooting information (default)

= Restrictions =

Prizm Image does not accept filenames that contain the character '+'.
If a file with a filename containing '+' is attempted to be reduced, then an error will be returned.

== Screenshots ==

1. See how much Prizm Image reduced your file sizes in the Media Library.
2. Customize your configuration settings in Media Settings.
3. Run all of the existing images in your Media Library through Prizm Image in Bulk Prizm Image.


== Installation ==

1. Upload the Prizm Image plugin to your /wp-content/plugins/ directory.
2. Activate the plugin through the Plugins menu in WordPress.
3. Obtain and configure your License Key.
4. Set automatic optimization options in Settings > Media.


== Changelog ==
= 2.4.3 =
*Changed license from GPLv3 to MIT

= 2.4 =
* JPEG files that had a file extension of ".jpeg" were not identified as file types that the plugin could process.  Fixed so that these files are processed.

= 2.3 =
* Provided fix for feature in Chrome browser in which going back to previous screen did not refresh the previous screen.

= 2.2 =
* Added support for reducing GIF files
* Added a running total of the number of bytes saved
* Improved efficiency by ensuring that unsupported file types are not sent to the Prizm Image service

= 2.1 =
* Fix checking of License Key

= 2.0 =
* Updated to use improved and faster Prizm Image API.
* Requires user to register for a License Key in order to use the plugin.

= 1.0 =
* First edition


== About Us ==
[Accusoft](http://www.Accusoft.com) provides a full spectrum of document, content and imaging solutions.


== Contact and Credits ==

Prizm Image includes a copy of the [PEAR JSON library](http://pear.php.net/pepr/pepr-proposal-show.php?id=198) written by Michal Migurski.

The Prizm Image Wordpress plugin (not the image compression) was based upon the [WP Smush.it plugin](http://wordpress.org/plugins/wp-smushit/).
