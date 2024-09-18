[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Has Step
Has steps are considered complete when the user has had every item, with its specified amount, in the ``items`` property in their inventory.

## Example:
```js
{
    "type": "has", // set the step type to has
    "instruction": "Obtain Cobblestone &b%1%\nObtain Stone &b%2%", // tell user what to do
    "items": {
        "COBBLESTONE": { // item #1 (skyblock id)
            "count": 0, // # obtained
            "target": 128, // # to obtain
            "done": false // status
        },
        "STONE": { // item #2
            "count": 0,
            "target": 64,
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

> [!TIP]
> You can use ``%1%`` in the instruction to display the user's progress for item #1, ``%2%`` for item #2 and so on.
