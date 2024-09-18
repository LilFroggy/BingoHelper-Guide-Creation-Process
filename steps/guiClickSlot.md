[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# GuiClickSlot Step
GuiClickSlot steps are considered complete when the user clicks on the slot with index ``slotIndex`` in the gui named ``guiName``.

## Example:
```js
{
    "type": "guiClickSlot", // set the step type to guiClickSlot
    "instruction": "Take lift to Lapis Quarry", // tell user what to do
    "guiName": "Lift", // this is the gui name for the lift
    "slotIndex": 12 // this is the index (use zero-based indexing) for the lapis quarry warp
}
```
### Required Properties:
- type (String)
- instruction (String)
- guiName (String)
- slotIndex (Number)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- command (String)
- clientCommand (String)

> [!NOTE]
> The slot with index ``slotIndex`` is highlighted in the gui named ``guiName``.
