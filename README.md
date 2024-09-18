# Guides
Guides are objects with metadata and a collection of [steps](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#steps).

### Structure:
```js
{
    "name": "Guide Name",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            // Steps go here
        ]
    }
}
```

# Steps
Steps are objects that contain information about what needs to be done in order to progress to the next step in a [guide](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#Guides). A list of step types can be found below.

### Step Types:
- [message](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/message.md#message-step)
- [cake](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/cake.md#cake-step)
- [sell](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/sell.md#sell-step)
- [buy](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/buy.md#buy-step)
- [coins](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/coins.md#coins-step)
- [has](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/has.md#has-step)
- [area](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/area.md#area-step)
- [subArea](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/subArea.md#subarea-step)
- [enchant](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/enchant.md#enchant-step)
- [reforge](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/reforge.md#reforge-step)
- [guiItem](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/guiItem.md#guiitem-step)
- [guiClickSlot](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/guiClickSlot.md#guiclickslot-step)
- [skill](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/skill.md#skill-step)
- [collection](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/collection.md#collection-step)

# Creating a Guide
Create guides by adding or deleting steps in the ``steps`` array under the ``data`` property of a guide object. Guides should follow [this](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md###Structure) format.

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
# Importing Guides
To import custom guides:
1. Copy the guide to your clipboard
2. Run ``/bh import``

> [!NOTE]
> You will want to disable ``Auto Import New Guides`` in settings so as not to overwrite your custom guide.
