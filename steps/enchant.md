# Enchant Step
Enchant steps are considered complete when every item in the ``items`` property has been in the enchanting slot in the enchantment table with all of the desired enchants on it.

## Example:
```js
{
    "type": "enchant", // set the step type to enchant
    "instruction": "Enchant items", // tell user what to do
    "items": {
        "GOLD_AXE": { // (skyblock id)
            "enchants": [ // array of enchants to go on the gold axe
                "Efficiency V",
                "Silk Touch I"
            ],
            "done": false
        },
        "PROMISING_PICKAXE": {
            "enchants": [
                "Efficiency V",
                "Fortune III"
            ],
            "done": false
        }
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
