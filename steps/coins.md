# Coins Step
Coins steps are considered complete when the sum of the user's bank and purse is >= the amount specified in the ``target`` property.

## Example:
```js
{
    "type": "coins", // set the step type to coins
    "instruction": "Get coins from leveling up enchanting &6%coins%", // tell user what to do
    "count": 0, // how many coins the user has
    "target": 50000 // how many coins we want the user to have
}
```
### Required Properties:
- type (String)
- instruction (String)
- count (Number)
- target (Number)

### Optional Properties:
- waypoint (Object)
- command (String)
- clientCommand (String)

> [!TIP]
> You can use ``%coins%`` in the instruction to display the user's progress.
