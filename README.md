# VetzPetz Email Signature Generator

A simple internal tool for generating consistent, email-client-safe signatures across Gmail, Apple Mail, and Outlook.

## Features

- **Single HTML file** — no frameworks, no dependencies, no build step
- **Three copy buttons** — one for each email client (Gmail, Apple Mail, Outlook)
- **Region-based branding** — automatically sets the correct logo, banner, website, and social links for AU, UK, TH, and Global
- **Email-client safe** — table-based layout with inline CSS, tested across Gmail, Apple Mail, and Outlook (Windows)
- **Step-by-step instructions** — shown per email client after clicking copy

## Usage

1. Open `index.html` in your browser
2. Fill in your details (name, job title, email prefix, phone, region)
3. Click **Generate Signature**
4. Click the copy button for your email client
5. Follow the on-screen instructions to paste into your email settings

## Supported Email Clients

| Client | Version |
|--------|---------|
| Gmail | Web |
| Apple Mail | macOS / iOS |
| Outlook | Windows desktop |

## Regions

| Region | Website | Image Directory |
|--------|---------|-----------------|
| Australia (AU) | vetzpetz.com.au | au |
| United Kingdom (UK) | antinol.co.uk | uk |
| Thailand (TH) | vetzpetz.co.th | th |
| Global (GL) | vetzpetz.com | global |

## File Structure

```
VP-email-sig/
├── index.html          # The signature generator (all-in-one)
├── images/
│   ├── logo.png        # VetzPetz logo
│   ├── tagline.png     # "Keep happiness in motion" tagline
│   ├── banner.gif      # Promotional banner
│   ├── icon-email.png  # Email icon
│   ├── icon-phone.png  # Phone icon
│   ├── icon-facebook.png
│   ├── icon-instagram.png
│   └── icon-web.png    # Website icon
└── README.md
```

## Notes

- Local images are used for the preview; remote CDN URLs are used in the copied signature
- The Outlook version uses a stricter table layout with fixed widths for compatibility
- Apple Mail users must uncheck "Always match my default message font" in signature settings
