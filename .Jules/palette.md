## 2024-07-22 - Fix hidden help menu item

**Learning:** The help menu, constructed in `drawKeeperHelp` within `gui_builder.cpp`, is fully data-driven from `data_free/game_config/help.txt`. If an entry in `help.txt` is missing either a `viewId` (icon) or a `title` (translation key), the entry is silently skipped and does not appear in the UI. This can make valid help content completely inaccessible to the user.

**Action:** When adding or modifying help content, always ensure that both a `viewId` and a `title` are present in `help.txt` to guarantee visibility in the help menu. I will verify this for all entries when I work on this file.
