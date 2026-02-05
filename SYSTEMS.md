\# Technical Systems Overview



This document describes the implementation details and design decisions of the major systems implemented for CSCI 522.



\## NPC AI \& Waypoints

\- Four-waypoint random movement, randomized walk/run speeds.

\- Target tracking with facing rotation and line-of-sight shooting (demo in docs/Assignment-2).



\## Navigation Mesh \& Pathfinding

\- NavMesh built over level geometry.

\- Collision-free shortest-path calculation; intermediate waypoints placed evenly.

\- Dynamic path recalculation when camera/scene changes to maintain robustness.



\## Collision \& Physics Manager

\- Physics Manager stores bounding volumes: sphere for dynamic actors, AABB for static geometry.

\- Collision detection uses radius checks and projects movement to slide along colliding surfaces.

\- Gravity: if no supporting surface, actor Y coordinate decreases incrementally until collision.



\## Frustum Culling \& Rendering Optimization

\- AABB computed from mesh position buffers and tested against camera frustum planes.

\- DebugRenderer visualizes bounding boxes and frustum for validation, improving rendering performance.



\## Server-based Asset Loading

\- HTTP server hosts the `AssetsOut` folder.

\- FileReader logic modified to issue HTTP GETs and buffer assets in memory, preserving compatibility with original file I/O.



\## Debug \& Visualization

\- Added persistent debug text overlays (e.g., "Trailing Camera") and runtime visualizers for developers.





