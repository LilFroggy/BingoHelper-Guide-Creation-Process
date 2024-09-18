# Cake Step
Cake steps are considered complete when the length of the ``eaten`` property is >= 14.

## Example:
```js
{
    "type": "message", // set the step type to message
    "instruction": "Run /warp hub", // tell the user what they should do
    "criteria": "Warping..." // Waring... appears in chat when users run /warp hub
}
```
### Required Properties:
- type (String)
- instruction (String)
- criteria (String)

### Optional Properties:
- waypoint (object)
- command (String)
- clientCommand (String)
