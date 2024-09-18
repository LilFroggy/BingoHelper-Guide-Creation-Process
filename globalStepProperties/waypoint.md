# Waypoint Step Property
The waypoint step property is a gobal step property (it can be specified on any type of step).

### Structure:
```js
"waypoint": {
    "beam": true, // whether or not the waypoints have beams
    "list": [ // array of waypoints that are displayed one at a time
        { // waypoint #1
            "text": "Wheat", // name of waypoint #1
            "position": [ location array for waypoint #1
                42, // x-coordinate for waypoint #1
                70, // y-coordinate for waypoint #2
                -123 // z-coordinate for waypoint #2
            ],
            "radius": 4 // If you are closer than 4 blocks to waypoint #1, it will disappear and waypoint #2 will appear
        },
        { // waypoint #2
            "text": "Wheat", // name of waypoint #2
            "position": [ // location array for waypoint #2
                47, // x-coordinate for waypoint #2
                71, // y-coordinate for waypoint #2
                -137 // z-coordinate for waypoint #2
            ],
            "radius": 3 // If you are closer than 3 blocks to waypoint #2, it will disappear but reappear if you are 3 or more blocks away because it is the last waypoint in this list
        }
  
    ],
    "index": 0 // Specifies which waypoint to display. Automatically increase (goes to the next waypoint) when the player is within the specified radius of the current waypoint.
}
```
