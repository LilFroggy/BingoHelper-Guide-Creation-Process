# Message Step
Area steps are considered complete when the area specified in the ``area`` property matches the area in tab.

## Example:
```js
{
    "type": "area", // set the step type to area
    "instruction": "Run /warp deep", // tell user what to do
    "area": "Deep Caverns" // this is the area in tab when in the deep caverns
}
```
### Required Properties:
- type (String)
- instruction (String)
- area (String)

### Optional Properties:
- waypoint (Object)
- command (String)
- clientCommand (String)

