[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Enchant Step
Enchant steps are considered complete when every item in the ``items`` property has been in the enchanting slot in the enchantment table with all of the desired enchants on it.

## Example:
```js
{
    "type": "enchant", // set the step type to enchant
    "instruction": "Enchant items", // tell user what to do
    "items": {
        "GOLD_AXE": { // item #1 to enchant (skyblock id)
            "enchants": [ // array of desired enchants on gold axe
                "Efficiency V",
                "Silk Touch I"
            ],
            "done": false
        },
        "PROMISING_PICKAXE": { // item #2 to enchant
            "enchants": [
                "Efficiency V",
                "Fortune III"
            ],
            "done": false
        }
        // add more items to enchant here...
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
> Items listed in the ``items`` property are highlighted in the player's inventory while the enchantment table menu is open if that item has not been fully enchanted and an item is not currently being enchanted. Desired enchants that are not present on the item being enchanted are highlighted.
