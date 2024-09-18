# Cake Step
Cake steps are considered complete when the length of the ``eaten`` property is >= 14.

## Example:
```js
{
    "type": "cake", // set the step type to cake
    "instruction": "Eat cakes &b%cakes%", // tell the user what they should do
    "eaten": [] // create an array to store eaten cakes
}
```
### Required Properties:
- type (String)
- instruction (String)
- eaten (Array)

### Optional Properties:
- waypoint (object)
- command (String)
- clientCommand (String)


> [!TIP]
> You can use **%cakes%** to reference the current number of unique cakes eaten in the instruction.
