# Guides
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
Use the format above to create and edit guides.

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
