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
            },
            {
                "type": "collection", // set the step type to collection
                "instruction": "Unlock Lapis Lazuli Collection 4", // tell user what to do
                "collection": "lapis_lazuli", // name of the collection
                "level": 4 // desired level in that collection
            }
            // add more steps here...
        ]
    }
}
```
