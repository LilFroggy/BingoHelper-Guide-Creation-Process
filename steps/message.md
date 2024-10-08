[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Message Step
Message steps are considered complete when a message appears in chat that starts with the text specified in the ``criteria`` property.

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
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) (String)
- [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) (String)
