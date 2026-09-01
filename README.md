# 🌐 Thirty Worlds

**Thirty tiny websites to learn, play, create and wander** — space, oceans, myths, music, games, wellness and more. One for every mood, every age group, and cultures from every corner of the world.

Every site is a single, fully self-contained `index.html` — all CSS and JS inline, no build step, no framework. External dependencies are limited to pinned CDN libraries (Three.js, GSAP + ScrollTrigger, Tone.js, canvas-confetti), Google Fonts, and flag images from flagcdn.com.

## 🚀 Live

**Hub (all 30 in one place):** https://thirty-worlds.vercel.app

Each world is also deployed as its **own standalone Vercel project**:

| # | World | Standalone URL | What it's for |
|---|-------|----------------|---------------|
| 1 | 🪐 Cosmos Explorer | https://tw-cosmos.vercel.app | Learn astronomy in an interactive 3D solar system (Three.js) — drag, zoom, tap planets for facts |
| 2 | ✨ Night Sky Stories | https://tw-night-sky.vercel.app | Eight real constellations on a twinkling canvas star map, each with its mythology |
| 3 | 🌊 Into the Deep | https://tw-ocean-depths.vercel.app | Scrollytelling descent 11,000 m through the five ocean zones with real creatures |
| 4 | ⚡ Physics Playground | https://tw-physics-lab.vercel.app | STEM sandbox — bouncing-ball physics with gravity, wind, friction and planet presets |
| 5 | 🧪 Element Lab | https://tw-periodic-table.vercel.app | All 118 elements, correctly laid out, color-coded, searchable, with real-world uses |
| 6 | 🦁 Alphabet Safari | https://tw-alphabet-safari.vercel.app | Toddlers learn letters — animal cards that bounce, speak aloud and burst confetti |
| 7 | 🃏 Memory Match | https://tw-memory-match.vercel.app | Kids' pair-matching game — 3 themes, 3 difficulties, star ratings, best times |
| 8 | 🔢 Math Arena | https://tw-math-arena.vercel.app | 60-second arithmetic sprints for ages 6–12 with streaks and personal bests |
| 9 | 📖 Story Forge | https://tw-story-forge.vercel.app | Kids build a read-aloud adventure story from heroes, places and problems |
| 10 | 🧠 Mind Gym | https://tw-mind-gym.vercel.app | Gentle brain training for seniors — trivia, number recall, odd-one-out, big adjustable type |
| 11 | 🍜 World Cuisine Atlas | https://tw-cuisine-atlas.vercel.app | Signature dishes of 16 cuisines with ingredients, badges and food-culture facts |
| 12 | 🎆 Festivals of the World | https://tw-festivals.vercel.app | A scrollytelling year of 10 festivals, each with its own palette and animated motif |
| 13 | 👋 Hello, World | https://tw-hello-world.vercel.app | Greetings in 20 languages in native script + romanization, spoken aloud |
| 14 | 🏺 Myth Codex | https://tw-myth-codex.vercel.app | 30 gods and legends across Greek, Norse, Egyptian, Hindu and Japanese traditions |
| 15 | 🏛️ Seven Wonders | https://tw-ancient-wonders.vercel.app | Layered parallax journey through the seven wonders of the ancient world |
| 16 | ⌨️ Typing Velocity | https://tw-type-racer.vercel.app | Typing speed trainer with real passages, live WPM/accuracy and a speed graph |
| 17 | 🚩 Flag Quest | https://tw-flag-quest.vercel.app | Geography quiz — 60 countries' flags with region filters and capital-city facts |
| 18 | 🐍 Neon Serpent | https://tw-snake.vercel.app | Retro arcade snake in CRT neon — keyboard, swipe or on-screen D-pad |
| 19 | ⭕ Tactic | https://tw-tic-tac-toe.vercel.app | Tic-tac-toe vs a minimax AI (unbeatable on Hard) or a friend |
| 20 | 🍳 Recipe Roulette | https://tw-recipe-roulette.vercel.app | Spin a physics wheel of 16 real dishes and get a cookable 5-step recipe |
| 21 | 🥁 Beat Lab | https://tw-beat-lab.vercel.app | 16-step, 6-voice drum machine + pentatonic synth pads (Tone.js) |
| 22 | 🎨 Color Theory Playground | https://tw-color-play.vercel.app | Six color harmonies, click-to-copy palettes and a WCAG contrast checker |
| 23 | 👾 Pixel Studio | https://tw-pixel-studio.vercel.app | Pixel-art editor with fill, mirror, eyedropper, undo and PNG export |
| 24 | 🌸 Haiku Garden | https://tw-haiku-garden.vercel.app | Generative 5-7-5 haiku in a zen scene that changes with the seasons |
| 25 | ☁️ Cloud Atlas | https://tw-cloud-atlas.vercel.app | The 10 cloud types with hand-drawn skies, altitude filtering and a quiz |
| 26 | 🫁 Stillpoint | https://tw-breathe.vercel.app | Guided box / 4-7-8 / coherent breathing with a glowing orb and sound cues |
| 27 | 🫀 Body Atlas | https://tw-body-atlas.vercel.app | Toggle five human body systems on one SVG map, with facts and a quiz |
| 28 | 💪 Fit Seven | https://tw-fit-seven.vercel.app | The classic 12-exercise 7-minute workout with countdown ring and form cues |
| 29 | 💰 Pocket Budget | https://tw-pocket-budget.vercel.app | Financial literacy for teens — live budget donut, 50/30/20 check, savings goals |
| 30 | 💡 Spark | https://tw-inventions.vercel.app | Scroll-drawn timeline of 12 inventions that changed everything |

Every world also lives on the hub at `https://thirty-worlds.vercel.app/<folder>/` (e.g. `/cosmos/`).

## 📁 Structure

```
.
├── index.html            # the hub — filter & search all 30 worlds
├── 404.html              # custom "lost world" page
├── cosmos/index.html     # each world = one folder, one self-contained file
├── night-sky/index.html
└── … (30 folders total)
```

## ✨ Built to a shared standard

- **Responsive** from 320 px phones to 4K — no horizontal page scroll, ≥44 px touch targets
- **Touch + mouse + keyboard** — games ship on-screen controls and swipe support
- **Accessible** — semantic landmarks, focus styles, ARIA labels, `prefers-reduced-motion` respected
- **Robust** — no console errors, gesture-gated audio, `localStorage` in try/catch, animations pause when the tab is hidden
- **Zero build step** — open any `index.html` in a browser, or deploy the folder anywhere static hosting exists

## 🛠 Deploy your own

```bash
# whole collection as one site
vercel deploy --prod

# any single world as its own site
vercel deploy --prod --cwd cosmos
```

---

Built with ❤️ as one collection — every world its own little site.
