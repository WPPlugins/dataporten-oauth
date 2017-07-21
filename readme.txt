=== Plugin Name ===
Contributors: kasperrt
Tags: authentication,oauth,dataporten,oauth2.0,uninett
Requires at least: 4.0
Tested up to: 4.6
Stable tag: 3.1
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Authentication plugin for oAuth2.0 with UNINETTS Dataporten.

== Description ==

This plugin enables login with Dataporten, UNINETTS oAuth2.0 platform. The plugin works both with and without Docker. When used with docker, environment variables for client_id, client_secret, redirect_uri and much more can be used.

The plugin enables new and existing users on a wordpress blog to be automaticly assigned to a role, fetched from an array of defined roles decided from user-groups on Dataporten.

This plugin needs php curl to work!

== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/dataporten-oauth` directory, or install the plugin through the WordPress plugins screen directly.
2. Activate the plugin through the 'Plugins' screen in WordPress
3. Use the Settings->Plugin Name screen to configure the plugin

= Quick Start =

1. Download and install the dataporten-oauth plugin.
2. Setup the oAuth2.0 settings in *Settings > Dataporten-oAuth*.
3. Enable the plugin with *Settings > Dataporten-oAuth > Enabled*


== Frequently Asked Questions ==

= Is it easy to change from Dataporten to any other system? =

Yes, probably.

= Am I allowed to change the plugin to fit my needs? =

Yes.

== Changelog ==

= 3.1 =
* Folders.. folders everywhere...

= 2.7 =
* Forgot to update versions everywhere

= 2.6 =
* Logging in now updates name and email if they don't match.

= 2.5 =
* Autoclicking dataporten-login button when default form is hidden.

= 2.4 =
* Testing done, and seems to be working

= 2.3 =
* Minor Versioning

= 2.2 =
* Fixed issue where email was mistaken as password

= 2.1 =
* Added some debugging

= 2.0 =
* Fixed better handling for varying scopes from dataporten, and added firstname + lastname in database from dataporten.

= 1.8 =
* Fix for http/https

= 1.7 =
* Versioning..

= 1.6 = 
* Fixing minor versions

= 1.4 =
* Added option for enabling registering with dataporten even when user-registering is disabled.

= 1.3 =
* Hiding login button if comments are closed.

= 1.2 =
* Added Tag

= 1.1 =
* Fixed error with nonce not being added in comments

= 1.0 =
* Added nonces to comment form

= 0.9 =
* Removed login-button from comment-form if user is logged in

= 0.8 =
* Fixed upadte issue

= 0.5 =
* Removed all use of sessions
* Fixed errors showing up in DEBUG_MODE

= 0.4 =
* Added nonce to links to prevent CSRF
* Removing old states once every day, and checking whether the states are older than 10 minutes. If it is older than 10 minutes, the login is discarded.

= 0.3 =
* Security update
* States are now added to database, with an url. This can be extracted so we don't have to rely on sessions for previous urls.

= 0.2 =
* Bug fixes
* Redirecting works better now.
