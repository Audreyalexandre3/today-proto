# Today · Agorapulse prototype

A clickable prototype of an action-oriented **Today** page in Agorapulse, and of the same action item shown on three surfaces (the app, an AI assistant briefing, a team chat notification).

- `index.html`: the Today page inside the Agorapulse app shell. Items are grouped by priority (Needs you, Worth a look, Good news), each with the agent's reason and actions you can take in place. Done items fold away into "Done today" with Undo.
  - **Start my day** (or press F) opens Focus: one item at a time, A for the main action, S to snooze, arrows to move, Esc to exit.
  - After a few seconds a new item arrives from the agents (a 5-star review), live.
  - Clearing everything shows an All clear recap with a short confetti burst. Animations respect reduced motion.
- `surfaces.html`: one action item on three surfaces, and the data model they share.

Built with the Agorapulse design system (`@agorapulse/ui-theme` 22.0.7 and `@agorapulse/ui-symbol` 22.0.0 from jsDelivr). Demo data only (Maison Lumen is a fictional brand). The "Today" rail item is the proposal; it isn't in the product.
