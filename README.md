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
    "name": "Guide Name",
    "version": 1,
    "data": {
        "stepIndex": 0,
        "steps": [
            {
                "type": "message",
                "instruction": "Run /warp hub",
                "criteria": "Warping..."
            }
        ]
    }
}
```
