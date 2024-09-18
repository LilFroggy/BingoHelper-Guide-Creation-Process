# Guides
Guides are a collection of steps.

### Structure:
```js
{
    "name": "Guide Name",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            // Put steps here
        ]
    }
}
```
Use the format above to create and edit guides by adding and deleting steps in the ``steps`` array under the ``data`` property.

### Example:
```js
{
    "name": "Example Guide",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            {
                "type": "message",
                "instruction": "Run /warp hub",
                "criteria": "Warping..."
            },
            {
                "type": "collection",
                "instruction": "Unlock Lapis Lazuli Collection 4",
                "collection": "lapis_lazuli",
                "level": 4
            }
            // add more steps here...
        ]
    }
}
```

# What is a Step?
Steps are objects that contain information about what needs to be done in order to advance to the next step in a guide. A list of step types can be found below.

### Step Types:
- [Message](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/message.md#message-step)
- [Cake](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/cake.md#cake-step)
- [Sell](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/sell.md#sell-step)
- [Buy](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/buy.md#buy-step)
- [Coins](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/coins.md#coins-step)
- [Has](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/has.md#has-step)
- [Area](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/area.md#area-step)
- [subArea](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/subArea.md#subarea-step)
- [Enchant](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/enchant.md#enchant-step)
- [Reforge](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/reforge.md#reforge-step)
- [guiItem](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/guiItem.md#guiitem-step)
- [guiClickSlot](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/guiClickSlot.md#guiclickslot-step)
- [Skill](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/skill.md#skill-step)
- [Collection](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/collection.md#collection-step)
