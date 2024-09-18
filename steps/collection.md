[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Collection Step
Collection steps are considered complete when the user reaches level ``level`` or higher in the ``collection`` collection.

## Example:
```js
{
    "type": "collection", // set the step type to collection
    "instruction": "Unlock Lapis Lazuli Collection 4", // tell user what to do
    "collection": "lapis_lazuli", // name of the collection
    "level": 4 // desired level in that collection
}
```
### Required Properties:
- type (String)
- instruction (String)
- collection (String)
- level (Number)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- command (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)
