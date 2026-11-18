# Today · Agorapulse prototype

A clickable prototype of an action-oriented **Today** page in Agorapulse, and of the same action item shown on three surfaces (the app, an AI assistant briefing, a team chat notification).

- `index.html`: the Today page inside the Agorapulse app shell. Items are grouped by priority (Needs you, Worth a look, Good news), each with the agent's reason and actions you can take in place. Done items fold away into "Done today" with Undo.
  - **Start my day** (or press F) opens Focus: one item at a time, A for the main action, S to snooze, arrows to move, Esc to exit.
  - After a few seconds a new item arrives from the agents (a 5-star review), live.
  - Clearing everything shows an All clear recap with a short confetti burst. Animations respect reduced motion.
- `surfaces.html`: one action item on three surfaces, and the data model they share.

Built with the Agorapulse design system (`@agorapulse/ui-theme` 22.0.7 and `@agorapulse/ui-symbol` 22.0.0 from jsDelivr). Demo data only (Maison Lumen is a fictional brand). The "Today" rail item is the proposal; it isn't in the product.


## Exploration: Today, clean (`next.html`)

A second take outside the design system, clean and light (off-white, Inter, white cards, black buttons).

- Overview first: every item of the day in a list (Needs you, Worth a look, Good news, then Later and Done), the selected one open in a detail panel. Up and down arrows move through the list. Buttons say exactly what happens, and every action can be undone.
- Inbox: bulk shortcuts, plus a side panel to handle spam, drafted replies and "your call" items one by one.
- Draft a post: from the mention spike, a composer prefilled from what the agents know (the TikTok, the inbox questions, the Opale photo), with angles, quick edits, networks, a preview and suggested times. Scheduling for Wednesday 10:00 also completes the "Wednesday is empty" item.
- Top post: the workshop Reel did 3× the average, with why it worked. "Make a similar post" opens the same composer prefilled with what worked; "Adapt for TikTok" opens a short review step: the agent has already cropped it to 9:16, rewritten the caption and hashtags and picked a time; you check the cover, caption, sound and time in a phone preview, then schedule. Whichever post takes Wednesday 10:00 fills the empty day.
- ⌘K command bar, live agent feed, numbers below the list.

`deck.html` keeps the earlier swipe-card version for comparison.

Live: https://audreyalexandre3.github.io/today-proto/next.html
