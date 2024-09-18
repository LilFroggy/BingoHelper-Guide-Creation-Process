[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Buy Step
Buy steps are considered complete when the user has bought the desired amount of every item specified in the ``items`` property.

## Example:
```js
{
    "type": "buy", // set the step type to buy
    "instruction": "Buy Rookie Hoe &b%1%\nBuy Red Mushrooms &b%2%", // tell user what to do
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
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)

> [!NOTE]
> Items listed in the ``items`` property are highlighted in menus:
> - **Green Highlight**: buying that amount will not put you over the target
> - **Yellow Highlight**: buying that amount will put you over target.
> 
> The largest quantity that does not put you over the target is highlighted in the shop trading options menu.

> [!TIP]
> You can use ``%1%`` in the instruction to display the user's progress for item #1, ``%2%`` for item #2 and so on.
