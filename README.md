# ClickFunnels Zurich (Patched)

**Contributors:** WP Republic, Webcitizen  
**Original Authors:** Etison, LLC  
**Tags:** clickfunnels, security-patch, legacy, landing pages, funnels  
**Requires at least:** 4.3  
**Tested up to:** 6.7  
**Stable tag:** 0.1.1  
**License:** GPLv2 or later  

## ⚠️ Security Notice
This is a **community-maintained fork** of the legacy ClickFunnels Classic plugin (v3.1.1). The original plugin is deprecated and contains unpatched security vulnerabilities.

**This version patches CVE-2022-4782 (Stored XSS)** by implementing strict sanitization and output escaping on all shortcodes.

---

## Description

**ClickFunnels Zurich (Patched)** allows you to connect your legacy ClickFunnels Classic (v1) account to your WordPress site. It is designed for users who need to maintain their existing integrations without exposing their sites to security risks.

**Key Features:**
* **Security Patched:** Fixes critical XSS vulnerabilities found in the original vendor version.
* **Rebranded:** Prevents accidental auto-updates from the abandoned original plugin.
* **Connect Pages:** Show any ClickFunnels page as your WordPress Homepage or 404 page.
* **Clean URLs:** Create custom slugs (e.g., `yourblog.com/offer`) that mask your ClickFunnels pages.

## Installation

1.  Download the plugin zip file (or clone this repo).
2.  Upload to your `/wp-content/plugins/` directory.
3.  Activate the plugin through the 'Plugins' menu in WordPress.
4.  Go to the **ClickFunnels** menu in your dashboard.
5.  Enter your **Authentication Key** (found in your ClickFunnels Classic account settings) and email.

## Frequently Asked Questions

**Do I need a ClickFunnels account?** Yes. This plugin requires an active ClickFunnels Classic account.

**Does this work with ClickFunnels 2.0?** No. ClickFunnels 2.0 does not support this API integration. This plugin is strictly for maintaining legacy pages built on the Classic platform.

**Why use this instead of the official plugin?** The official plugin has been abandoned and contains a known security vulnerability (CVE-2022-4782). This fork fixes that issue while keeping the functionality intact.

## Changelog

### Version 0.1.1
* **Security Fix:** Patched Stored Cross-Site Scripting (XSS) vulnerability (CVE-2022-4782).
* **Security:** Implemented strict data sanitization (`sanitize_text_field`, `esc_url`) and output escaping (`esc_attr`, `esc_js`) for all shortcodes.
* **Optimization:** Implemented dynamic version constant to automate footer updates.

### Version 0.1.0
* Initial release as ClickFunnels Zurich (Patched).
* Rebranded to WP Republic to prevent conflict with the deprecated vendor version.
