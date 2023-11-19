# Smart-Target (Variant Fork)

![Latest Release Download Count](https://img.shields.io/github/downloads/p4535992/foundryvtt-smart-target-variant/latest/module.zip?color=2b82fc&label=DOWNLOADS&style=for-the-badge)

[![Forge Installs](https://img.shields.io/badge/dynamic/json?label=Forge%20Installs&query=package.installs&suffix=%25&url=https%3A%2F%2Fforge-vtt.com%2Fapi%2Fbazaar%2Fpackage%2Fsmart-target-variant&colorB=006400&style=for-the-badge)](https://forge-vtt.com/bazaar#package=smart-target-variant)

![Foundry Core Compatible Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-smart-target-variant%2Fmaster%2Fsrc%2Fmodule.json&label=Foundry%20Version&query=$.compatibility.verified&colorB=orange&style=for-the-badge)

![Latest Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-smart-target-variant%2Fmaster%2Fsrc%2Fmodule.json&label=Latest%20Release&prefix=v&query=$.version&colorB=red&style=for-the-badge)

[![Foundry Hub Endorsements](https://img.shields.io/endpoint?logoColor=white&url=https%3A%2F%2Fwww.foundryvtt-hub.com%2Fwp-json%2Fhubapi%2Fv1%2Fpackage%2Fsmart-target-variant%2Fshield%2Fendorsements&style=for-the-badge)](https://www.foundryvtt-hub.com/package/smart-target-variant/)

![GitHub all releases](https://img.shields.io/github/downloads/p4535992/foundryvtt-smart-target-variant/total?style=for-the-badge)

[![Translation status](https://weblate.foundryvtt-hub.com/widgets/smart-target-variant/-/287x66-black.png)](https://weblate.foundryvtt-hub.com/engage/smart-target-variant/)

A user interface to manage companions with summoning animations and automated summoning for spells

![hud](./wiki/feature_hud_ce_1.gif)

**Note: This is module is inspired from the  wonderful work done by [theRipper93](https://github.com/theripper93) with its [smart-target](https://github.com/theripper93/smart-target) module.
If you want to support more modules of this kind, I invite you to go and support his patreon**

[![alt-text](https://img.shields.io/badge/-Patreon-%23ff424d?style=for-the-badge)](https://www.patreon.com/theripper93) [![alt-text](https://img.shields.io/badge/-Discord-%235662f6?style=for-the-badge)](https://discord.gg/F53gBjR97G)

## With theripper93's permission i implemented a variant (or custom patch) of his project, these are the differences:

- NEW SETTING: Add module settings for disable 'CLear ll targets' button
- NEW FEATURE: Embedded integration of the module [Manage Player Targets](https://github.com/dev7355608/manage-player-targets)
- NEW SETTING: Set the PIXI Pointer of "Better Target" as default...

## You can find the documentation on the [WIKI](https://api.theripper93.com/modulewiki/smarttarget/free)

## Features

1. Target with `Alt + Click`
2. For players, target by just left clicking a non-owned
   token (Alt+Click to target owned token)
3. Target all tokens in a template by `Alt + Click`ing the template
   *(shift modifier and standard\\sticky behaviour apply)*
4. Show portraits instead of colored pips to indicate targets, positioning\\offset and
   size of the icons can be configured in the module settings 5. Customize color\\shape
   of the targeting reticule

<img src="./wiki/smartTarget.jpg" width="300" height="300">

<img src="./wiki/targetoptions.jpg" height="300">

## Settings

- **Targeting Mode**
  - **Default**: Default foundry behaviour.
  - **Alt-click**: Target tokens by pressing Alt+Click, add Shift to
    target multiple.
  - **Always Target**: Clicking on non-owned tokens automatically
    targets them"
- **Release Behaviour**
  - This setting determines how refresh target
    behaves when clicking multiple tokens.
  - Options:
    - **Sticky** mode will target each clicked token without
      un-targeting anything, and you must click a token again to
      un-target it.
    - **Standard** mode more closely matches the standard foundry
      behaviour where all previous tokens are automatically
      un-targeted when clicking a new token, and you must hold Shift
      while clicking in order to target multiple tokens.
- **Show indicator portraits instead of colors**
  - Uses avatar for GM,
    defaults to Token for players if no avatar is found for the assigned
    actor (requires refresh)
- **Use Tokens instead of Avatars**: Use tokens instead of avatars for
  players target indicators
- **GM Image**
  - The image to use on indicator portraits for the GM
  - Options
    - Player Avatar
    - Token Portrait
    - Token Image
- **Keep target indicators inside the token**: Move the target indicators
  in a way that they remain inside the token border
- **Target Icon Image Scale**: Set the scale for the image used by the
  target icons (default: 1)
- **Target Image Y Offset**: Add a flat offset to the image in pixels
  (default: 0)
- **Target Image X Offset**: Add a flat offset to the image in pixels
  (default: 0)
- **Target Icon Size**: Set the size for the target icon in pixels
  (default: 12)
- **Target Icon Offset**: Set the distance between icons in pixels
  (default: 16)
- **Border Thickness**: Set the thickness of the border in pixels
  (default: 2)
- **Bring Targeting Arrows Closer Together**: Bring the targeting arrows
  closer together so that they are inside the token frame
- **Targeting Arrows Color**: Hex color for the targeting arrows (default:
  `#ff9829`)
- **Target indicator**: Select the indicator for a targeted token
  - Default Foundry Indicator
  - CrossHair 1
  - CrossHair 2
  - BullsEye 1
  - BullsEye 2
  - Better Target
- **Use player color for target indicator**: Use player color for target indicator