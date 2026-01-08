=== ClickFunnels Zurich (Patched) ===

Contributors: WP Republic, Webcitizen
Plugin URI: https://github.com/makmour/clickfunnels-zurich
Author URI: https://github.com/makmour
clickfunnels, patched
Requires at least: 4.3
Tested up to: 6.9
Stable tag: 0.1.1

This is the patched version for the original WordPress Clickfunnels plugin, version <= 3.1.1 which was vulnerable under a Stored Cross-Site Scripting attack.

== Description ==
Run the ClickFunnels Zurich installation and setup as you did with the original plugin.

== Changelog ==

= Version 0.1.1 =
* Security Fix: Patched Stored Cross-Site Scripting (XSS) vulnerability (CVE-2022-4782).
* Security: Implemented strict data sanitization and output escaping for `clickfunnels_embed`, `clickfunnels_clickpop`, and `clickfunnels_clickoptin` shortcodes to prevent malicious script injection.

= Version 0.1.0 =
* Initial release as ClickFunnels Zurich (Patched).
* Rebranded to WP Republic.