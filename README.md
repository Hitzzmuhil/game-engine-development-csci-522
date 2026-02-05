# Game Engine Development – CSCI 522

This repository contains my coursework, milestones, and assignments for **CSCI 522: Game Engine Development** at the University of Southern California. The project focuses on implementing core game engine systems, AI behaviors, rendering optimizations, physics, and debugging tools.

---

## Repository Structure

├── SYSTEMS.md # High-level overview of implemented systems
├── docs/ # Detailed PDFs for milestones and assignments
├── videos/ # Video demonstration links (hosted on Google Drive)
├── README.md # Main project overview

---

## Implemented Systems and Features

### Server-Based Asset Loading
- Implemented dynamic asset loading via an HTTP server
- Assets are fetched over the network instead of local disk storage
- Enables centralized asset management and seamless updates

### NPC Waypoint AI and Target Tracking
- Random waypoint-based movement with walk/run transitions
- Real-time target tracking using rotation alignment
- Shooting behavior based on range and line-of-sight detection

### Navigation Mesh Pathfinding
- Collision-free shortest path computation
- Intermediate waypoint generation for smooth movement
- Dynamic path recalculation for adaptive NPC navigation

### Frustum Culling using AABB
- Axis-Aligned Bounding Boxes computed per mesh
- Camera frustum plane generation
- Objects outside the view frustum are culled to optimize rendering
- Debug visualization to validate culling behavior

### Debug Visualization and Tools
- Persistent on-screen debug text displaying camera state
- Dynamic positioning to ensure continuous visibility
- Enhanced system transparency and debugging support

### Collision and Physics System
- Physics Manager for handling bounding volumes
- Sphere-based collision detection for soldiers
- Axis-Aligned Bounding Boxes for static objects
- Sliding collision response and gravity simulation

---

## Documentation

All detailed documentation for milestones and assignments is available in the `docs/` directory:

- Server-Based Asset Loading
- NPC Waypoint AI
- Navigation Mesh Pathfinding
- Frustum Culling with AABB
- Debug Visualization and Tools
- Collision and Physics System

Each document explains system design, implementation details, and behavior.

---

## Video Demonstrations

Video demonstrations are hosted externally due to GitHub file size limits.

Please refer to:  
➡️ **[`videos/README.md`](videos/README.md)**

This file contains:
- Google Drive links to all demo videos
- Descriptions of each video
- Corresponding milestones and assignments

---

## Notes

- Video files are not stored in this repository to comply with GitHub size constraints
- All demo videos are accessible via public Google Drive links
- This repository is intended for academic evaluation and learning purposes

---

## Author

**Name:** Muhil Thiruvenkadam  
**Course:** CSCI 522 – Game Engine Development  
**Institution:** University of Southern California
