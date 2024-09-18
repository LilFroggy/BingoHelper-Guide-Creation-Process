[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Reforge Step
Reforge steps are considered complete when every item in the ``items`` property has been in the reforge slot in the reforge menu with one of its accepted reforges.

## Example:
```js
{
    "type": "reforge", // set the step type to reforge
    "instruction": "Reforge items", // tell user what to do
    "items": {
        "END_SWORD": { // item #1 to reforge (skyblock id)
            "reforges": [ // array of acceptable reforges
                "Sharp",
                "Spicy"
            ],
            "done": false
        },
        "MUSHROOM_HELMET": { // item #2 to reforge (skyblock id)
            "reforges": [
                "Fierce"
            ],
            "done": false
        }
        // add more items to reforge here...
    }
}
```
### Required Properties:
- type (String)
- instruction (String)
- items (Object)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)

> [!NOTE]
> Items listed in the ``items`` property are highlighted in the player's inventory while the reforge menu is open if that item has not been in the reforge slot with an acceptable reforge and an item is not currently being reforged.

> [!WARNING]
> Attempts to reforge (clicks) are cancelled if the following statements are true:
> 1. The current item being reforged is specified in ``items``
> 2. The current reforge item has one of its accepted reforges
> 3. The current or previous step is a reforge step
