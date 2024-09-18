[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# SubArea Step
SubArea steps are considered complete when the sub area specified in the ``subArea`` property matches the subArea on the scoreboard.

## Example:
```js
{
    "type": "subArea", // set the step type to subArea
    "instruction": "Go to the gunpowder mines", // tell user what to do
    "subArea": "Gunpowder Mines" // sub-area located on scoreboard
}
```
### Required Properties:
- type (String)
- instruction (String)
- subArea (String)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- command (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)
