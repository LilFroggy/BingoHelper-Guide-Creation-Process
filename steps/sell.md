# Sell Step
Sell steps are considered complete when the user has no items in their inventory with an id specified in the ``items`` property.

## Example:
```js
{
    "type": "sell", // set the step type to sell
    "instruction": "Sell items", // tell user what to do
    "items": [ // array of items to sell (not have in inventory)
        "HAY_BLOCK", // (skyblock id)
        "WHEAT",
        "SEEDS"
    ]
}
```
### Required Properties:
- type (String)
- instruction (String)
- items (Array)

### Optional Properties:
- waypoint (Object)
- command (String)
- clientCommand (String)

> [!NOTE]
> Items listed in the ``items`` property are highlighted in menus where they can be sold (npc shops, trade menu, etc.).
