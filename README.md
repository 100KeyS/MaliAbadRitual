Built as a single dependency-free HTML file — no framework,
 no build step — as a deliberate constraint.
 Along the way I hit a real mobile performance wall:
 several animations were forcing the browser to repaint every frame,
 instead of letting the GPU just composite,
 so I rewrote them around opacity/transform only,
 and fixed a classic flexbox overflow bug 
(implicit min-width: auto) that broke long strings on narrow screens.
https://100keys.github.io/MaliAbadRitual/
