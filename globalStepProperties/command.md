# Command Step Property
The command step property is a gobal step property—it can be specified on any step. The command step property suggests a command for the user to run to help them complete their current step. This property differs from the clientCommand step property because it sends the command server-side whereas clientCommand runs the command client-side.

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
