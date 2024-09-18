# Buy Step
Buy steps are considered complete when the user has bought the desired amount of every item specified in the ``items`` property.

## Example:
```js
{
    "type": "buy",
    "instruction": "Buy Rookie Hoe &b%1%\nBuy Red Mushrooms &b%2%",
    "items": {
        "ROOKIE_HOE": { // item #1 (skyblock id)
            "count": 0, // # bought
            "target": 1, // # to buy
            "done": false // status
        },
        "RED_MUSHROOM": { // item #2
            "count": 0,
            "target": 24,
            "done": false
        }
        // add more items here...
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
> Items listed in the ``items`` property are highlighted in menus:
> - **Green Highlight**: buying that amount will not put you over the target
> - **Yellow Highlight**: buying that amount will put you over target.
> 
> The largest quantity that does not put you over the target is highlighted in the shop trading options menu.

> [!TIP]
> You can use ``%1%`` in the instruction to display the user's progress for item #1, ``%2%`` for item #2 progress and so on.
