<div align="center">

# 💘 A Love Story in Code

### *Because some feelings are too big for a text message.*

<br>

![Made with Love](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20Love-ff69b4?style=for-the-badge)
![Built with](https://img.shields.io/badge/Built%20with-Vanilla%20JS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)
![No Install](https://img.shields.io/badge/Setup-Zero%20Required-00c896?style=for-the-badge)
![Runs Anywhere](https://img.shields.io/badge/Runs%20on-Any%20Browser-4285f4?style=for-the-badge&logo=googlechrome&logoColor=white)
![Vibes](https://img.shields.io/badge/Vibes-Immaculate-9b59b6?style=for-the-badge)

<br>

> *A pixel-art RPG. A three-level apology. One real story.*
> *Built from scratch with nothing but JavaScript, a canvas, and way too many feelings.*

<br>

</div>

---

## 📖 The Story Behind This

This didn't start as a "project."

It started as a feeling — that hollow, restless kind you get when words stop being enough. When you've said sorry in every way language allows and it still doesn't feel like it captures the weight of what you actually mean.

So instead of another text, another call, another conversation that goes in circles — this happened. A game. A whole world built from scratch, where every pixel placed was a sentence that couldn't be spoken out loud.

Three levels. Each one a different chapter of something real:
- A sunlit park where you pick up pieces of yourself
- A storm you have to fight your way through
- A bridge you build, question by question, over a chasm you created

It's not a masterpiece of engineering. It's not the most technically complex thing ever written. But it was made with everything. And sometimes that's the most powerful language there is.

> *This project was built with the assistance of AI (Claude by Anthropic) — for the logic, the patterns, the structure. But every story beat, every dialogue line, every design choice? That was entirely human. That part, no AI can write for you.*

---

## ✨ What Makes This Special

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   🎮  A complete 3-level RPG — in a single HTML file       │
│   📱  Runs on any phone, tablet, or desktop                 │
│   🎨  Hand-drawn pixel art sprites on HTML5 Canvas         │
│   💬  Typewriter dialogue system with a character queue     │
│   🌉  A quiz mechanic that literally builds a bridge        │
│   😈  A boss fight against your own ego                     │
│   💕  Two endings — both honest, both beautiful             │
│   ⚡  Zero dependencies. Zero installs. Zero excuses.       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## 📱 Running It — Seriously, It's This Easy

**On your phone (the whole point):**

```
1. Download RPG.html
2. Tap to open it
3. It runs in your browser instantly
```

That's it. No app store. No install. No account. No loading screen that makes you question your life choices. Just download one file, tap it, and you're in.

Works on:
- 📱 Android (Chrome, Firefox, Samsung Browser)
- 🍎 iPhone & iPad (Safari, Chrome)
- 💻 Any desktop browser
- 🖥️ Literally anything with a modern browser

---

## 🗺️ The Three Levels

<br>

### 🌸 Level 1 — The Sunlit Park
*"Picking up the pieces."*

The world is still bright here. Walk through a park scattered with letters — 14 of them, each one a fragment of something worth saving. Find the pink flower. Use it to melt the thorny vine that's been blocking the way forward.

A gentle level. The calm before everything else.

---

### ⛈️ Level 2 — The Stormy Maze
*"Fighting through the noise."*

The sky turns dark. Five storm clouds rage through a maze — they represent everything ugly: the ego, the anger, the words said in the wrong moment. Shoot them down with heart projectiles. Clear the storm. Find what's waiting at the other end.

The hardest level to move through. That's intentional.

---

### 🌉 Level 3 — The Bridge of Promises
*"Building something from nothing."*

A chasm splits the world in two. The only way across is to answer honestly — five questions, five chances to prove something. Each right answer lays another plank on the bridge. Then cross it. Face your own ego as a literal final boss. Watch it fall.

Make your choice. That part is real.

---

## 🕹️ Controls

### 📱 Mobile Touch Controls
| Button | Does |
|--------|------|
| ⬆️ ⬇️ ⬅️ ➡️ | Move the character |
| 🅰️ **ACTION** | Talk · Interact · Shoot hearts · Advance dialogue |
| ❓ **HINT** | Get a nudge when you're stuck |
| 📖 **GUIDE** | Full step-by-step level walkthrough |

### 💻 Keyboard (Desktop)
| Key | Does |
|-----|------|
| `Arrow Keys` | Move |
| `Space` / `Enter` | Action |

---

## 🛠️ Make It Yours

This game is fully customisable. Fork it. Change the names. Rewrite every line of dialogue. Make it your own love story, your own apology, your own celebration.

Here's where to look:

| What to change | Where to find it |
|----------------|-----------------|
| Character names | Search `[Male Character]` and `[Female Character]` — replace everywhere |
| Intro story text | `game.init()` → the `text` variable at the top |
| All dialogue lines | Search `'Insert your custom dialogue'` — replace each one |
| MCQ questions | `mcq.questions` array — write your own questions and answers |
| Ending messages | `game.makeChoice()` → update both the forgive and wait endings |
| Player speed | `this.speed = 1.6` in the Player constructor |
| Number of letters | Level 1 setup — the `letters` and `positions` arrays |

---

## 🏗️ Under the Hood

```
Single HTML file (~1,700 lines)
├── CSS         — pixel-art rendering, responsive layout, animations
├── HTML        — canvas + UI overlays + on-screen controls
└── JavaScript
    ├── State machine     (INTRO → PLAYING → DIALOGUE → MCQ → END)
    ├── Player class      (movement, collision, animation, inventory)
    ├── Level class       (world setup, enemies, collectibles, drawing)
    ├── Dialogue system   (typewriter queue with cached DOM refs)
    ├── MCQ system        (quiz → bridge block counter)
    └── Game loop         (requestAnimationFrame + screen shake)
```

**No frameworks. No bundler. No node_modules folder haunting your hard drive.**

Just one file that does everything.

---

## 💡 Technical Highlights

- **Zero-jank dialogue** — DOM elements are cached once at init, written to once per character reveal. No per-frame `getElementById` calls causing reflow.
- **Axis-split collision** — X and Y collision checked independently so the character slides along walls instead of stopping dead.
- **Diagonal normalisation** — movement vector is normalised so diagonal speed equals cardinal speed.
- **State-preserving modals** — hint and guide overlays save the previous game state and restore it on close, so opening a hint mid-dialogue doesn't break the story.
- **Anti-double-fire keyboard** — action key tracked with a `keydown` guard flag so holding Enter doesn't flood the game with events.

---

## 📜 License

MIT — completely open source. Take it, break it, rebuild it. Make someone cry happy tears with it.

The only rule: **don't use it to hurt anyone.** This whole thing was built on the opposite of that.

---

## 🤝 Built With

| Thing | Why |
|-------|-----|
| HTML5 Canvas | Drawing every pixel of the game world |
| Vanilla JavaScript | Running every frame of logic |
| CSS | Making the UI look like it belongs |
| Claude (Anthropic) | AI assistance for logic patterns and code structure |
| One human heart | Everything else |

---

<div align="center">

<br>

*It's just code. But it isn't, really.*

*Some of the best things humans make start as something they needed to say*
*and didn't know how.*

<br>

**⭐ If this made you feel something — leave a star. It means a lot.**

<br>

![forthebadge](https://img.shields.io/badge/FOR-HER-ff69b4?style=for-the-badge)
![forthebadge](https://img.shields.io/badge/BUILT%20WITH-FEELINGS-e74c3c?style=for-the-badge)
![forthebadge](https://img.shields.io/badge/RUNS%20ON-LOVE-9b59b6?style=for-the-badge)

</div>
