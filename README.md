# SudoWP Zurich for ClickFunnels

![PHP Version](https://img.shields.io/badge/PHP-%3E%3D%208.2-777bb4.svg)
![License](https://img.shields.io/badge/License-GPLv2%2B-blue.svg)
![Status](https://img.shields.io/badge/Status-Security%20Hardened-green.svg)

**Contributors:** SudoWP, WP Republic  
**Original Authors:** Etison, LLC  
**Tags:** clickfunnels, security-patch, legacy, landing pages, funnels, sudowp  
**Requires at least:** 4.3  
**Tested up to:** 6.7  
**Stable tag:** 0.1.1  
**License:** GPLv2 or later  

## Security Notice
This is a **community-maintained fork** of the legacy ClickFunnels Classic plugin (v3.1.1). The original plugin is deprecated and contains unpatched security vulnerabilities.

**This version patches CVE-2022-4782 (Stored XSS) and CVE-2022-47152 (CSRF)** by implementing strict sanitization, output escaping, and nonce verification.

---

## Description

**SudoWP Zurich for ClickFunnels** allows you to connect your legacy ClickFunnels Classic (v1) account to your WordPress site. It is designed for users who need to maintain their existing integrations without exposing their sites to security risks.

**Key Features:**
* **Security Patched:** Fixes critical XSS and CSRF vulnerabilities found in the original vendor version.
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

**Why use this instead of the official plugin?** The official plugin has been abandoned and contains known security vulnerabilities (CVE-2022-4782 & CVE-2022-47152). This fork fixes those issues while keeping the functionality intact.

## Changelog

### Version 0.1.2
* **Security Hardening:** Comprehensive OWASP Top 10 2021 security audit
* **Access Control:** Added capability checks to all admin pages
* **Input Validation:** Enhanced sanitization of all $_GET, $_POST, and $_SERVER inputs
* **Output Escaping:** Comprehensive output escaping with context-appropriate functions
* **Cookie Security:** Added httponly and secure flags to cookies
* **CSRF Protection:** Enhanced nonce verification across all forms
* **Documentation:** Added SECURITY_NOTES.md with detailed security information

### Version 0.1.1
* **Rebranding:** Renamed to `sudowp-clickfunnels-zurich` and standardized code prefixes.
* **Security Fix:** Patched Cross-Site Request Forgery (CSRF) vulnerability in settings (CVE-2022-47152).
* **Security Fix:** Patched Stored Cross-Site Scripting (XSS) vulnerability (CVE-2022-4782).
* **Security:** Implemented strict data sanitization (`sanitize_text_field`, `esc_url`), output escaping (`esc_attr`, `esc_js`), and nonce verification.

### Version 0.1.0
* Initial release as Zurich for ClickFunnels (SudoWP Edition).
* Rebranded to prevent conflict with the deprecated vendor version.
