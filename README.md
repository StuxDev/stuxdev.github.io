<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.dev/logo-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.dev/logo-dark.png"><img src="https://global.media.stux.dev/logo-dark.png" height="100" alt="Stux.Dev Logo"></picture>
</p>

# Stux.Dev GitHub Pages Redirect

A simple template for redirecting your GitHub Pages site (username.github.io) to your custom domain.

## Features

- ✨ Lightweight and fast redirect solution
- 🎯 Easy to set up in minutes
- 📱 Works on all devices and browsers

## Quick Start

1. **Fork or use this template** to create a new repository named `username.github.io`
2. **Update the domain** in the HTML file:
   - Replace `example.com` with your actual domain
3. **Enable GitHub Pages** in your repository settings
4. **Visit** `https://username.github.io` to test the redirect

## How It Works

This template uses a simple HTML meta refresh to redirect visitors from your GitHub Pages URL to your custom domain. The redirect happens automatically when users visit your `username.github.io` page.

## Installation

### Option 1: Using as a Template
1. Click **"Use this template"** on the GitHub repository page
2. Name your repository `username.github.io` (replace `username` with your GitHub username)
3. Customize the domain in `index.html`

### Option 2: Manual Setup
1. Create a new repository named `username.github.io`
2. Copy the contents of this template to your repository
3. Update the redirect URL in `index.html`
4. Push to GitHub

## Configuration

Edit these two lines in `index.html` (this repository's copy sends `stuxdev.github.io` to Stux.Dev's GitHub profile):
```html
<meta http-equiv="refresh" content="0;url=https://github.com/StuxDev" />
<link rel="canonical" href="https://github.com/StuxDev" />
```

Replace `https://github.com/StuxDev` with your actual domain. Every visitor lands on that one URL; the path they asked for isn't carried over.

## Troubleshooting

- **Redirect not working?** Ensure your repository is named exactly `username.github.io` and GitHub Pages is enabled
- **Need to change the redirect delay?** Modify the `content="0;url=..."` value (0 = immediate)
- **Want to customize the loading page?** Edit the HTML content before the meta redirect tag

## Versioning

This project uses [Date Versioning](https://datevers.ing): each release is numbered by its UTC release date as `YY.MM.DD` (for example `26.10.23`), with `-1`, `-2`… for later releases the same day. See [CHANGELOG.md](CHANGELOG.md) for what changed in each release.

Work happens on the `test` branch, and changes reach `main` only through a pull request from `test`. Release commits and tags are made on `test` (`git push origin test --tags`) and go live when that pull request is merged.

## License

Feel free to use this template for your own projects! Copyright © 2026 Stux.Group.

## Support

Have questions? Check the [GitHub Pages documentation](https://pages.github.com/) or open an issue in this repository.

---

*Built & Maintained by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.dev/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.dev/icon-dark.png"><img src="https://global.media.stux.dev/icon-dark.png" height="14" alt="Stux.Dev" valign="middle"></picture> [Stux.Dev](https://github.com/StuxDev).  
Stux.Dev is a part of the <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.group/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.group/icon-dark.png"><img src="https://global.media.stux.group/icon-dark.png" height="14" alt="Stux.Group" valign="middle"></picture> Stux.Group Brand of Companies.*
