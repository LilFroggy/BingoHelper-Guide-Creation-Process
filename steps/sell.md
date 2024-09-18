# Cake Step
Sell steps are considered complete when the user has no items in their inventory (including armor slots) with an id specified in the ``items`` property.

## Example:
```js
{
        "type": "sell",
        "instruction": "Sell materials",
        "items": [
                "HAY_BLOCK", // skyblock id
                "WHEAT",
                "SEEDS"
        ]
}
```
### Required Properties:
- type (String)
- instruction (String)
- eaten (Array)

### Optional Properties:
- waypoint (object)
- command (String)
- clientCommand (String)

> [!WARNING]
> You can use ``%cakes%`` in the instruction to display the user's progress.
