# 📨 WordPress HTML Email Template

This repository contains a clean, responsive, and fully compatible **HTML email template** designed for use in **WordPress-based websites**. It's ideal for customizing:

- 🔔 Transactional emails (new comment, password reset, user registration)
- 📬 Newsletters or content updates
- 🛒 WooCommerce order notifications
- 🧩 Plugin-generated emails (e.g., form submissions, bookings)

## 🌐 Why Use This?

WordPress core and many plugins generate HTML emails with limited styling. This template gives you:

- Better branding control
- Responsive layout
- Clean, readable typography
- Cross-client consistency

## 🗂️ Files Included

- `wp-email-template.html` – The core email layout
- `preview.png` – Screenshot of the rendered email
- `images/` – Optional images or logos
- `README.md` – This documentation

## 🖼️ Preview

![Email Screenshot](preview.png)

Open `wp-email-template.html` in a browser or email builder to preview the full layout.

## 📦 Features

- ✅ WordPress-compatible structure
- ✅ Inline CSS for maximum email client support
- ✅ Table-based layout (Outlook-friendly)
- ✅ Customizable header, body, footer
- ✅ Button styles for CTAs

## ⚙️ How to Use

### Option 1: With a Plugin (Recommended)
Use plugins like:

- [WP Mail SMTP](https://wordpress.org/plugins/wp-mail-smtp/)
- [Kadence WooCommerce Email Designer](https://wordpress.org/plugins/kadence-woocommerce-email-designer/)
- [Email Templates](https://wordpress.org/plugins/email-templates/)

Paste the HTML from `wp-email-template.html` into the plugin's email editor.

### Option 2: Hardcode in a Theme/Plugin
In your PHP email function:
```php
$message = file_get_contents( get_template_directory() . '/emails/wp-email-template.html' );
wp_mail( $to, $subject, $message, $headers );
