# Catalyst Alpha

A three-page static website presenting the Catalyst Alpha crypto research concept. It provides a landing page, strategy descriptions, and a methodology page in plain HTML and CSS, with links to an external Telegram channel.

This repository contains the presentation website only. It does not include market data ingestion, signal generation, backtesting, portfolio management, or trading execution. Statements in the page copy about research validation, monitoring, and trading performance are not demonstrated by code or results in this repository.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | Landing page, strategy cards, and calls to action |
| `strategy.html` | Descriptions of token unlock, funding rate, and airdrop/TGE strategies |
| `about.html` | Methodology, research process, and infrastructure descriptions |
| `style.css` | Shared colors, typography, cards, navigation, and responsive layout |

Each HTML page includes its own navigation and footer. A small inline JavaScript handler toggles the mobile menu. The shared stylesheet uses CSS variables, Grid, Flexbox, and a mobile breakpoint at 640 pixels.

## View locally

Download or clone the repository, keep the four files together, and open `index.html` in a modern browser. Follow the navigation to the other pages. No package installation, build step, environment variables, or application server is required.

JavaScript must be enabled for the collapsed mobile navigation. Inter and JetBrains Mono are loaded from Google Fonts; internet access is required for those fonts and the external Telegram destination. The stylesheet supplies fallback fonts.

## Editing and checking

Edit page content directly in the HTML files and shared presentation rules in `style.css`. Navigation and footer changes need to be applied to all three pages.

There is no test runner, package manifest, or repository-defined CI workflow. Suggested manual checks, not a verified test suite:

- Open all three pages and check internal navigation.
- Resize below 640 pixels and test opening and closing the mobile menu.
- Check keyboard navigation, text wrapping, and font fallback behavior.
- Review external destinations and substantiate or revise research claims before publishing changed content.

The files can be served by a static web host without compilation. Hosting configuration is outside this source tree.

## Attribution and license

The site carries a “© 2026 Catalyst Alpha. All rights reserved.” notice. No license file or open-source license grant is included. Google Fonts supplies the external typefaces. References to *Advances in Financial Machine Learning* describe the site's research narrative; no implementation of that framework is bundled here.
