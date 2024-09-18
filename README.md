# How to Create a Guide
Guides are a collection of steps.

## Structure:
```js
{
    "name": "Guide Name",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            // Put steps here
        ]
    }
}
```
Use the format above to create and edit guides by adding and deleting steps in the ``steps`` array under the ``data`` property.

### Example:
```js
{
    "name": "Example Guide",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            {
                "type": "message",
                "instruction": "Run /warp hub",
                "criteria": "Warping..."
            },
            {
                "type": "collection",
                "instruction": "Unlock Lapis Lazuli Collection 4",
                "collection": "lapis_lazuli",
                "level": 4
            }
            // add more steps here...
        ]
    }
}
```

# What is a Step?
Steps are objects that contain information about what needs to be done in order to advance to the next step in the guide. A list of all step types can be found below:

[Message](https://github.com/LilFroggy/BingoHelper-Guide-Creation-Process/blob/master/steps/message.md#message-step)
