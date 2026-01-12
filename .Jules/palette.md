## 2024-07-29 - Data-Driven UI is Maintainable UI
**Learning:** Hardcoded UI elements, especially lists and menus, become a significant maintenance burden over time. Seemingly small text changes require a full recompile, and localization becomes a nightmare of scattered strings. A data-driven approach, where UI content is loaded from external files (like `.txt` or `.json`), is almost always a superior long-term solution.

**Action:** Before hardcoding a list of items in UI code, I will always ask: "Could this ever change? Does this need to be translated?" If the answer is yes, I'll advocate for moving the content to a configuration or translation file, even for seemingly small lists. This keeps the UI flexible and easy to update without developer intervention.
