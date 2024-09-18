# Message Step
Message steps are considered compelted when the message specified under ``step.criteria`` is found in chat.

## Example:
```js
{
    "type": "message", // set the step type to message
    "instruction": "Run /warp hub", // tell the user what they should do
    "criteria": "Warping..." // Waring... appears in chat when users run /warp hub
}
```
### Required Properties:
- type
- instruction
- criteria

### Optional Properties:
- waypoint
- command
- clientCommand
