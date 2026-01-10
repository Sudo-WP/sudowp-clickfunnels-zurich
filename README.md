# Zurich for ClickFunnels (SudoWP Edition) 🛡️

![Status](https://img.shields.io/badge/Status-Maintained-green) ![Security](https://img.shields.io/badge/Security-Patched-blue)

> **⚠️ IMPORTANT NOTICE:**
> This is an **unofficial fork** of the original "ClickFunnels" plugin (v3.1.1).
> This repository is maintained by **SudoWP** solely for the purpose of keeping the plugin secure and compatible with modern WordPress versions.
>
> We are **NOT** affiliated with, endorsed by, or connected to **ClickFunnels / Etison, LLC**.
> If you are a current ClickFunnels user looking for the legacy integration, use this patched version at your own risk.

## ℹ️ Why this fork exists?
The original plugin appears to be deprecated/abandoned in the WordPress repository, yet it contained a critical Stored XSS vulnerability (CVE-2022-4782).
**SudoWP** created this fork ("Zurich") to provide a secure alternative for existing users.

### Key Patches
* ✅ **Security:** Fixed Stored Cross-Site Scripting (XSS) vulnerability.
* ✅ **Hardening:** Implemented strict sanitization (`sanitize_text_field`) and output escaping on all shortcodes.
* ✅ **Compatibility:** Fixed PHP deprecation notices.

## 🚀 Installation
Since this plugin is not on the official repository, you must install it manually:

1.  Download the latest `.zip` from the **[Releases](../../releases)** page.
2.  Go to your **WordPress Dashboard -> Plugins -> Add New -> Upload Plugin**.
3.  Upload the zip file and Activate.
4.  Navigate to the **ClickFunnels** menu to configure your API key.

## 📝 Changelog

### [v0.1.1 - Zurich Edition]
* **SECURITY:** Patched Stored XSS in shortcodes (CVE-2022-4782).
* **HARDENING:** Added `esc_url`, `esc_js`, and `esc_attr` to all output functions.
* **REBRAND:** Updated plugin metadata to prevent conflicts with the original abandoned version.

---
*Original code is licensed under GPLv2 or later.*