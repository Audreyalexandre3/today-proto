# Today · Agorapulse prototype

A clickable prototype of an action-oriented **Today** page in Agorapulse, and of the same action item shown on three surfaces (the app, an AI assistant briefing, a team chat notification).

- `index.html`: the Today page inside the Agorapulse app shell. Items are grouped by priority (Needs you, Worth a look, Good news), each with the agent's reason and actions you can take in place. Done items fold away into "Done today" with Undo.
  - **Start my day** (or press F) opens Focus: one item at a time, A for the main action, S to snooze, arrows to move, Esc to exit.
  - After a few seconds a new item arrives from the agents (a 5-star review), live.
  - Clearing everything shows an All clear recap with a short confetti burst. Animations respect reduced motion.
- `surfaces.html`: one action item on three surfaces, and the data model they share.

Built with the Agorapulse design system (`@agorapulse/ui-theme` 22.0.7 and `@agorapulse/ui-symbol` 22.0.0 from jsDelivr). Demo data only (Maison Lumen is a fictional brand). The "Today" rail item is the proposal; it isn't in the product.


## Exploration: Today, clean (`next.html`)

A second take outside the design system: a clean off-white look with one plain font (Inter), white cards and black buttons, plus new patterns: a card deck you swipe right to act and left to snooze (or ← →), a ⌘K command bar, a live agent feed that types in new activity, a bento of numbers, a progress ring, and an All clear end state. The inbox card's Review buttons open a side panel to handle spam, drafted replies and "your call" items one by one (keep, hide, send, skip, edit a reply for one person or a whole group). Live: https://audreyalexandre3.github.io/today-proto/next.html
