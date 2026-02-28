# OpenMower-Simple-Visual-Map-Editor
A lightweight, zero-dependency, single-file HTML application to visually view, edit, and optimize map.json files for OpenMower.

Features:
Accurate Coordinate System: Translates standard screen graphics perfectly into OpenMower's ROS/GPS-based cartesian math (Y-axis pointing North). Includes a metric grid and origin (0,0) indicator.

Visual Node Editing: Drag and drop nodes, double-click lines to add points, and right-click to delete them. Allows editing of the Docking Station heading graphically.

Point Protection (Locking): Mark crucial points as "Favorites/Locked" to prevent accidental modifications or deletion. Locked state is safely hidden inside GeoJSON metadata without breaking OpenMower logic.

Path Subdivide & Simplify: Automatically halve point density to optimize robot CPU load, or double point density for higher precision curves.

Interactive Background Alignment: Load a satellite image or drone shot of your garden, position/scale it independently to match your map data, then lock it into the world view to use as a tracking reference.

100% Client-Side: No server, no Node.js required. Works entirely locally in your browser to guarantee data privacy.
