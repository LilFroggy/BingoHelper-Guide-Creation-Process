# Command Step Property
The command step property is a gobal step property—it can be specified on any step. The command step suggests a command for the user to run to help them complete their current step.

### Structure:
```js
"command": "/warp hub" // command goes here
```
### Example:
```js
{
    "type": "message",
    "instruction": "/warp hub",
    "criteria": "Warping...",
    "command": "/warp hub"
}
```
> [!NOTE]
> Even though this is a message step type, we could apply the same command property to **ANY** type of step.
