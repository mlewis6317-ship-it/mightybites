# MightyBites

Interactive iPad mockups for a kids' meal-tracking + responsibility app. Avatars grow as kids eat well, evolve through a season, and earn cosmetics + badges.

## Live demo

Once GitHub Pages is enabled, the live prototype will be at:

**https://mlewis6317-ship-it.github.io/mightybites/**

## What's in here

- `index.html` — the live, deployable interactive prototype (open this on iPad in landscape).
- `mockups.html` — original snapshot of the mockup as a reference.

## Screens

The prototype has 9 navigable screens:

- **Home (Leaderboard)** — kitchen-iPad view showing the family ranking, sluggish/hungry kids flagged, tap-to-log flow
- **Choose Buddy** — character picker with growth path preview
- **Profile** — avatar, weekly goal, trust pill, badges strip, growth strip
- **Meal Log** — food groups, meal time picker, dinner expectations & bonuses, animated feed-the-dino XP
- **Trophies** — lifetime stats, latest cosmetic unlock, dressing room (drag-and-drop cosmetics on a 3D avatar), Champions Wall, full badge collection
- **Responsibility** — kid-only view showing trust meter, privileges, daily + weekly chores
- **Settings** — PIN-locked parent zone with family members, behavior bonuses, per-kid responsibility setup with age-appropriate suggestions and conversation prompts, trust rewards, app preferences
- **Recap (Kid)** — Spotify-Wrapped-style 6-card swipeable weekly recap
- **Recap (Parent)** — analytical weekly recap with per-kid insights

## Core systems

**Dual-currency.** Strength (food XP) drives the leaderboard. Trust (responsibility) earns privileges. Different lanes so younger kids aren't unfairly compared to older siblings on chores.

**Dinner is the main quest.** Eating dinner all 7 nights = 700 pts = the weekly goal. Breakfast/lunch are bonus (25% each). The 5 healthy food groups sum to 100 pts per dinner: Veggies 25, Protein 25, Dairy 20, Fruit 15, Grains 15.

**Scaling urgency.** When a food group hasn't been logged in 48hrs the avatar starts asking. Bonuses scale: 48hr +25, 72hr +35, 96hr +50.

**Treats penalty.** Skipping a treat = +5. First treat = 0. Second = -5. Third+ = -15 and the avatar goes queasy/sick.

**Hybrid progression.** Lifetime stage (months to climb) for permanent identity + weekly score (resets) for the leaderboard race.

**Age range 3+.** Tracking starts at age 3 with picture-led, very small chores. Age-appropriate suggestions in Settings.

## Tech

Single-file static prototype: HTML + CSS + vanilla JS, no build step. Designed for iPad landscape but responsive to portrait. All state lives in memory for now — no persistence yet.
