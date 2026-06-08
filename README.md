Question 6 · Dashboard
Combine four APIs · 20 marks · Topics: independent fetch chains, parallel requests, resilience

Concept

A dashboard shows several live values at once. The key idea: give each tile its own fetch chain so they run independently and in parallel — one failing API must never blank the others. Each chain still follows the same fetch → .then(json) → display → .catch skeleton.

Tasks

Build four tiles. On page load, populate four tiles from four different APIs:

Zanzibar weather
USD → TZS rate
Tanzania population
Advice of the moment

(8 marks)

Independent chains. Give each tile its own fetch + .then + .catch so a single failure shows "—" in that tile only, never breaking the others.

(4 marks)

Refresh. Add a "Refresh all" button that re-runs every tile’s fetch.

(3 marks)

Loading state. Show a placeholder (e.g. "...") in each tile while its request is pending.

(2 marks)

Layout. Arrange the tiles in a responsive grid so they reflow on a narrow screen.

(3 marks)

Total: 20 Marks
