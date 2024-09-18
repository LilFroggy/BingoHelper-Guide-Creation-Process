# Message Step
Message steps are considered compelted when the message specified under ``step.criteria`` is found in chat.

## Example:
```js
{
    "type": "message", // type is a required property for all steps
    "instruction": "Run /warp hub", // instruction is a required property for all steps
    "criteria": "Warping..."
}
```
