# ClientCommand Step Property
The clientCommand step property is a gobal step property—it can be specified on any step. The clientCommand step property suggests a command for the user to run to help them complete their current step. This property differs from the [command]() step property because it sends the command client-side whereas command runs the command server-side.

### Structure:
```js
"clientCommand": "/bh skip" // client-command goes here
```
### Example:
```js
{
    "type": "message",
    "instruction": "Skip this step",
    "criteria": "lksajdlaskdj", // A message probably won't start with this!
    "clientCommand": "/bh skip"
}
```
