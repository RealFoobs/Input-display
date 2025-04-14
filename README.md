Shiyo Kakuge's ADD004 input display system, updated to work with the new explod logic and trimmed down to a common file.

![alt text](https://raw.githubusercontent.com/RealFoobs/Input-display/refs/heads/main/Animation.gif)

**Installation**

Extract the release folder to `data/`. Change your config.ini from this:

```
States  = data/functions.zss, data/action.zss, data/dizzy.zss, data/guardbreak.zss, data/score.zss, data/system.zss, data/tag.zss, data/training.zss
; Common packs of graphic and/or sound effects called during the match by using
; a specific prefix before animation and sound numbers (like lifebar fightfx)
Fx      =
```

To something like this:

```
States  = data/functions.zss, data/action.zss, data/dizzy.zss, data/guardbreak.zss, data/score.zss, data/system.zss, data/tag.zss, data/training.zss, data/inputdisplay/inputdisplay.zss
; Common packs of graphic and/or sound effects called during the match by using
; a specific prefix before animation and sound numbers (like lifebar fightfx)
Fx      = data/inputdisplay/inputdisplay.def
```

**Notes**

These files will only work with Ikemen's nightly build as of 2025/04/14, not on 0.99 or earlier versions.

If you think the icons are too small, you can always go to inputdisplay.def and change the localcoord to something like 240,180.

The input explods are controlled by a helper, so there will be 1 frame delay between button press and the icons showing up. This may or may not be changed in the future.
