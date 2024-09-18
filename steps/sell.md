# Sell Step
Sell steps are considered complete when the user has no items in their inventory with an id specified in the ``items`` property.

## Example:
```js
{
        "type": "sell",
        "instruction": "Sell materials",
        "items": [
                "HAY_BLOCK", // skyblock id (String)
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
> Items listed in the ``items`` array are highlighted in menus where they can be sold (npc shops, trade menu, etc...).

> [!WARNING]
> You can use ``%cakes%`` in the instruction to display the user's progress.
