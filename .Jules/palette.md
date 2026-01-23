## 2024-05-23 - Make Invisible UI Visible

**Learning:** I discovered that the help menu, constructed in `drawKeeperHelp` within `gui_builder.cpp`, is fully data-driven from `data_free/game_config/help.txt`. The function silently skips rendering any entry that is missing both a `viewId` (an icon) and a `title` (a translation key). This can lead to help topics being unintentionally hidden from the player if the configuration is incomplete. In this case, a "travelling" entry was defined without either, making it completely invisible.

**Action:** When adding or modifying data-driven UI elements, I will now actively check for and fix any incomplete entries that might cause them to be invisible to the user. I will also verify that all necessary assets, like icons and translation strings, are present to ensure the UI renders correctly.
