# Buy Step
Buy steps are considered complete when the user has reached the desired target for every item specified in the ``items`` property.

## Example:
```js
{
    "type": "buy",
    "instruction": "Buy Rookie Hoe &b%1%\nBuy Red Mushrooms &b%2%",
    "items": {
        "ROOKIE_HOE": { // item #1 (Skyblock ID)
            "count": 0, // # bought
            "target": 1, // # to buy
            "done": false // status
        },
        "RED_MUSHROOM": { // item #2 (Skyblock ID)
            "count": 0, // # bought
            "target": 24, // # to buy
            "done": false // status
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
> Items listed in the ``items`` property are highlighted in menus where they can be sold (npc shops, trade menu, etc.).
