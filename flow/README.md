# Pull request 14860: the whole flow at 1280 x 720

Pictures for [tangency-labs/solidcraft#14860](https://github.com/tangency-labs/solidcraft/pull/14860), "a link can keep a linked design's components as a linked subassembly, each occurrence rigid or flexible".

The example is a real assembly from my own work: a vacuum chamber of 211 bodies with a latch assembly linked into it. Every picture is the whole app window at 1280 x 720, uncropped (captured on a 150% display and scaled to 1280 x 720). The strip under each picture and the magenta marks are mine. The same pictures without marks are in [`plain/`](plain).

The pictures are from the pull request's branch at `39bebde94`.

## 1. The assembly and the ribbon

![Step 1: the chamber assembly on the Assemble tab](step-01-chamber-and-ribbon.png)

## 2. The two preferences, as shipped

![Step 2: Preferences, Design, Linked designs, both new options off](step-02-preferences-as-shipped.png)

## 3. Turning the option on

![Step 3: the first option ticked, the second now available](step-03-option-turned-on.png)

## 4. Insert Design

![Step 4: Assemble, Insert, the latch assembly picked from the open designs](step-04-insert-design.png)

## 5. The Browser: a linked subassembly

![Step 5: the latch in the Browser with its own component kept](step-05-linked-subassembly.png)

## 6. The Browser: its parts, locked

![Step 6: the latch's parts as locked components](step-06-kept-parts.png)

## 7. Keep Its Components, for a link that keeps none

![Step 7: the menu of a link that keeps no components, with Keep Its Components](step-07-keep-its-components.png)

## 8. The occurrence's menu: Make Flexible

![Step 8: the occurrence menu with Make Flexible](step-08-make-flexible.png)

## 9. Flexible: the latch's joints are joints of this design

![Step 9: the latch's twelve joints in the Browser, the History bar and the view](step-09-joints-carried.png)

## 10. The same menu now offers Make Rigid

![Step 10: the occurrence menu with Make Rigid](step-10-make-rigid.png)

## 11. The result: the latch driven open inside the chamber

![Step 11: the latch's shaft driven to -84.8 degrees](step-11-latch-driven-open.png)

## 12. The result: one latch flexible and open, the other as saved

![Step 12: the whole chamber, lower latch open, upper latch as saved](step-12-result.png)

## Detail: the greyed preference says what it needs

![The tooltip of the second preference while the first is off](detail-greyed-option-tooltip.png)

## What these show for the small window

- The two preferences each fit on one line of Preferences › Design › Linked designs (steps 2 and 3). The second is greyed until the first is on, and its tooltip says why (last picture).
- The new menu items sit in the existing Component submenu, one at a time: Keep Its Components, Make Flexible or Make Rigid (steps 7, 8 and 10). The menu and its submenu stay inside the window.
- The Browser shortens long names as it does for any component. A kept component has a lock (steps 5 and 6), and a flexible occurrence's joints are listed with the design's joints (step 9).

One thing that is not from this change: the warning mark on the first History item is the chamber body's own STEP import (three of its bodies come in as surfaces).
