---
title: VimCord
description: VimCord is a BetterDiscord plugin that brings Vim-style navigation and link hinting to Discord. Move around with hjkl, focus panes, and click anything using keyboard-driven hint labels.
poster: /projects/generic.webp
techstack:
  - JS
---

VimCord is a BetterDiscord plugin that brings Vim-style navigation and link hinting to Discord. Move around with hjkl, focus panes, and click anything using keyboard-driven hint labels. [[source](https://github.com/CyR1en/VimCord)]

### Features:
- Normal, Insert, and Hint modes with a subtle mode indicator in the user area
- Keyboard scrolling and pane switching (server list, channel list, DM/friends, chat)
- Robust hinting:
    - Filters visible/clickable elements
    - Handles click traps with a multi-strategy “real click” simulation
    - Live filtering as you type
    - Enter to accept; auto-accept after a short pause
    - Ambiguous exact matches wait (e.g., A vs. AA), unambiguous exact matches activate immediately
- Customizable visuals via BetterDiscord’s Custom CSS

### Preview:
![VimCord Preview](https://raw.githubusercontent.com/CyR1en/VimCord/refs/heads/main/media/image(hints).png)