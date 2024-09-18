[< Back](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/README.md#step-types)
# Skill Step
Skill steps are considered complete when the user reaches level ``level`` or higher in the ``skill`` skill.

## Example:
```js
{
    "type": "skill", // set the step type to skill
    "instruction": "Unlock Combat 12", // tell user what to do
    "skill": "combat", // name of the skill
    "level": 12 // desired level in that skill
}
```
### Required Properties:
- type (String)
- instruction (String)
- skill (String)
- level (Number)

### Optional Properties:
- [waypoint](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/waypoint.md#waypoint-step-property) (Object)
- command (String)
- clientCommand (String)
