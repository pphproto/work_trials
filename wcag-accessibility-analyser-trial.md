# Work Trial: WCAG 2.2 Accessibility Analyser Chrome Extension

**Duration:** 3–5 days (early submissions are viewed favorably)

---
© Floto Inc 2026

## What to Build

Build a Chrome extension that analyses any webpage the user is viewing and reports on its compliance with a defined subset of WCAG 2.2 (Web Content Accessibility Guidelines) success criteria. Think of it as a lightweight, in-browser accessibility linter.

## What the Tool Should Do

- Open via the browser toolbar icon and display analysis results for the currently active tab
- Run the accessibility analysis on demand — when the user opens the popup or clicks a "Run Analysis" button (not automatically in the background)
- Check for at least 8 of the following 12 WCAG 2.2 success criteria — pick the ones you find most interesting or technically approachable, and be ready to justify your choices:

| # | Criterion | Level | What to Check |
|---|-----------|-------|---------------|
| 1 | 1.1.1 Non-text Content | A | Images missing alt attributes, or with empty alt on non-decorative images |
| 2 | 1.3.1 Info and Relationships | A | Headings used out of order (e.g. h1 → h3, skipping h2); form inputs without associated labels |
| 3 | 1.4.3 Contrast (Minimum) | AA | Text elements with foreground/background contrast ratio below 4.5:1 (3:1 for large text) |
| 4 | 2.1.1 Keyboard | A | Interactive elements (buttons, links, inputs) that are not reachable via keyboard (missing tabindex or focus styles) |
| 5 | 2.4.2 Page Titled | A | Page `<title>` is missing or empty |
| 6 | 2.4.6 Headings and Labels | AA | Headings that are empty or contain only whitespace |
| 7 | 2.4.7 Focus Visible | AA | Focusable elements with `outline: none` or `outline: 0` and no alternative visible focus style |
| 8 | 3.1.1 Language of Page | A | `<html>` element missing a valid lang attribute |
| 9 | 4.1.2 Name, Role, Value | A | Buttons and links with no accessible name (no text content, no aria-label, no aria-labelledby) |
| 10 | 1.4.4 Resize Text | AA | Text set in px units that may not scale with browser font size changes |
| 11 | 2.4.4 Link Purpose | A | Links whose text is non-descriptive (e.g. "click here", "read more", "here") |
| 12 | 2.5.3 Label in Name | A | Buttons or links where the visible label text is not contained within the accessible name |

- Group results by criterion, showing a count of violations per check and a list of affected elements (e.g. a CSS selector, element type, or snippet of the element's HTML) so the user can locate them
- Show a top-level pass/fail summary: how many checks passed and how many flagged issues

## Tech Stack

- Chrome Extension Manifest V3
- Vanilla JavaScript (no build tools or bundlers required)
- You may use a UI library for the popup if you prefer, but keep it simple
- All analysis must run locally in the browser via a content script — no external API calls

## Submission

1. Push code to a GitHub repository
2. Include detailed instructions on how to run your code (deployment is optional, not required)
3. Include a `README.md` with:
   - Setup instructions
   - Which 8+ criteria you implemented and why you chose them
   - Any known limitations
4. **Record a Loom** walking through the working extension — show the popup, trigger an analysis on a real page, and narrate what's happening
5. **If you used AI tools** (Claude, Cursor, GitHub Copilot, ChatGPT, etc.), export and include your chat history so we can evaluate the prompts used to generate code

**Note:** We highly recommend using AI copilots (Claude, Cursor, GitHub Copilot, ChatGPT, etc.) to complete this trial efficiently. At Floto, coding agents are a core part of how we build — we expect you to use one. The question isn't whether you use an agent, it's how well you direct it, review its output, and take ownership of the result. If you're unable to complete the implementation, you can still submit your work. In your `README.md`, document what you attempted, what worked, what didn't, and why. We evaluate based on effort, problem-solving approach, and the progress you made — not just the final outcome.
