# Reforge Step
Reforge steps are considered complete when every item in the ``items`` property has been in the reforge slot in the reforge menu with its desired reforge.

## Example:
```js
{
    "type": "reforge", // set the step type to reforge
    "instruction": "Reforge items", // tell user what to do
    "items": {
        "END_SWORD": { // item #1 (skyblock id)
            "reforges": [ // array of acceptable reforges
                "Sharp"
            ],
            "done": false
        },
        "MUSHROOM_HELMET": { // item #2 (skyblock id)
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
- waypoint (Object)
- command (String)
- clientCommand (String)

> [!NOTE]
> Items listed in the ``items`` property are highlighted in the player's inventory while the reforge menu is open if that item has not been in the reforge slot with the desired reforge and an item is not currently being reforged.
