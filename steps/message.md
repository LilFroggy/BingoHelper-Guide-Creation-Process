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
- waypoint (Object)
- command (String)
- clientCommand (String)
