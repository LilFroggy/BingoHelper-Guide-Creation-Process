# Waypoint Step Property
The waypoint step property is a gobal step property—it can be specified on any step.

### Structure:
```js
"waypoint": {
    "beam": true, // whether or not the waypoints should have beams
    "list": [ // array of waypoints that are displayed one at a time
        {
            "text": "Wheat", // name of waypoint #1
            "position": [
                42, // x-coordinate for waypoint #1
                70, // y-coordinate for waypoint #1
                -123 // z-coordinate for waypoint #1
            ],
            "radius": 4 // If you are closer than 4 blocks to waypoint #1, it will disappear and waypoint #2 will appear
        },
        {
            "text": "Wheat", // name of waypoint #2
            "position": [
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
### Example:
```diff
{
=    "type": "skill",
=    "instruction": "Unlock Farming 7",
=    "skill": "farming",
=    "level": 7,
+    "waypoint": {
+        "beam": true,
+        "list": [
+            {
+                "text": "Wheat",
+                "position": [
+                    42,
+                    70,
+                    -123
+                ],
+                "radius": 4
+            },
+            {
+                "text": "Wheat",
+                "position": [
+                    47,
+                    71,
+                    -137
+                ],
+                "radius": 3
+            }
+        ],
+        "index": 0
+    }
+}
```
> [!NOTE]
> Even though this is a skill step type, we could apply the same waypoint property to **ANY** type of step.
