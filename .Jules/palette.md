## 2025-05-15 - Improving Help Menu Organization
**Learning:** In KeeperRL, help menu entries in `help.txt` are silently filtered out by the UI if they lack either an icon (`viewId`) or a title. This can make help topics (like "Travelling") invisible even if their content file exists.
**Action:** Always verify that every help scriptedId has a corresponding icon and translation key in the configuration to ensure visibility.
