# Command Step Property
The ``command`` step property is a gobal step property—it can be specified on any step. The ``command`` step property suggests a command for the user to run to help them complete their current step. This property differs from the [clientCommand](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/clientCommand.md#clientcommand-step-property) step property because it sends the command server-side whereas the ``clientCommand`` step property runs the command client-side.

### Structure:
```js
"command": "/warp hub" // replace /warp hub with your command
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
