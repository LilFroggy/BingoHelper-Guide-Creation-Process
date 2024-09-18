# GuiItem Step
GuiItem steps are considered complete when either:
1. ``itemIndex``, ``has``, and ``doesntHave`` are all nullish but ``guiName`` matches the player's current container name.
2. The item with index ``itemIndex`` (zero-based indexing) in the the gui named ``guiName`` has lore that includes the string ``has`` but does not include the string ``doesntHave``.

## Example:
```js
{
    "type": "message", // set the step type to message
    "instruction": "Run /warp hub", // tell user what to do
    "criteria": "Warping..." // Waring... appears in chat when users run /warp hub
}
```
### Required Properties:
- type (String)
- instruction (String)
- criteria (String)

### Optional Properties:
- waypoint (Object)
- command (String)
- clientCommand (String)
