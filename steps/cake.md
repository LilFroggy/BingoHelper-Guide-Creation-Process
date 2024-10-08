[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Cake Step
Cake steps are considered complete when the length of the ``eaten`` property is >= 14.

## Example:
```js
{
    "type": "cake", // set the step type to cake
    "instruction": "Eat cakes &b%cakes%", // tell user what to do
    "eaten": [] // array to store eaten cakes
}
```
### Required Properties:
- type (String)
- instruction (String)
- eaten (Array)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)

> [!TIP]
> You can use ``%cakes%`` in the instruction to display the user's progress.
