# ClientCommand Step Property
The ``clientCommand`` step property is a gobal step property—it can be specified on any step. The ``clientCommand`` step property suggests a command for the user to run to help them complete their current step. This property differs from the [command](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/globalStepProperties/command.md#command-step-property) step property because it sends the command client-side whereas the ``command`` step property runs the command server-side.

### Structure:
```js
"clientCommand": "/bh skip" // replace /bh skip with your client-command
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
