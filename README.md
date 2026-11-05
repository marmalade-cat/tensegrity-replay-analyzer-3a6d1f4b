TensegrityReplayAnalyzer

Simple prototype web app to load module pose time-series (CSV or JSON), normalize timestamps and coordinate frames, preview 2D/3D trajectories, and export replay-ready JSON. Drag a file onto the page or click Load. CSV expects header: timestamp,x,y,z,qw,qx,qy,qz,module_id. Output is a JSON array [{t, module_id, pos:[x,y,z], quat:[qw,qx,qy,qz]}].

Usage:
- Open index.html in a modern browser (no server required).
- Load CSV or JSON.
- Use controls to normalize time and flip axes.
- Click Export to download replay JSON.

Notes:
- This is a prototype. No external libs, limited validation.
- Interpretation: timestamps normalized to start at 0; axis flips are simple coordinate transforms. Adjust as needed for your replay tool.

