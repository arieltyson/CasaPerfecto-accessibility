# CasaPerfecto Accessibility Statement

Updated 9 October 2026.

CasaPerfecto aims to conform to the Web Content Accessibility Guidelines (WCAG) 2.2 at Level AA. This statement describes what is supported, how it is checked, and what is still open.

## What is supported

| Feature | Support |
| --- | --- |
| Screen readers | Semantic headings, landmarks and labelled controls. The map is one labelled image with a text summary; the **Areas** tab holds the same information as a sortable table. Recalculated results are announced. |
| Keyboard | Every control is reachable by keyboard. Tabs follow the WAI-ARIA tabs pattern (arrow keys, Home and End). Map picking has keyboard alternatives: intersection search and the default workplace. |
| Voice control | Buttons and inputs use visible text that matches their accessible names. |
| Larger text and zoom | Type is set in rem, so it follows your browser's text size. Layouts reflow at 320 CSS pixels without horizontal scrolling. |
| Dark interface | Follows your system setting, with a manual override in **Settings**. |
| Color | Every color carries meaning with a second carrier: numbers in each legend step, text labels, dashed outlines for danger zones, and glyphs on status badges. Map scales change in brightness within one hue, so they stay ordered for color-blind readers and in grayscale. |
| Contrast | All text is at least 4.5:1 in every appearance (lowest 5.09:1). A high-contrast palette is used when your system asks for more contrast. |
| Reduced motion | Map camera moves and transitions are removed when your system asks for reduced motion. |
| Captions and audio descriptions | Not applicable. The site has no audio or video. |

## How it is checked

- Automated: every deploy runs axe-core against the WCAG 2.0, 2.1 and 2.2 A and AA rules on the welcome screen, each onboarding step and every dashboard tab, in light and dark appearances, at desktop and phone sizes. Any violation blocks the deploy.
- Automated: unit tests compute WCAG contrast for every color pair and check that map scales stay ordered under simulated protanopia, deuteranopia and tritanopia.
- Automated: tests check keyboard tab navigation, reflow at 320 pixels and the map's text summary.
- Manual testing with screen readers is listed under known issues until it is complete.

## Technology

The site relies on HTML, CSS, JavaScript and WebGL. Without WebGL the map is replaced by a message, and all of its information remains available in the **Areas** tab.

## Feedback

Open an issue at [github.com/arieltyson/CasaPerfecto-accessibility/issues](https://github.com/arieltyson/CasaPerfecto-accessibility/issues). Known limitations are listed on the [known issues](known-issues/) page.
