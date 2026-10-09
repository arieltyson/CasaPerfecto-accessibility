# Known Issues

Gaps we know about, and how each will be addressed.

| Issue | Impact | Plan |
| --- | --- | --- |
| Manual screen reader testing (VoiceOver on iOS and macOS, NVDA on Windows, TalkBack) has not been completed. | Real-world reading order or announcements may have problems the automated checks do not catch. | Complete each common task with each screen reader and record the results here. |
| The map canvas cannot be explored by screen reader. | Blocks cannot be inspected one by one without sight. | The **Areas** tab provides the same information by neighborhood. Per-block details are available by clicking a block; a keyboard block cursor is planned. |
| Street names on the basemap are in English in both languages. | Spanish readers see English map labels. | Map labels come from OpenStreetMap; the interface itself is fully translated. |
| Intersection search uses the browser's built-in suggestion list. | Suggestion behavior differs between browsers and assistive technologies. | Replace with an accessible combobox if users report problems. |
| The Areas table scrolls sideways in the narrow panel. | At large text sizes, some columns need horizontal scrolling inside the table. | Offer a stacked layout for narrow widths. |
