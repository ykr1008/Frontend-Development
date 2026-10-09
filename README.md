# Exploring Renewable Energy — Accessible HTML Project

## Overview

This project is an accessible webpage about renewable energy, built using semantic HTML. It explores the benefits and challenges of renewable energy, includes illustrative images, and presents a data table.

The project demonstrates HTML structure, accessibility best practices, JavaScript loading behavior, and web performance optimization.

## Features

* **Semantic HTML:** Uses `header`, `nav`, `main`, `article`, `section`, `aside`, `figure`, `figcaption`, `time`, and `footer`.
* **Accessible navigation:** Includes a skip-to-main-content link and a table of contents.
* **Accessible images:** Provides meaningful alternative text for informative images and empty alternative text for decorative images.
* **Heading hierarchy:** Uses one `h1` and a logical heading structure.
* **Data table:** Includes a caption, table headers, and appropriate `scope` attributes.
* **JavaScript loading:** Demonstrates normal, `async`, and `defer` script execution.
* **Image optimization:** Uses resized WebP images to reduce image download sizes.
* **Accessibility testing:** Includes keyboard navigation and screen-reader testing.

## Technologies and Tools

* HTML5
* JavaScript
* WebP images
* Visual Studio Code
* Browser Developer Tools
* Lighthouse
* axe DevTools
* NVDA Screen Reader

## Project Structure

```text
Frontend-Development/
├── images/
│   ├── Axe devtools scan result.png
│   ├── Console outputs with timestamps.png
│   └── Heading verification.png
├── images_for_webpage/
│   ├── dec-image-optimized.webp
│   ├── hydroelectric-dam-optimized.webp
│   ├── solar-panels-optimized.webp
│   ├── wind-turbines-solar-panels-optimized.webp
│   └── windturbines-optimized.webp
├── scripts/
│   ├── async.js
│   ├── defer.js
│   └── normal.js
├── index.html
├── keyboard accessibility test.md
├── Lighthouse final run.pdf
├── Lighthouse initial run.pdf
├── NVDA screen reader result.md
├── README.md
├── scripts_explanation.md
└── why does semantic html matter.md
```

## Accessibility

The webpage was evaluated using several accessibility testing methods:

* **Heading verification:** Confirmed one `h1` and a logical heading hierarchy.
* **Keyboard navigation:** Tested whether navigation links were reachable using the keyboard and whether focus indicators were visible.
* **Skip link:** Verified that the skip-to-content link appears first in the keyboard focus order and points to the main content.
* **NVDA screen reader:** Evaluated how page landmarks, headings, links, and image alternative text were announced.
* **axe DevTools:** Ran an accessibility scan and recorded the results.

Supporting screenshots and test notes are included in the repository.

## Lighthouse Results

The final Lighthouse audit reported:

| Category       | Score |
| -------------- | ----: |
| Performance    |   100 |
| Accessibility  |   100 |
| Best Practices |   100 |
| SEO            |   100 |

The initial and final Lighthouse reports are included for comparison. Image optimization and improved navigation link spacing helped address the reported issues.

## JavaScript Execution

The `scripts` directory contains three JavaScript files demonstrating different loading behaviors:

* **`normal.js`:** Executes when the browser reaches the script and blocks HTML parsing while it downloads and executes.
* **`async.js`:** Executes as soon as it finishes downloading; execution order is not guaranteed.
* **`defer.js`:** Downloads while HTML parsing continues and executes after parsing, preserving document order among deferred scripts.

Console timestamps were used to observe and document execution order. The output and explanation are included in the repository.

## Learning Outcomes

This project provided practical experience with:

* Building webpages with semantic HTML.
* Improving accessibility through headings, landmarks, alternative text, and keyboard navigation.
* Creating structured HTML data tables.
* Understanding normal, `async`, and `defer` script loading.
* Optimizing images for web delivery.
* Testing webpages with Lighthouse, axe DevTools, and NVDA.

## Author

Created as a frontend development practice project.
