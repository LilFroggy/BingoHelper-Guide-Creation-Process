[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# GuiItem Step
GuiItem steps are considered complete when either:
1. ``itemIndex``, ``has``, and ``doesntHave`` are all nullish but ``guiName`` matches the player's current container name.
2. The item with index ``itemIndex`` in the the gui named ``guiName`` has lore that includes the string ``has`` but does not include the string ``doesntHave`` (if ``has`` or ``doesntHave`` is nullish, its check is ignored).

## Example:
```js
{
    "type": "guiItem", // set the step type to guiItem
    "instruction": "Apply Dirt Bottle to End Sword", // tell user what to do
    "guiName": "Reforge Anvil", // this is the gui name for the menu where you apply reforge stones
    "itemIndex": 13, // this is the index (use zero-based indexing) for the slot where the result of the two inputs is shown 
    "has": "Dirty End Sword", // we expect this item to be named Dirty End Sword (item name is part of the lore)
    "doesntHave": "Click the ANVIL BELOW to combine." // we don't want the item to say this because if it does, we haven't combined the items yet
}
```
### Required Properties:
- type (String)
- instruction (String)
- guiName (String)

### Optional Properties:
- itemIndex (Number)
- has (String)
- doesntHave (String)
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)
