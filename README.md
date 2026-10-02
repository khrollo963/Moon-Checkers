# LUNAR MYTH DRAUGHTS: PLAY HERE https://khrollo963.github.io/Moon-Checkers/
# Support the Itch.io build https://kennyfromthering.itch.io/checkers
# Play on NEWGROUNDS: 

A roguelike checkers game told in two mythologies at once. Pick your pantheon at the title screen — **Kemetic** or **Hellenic** — and wager against the moon to win back the days lost to a jealous sun god's curse.

☾ ☥ ☾

---

## PICK YOUR THEME

Lunar Myth Draughts is one game told two ways. Choosing a theme is the first thing you do, and it's locked in for the rest of the session — no switching mid-run.

### Kemetic
You play as **Thoth** (Djehuty, Lord of Writing) against **Khonsu**, the Wanderer, Moon God. **Ra** cursed **Nut**, the sky goddess, and Thoth wagers with the moon to win her freedom back.

### Hellenic
You play as **Hermes**, Herald of Olympus, against **Selene**, Titaness of the Moon. **Helios** cursed **Rhea**, mother of the gods, and Hermes wagers with the moon on her behalf.

Everything reskins with the theme — names, dialogue, the myth text, the difficulty tiers, the piece icon, even the two character portraits and the backdrop's infrastructure (pyramids for Kemetic, a temple colonnade for Hellenic). **Achievements and your all-time best run are shared across both** — beating the game as Hermes counts exactly the same as beating it as Thoth.

---

## THE MYTH

**The sun cursed the mother goddess**, forbidding her from bearing children on any day of the calendar year. For eons, she remained barren while the cosmic cycle turned.

**The messenger god took pity on her.** He wagered with the moon, playing with skill and cunning. With each victory, he carved out moments outside the calendar — five sacred days where the curse held no power.

**On these five days, five gods were born:**

| Kemetic | Hellenic |
|---|---|
| Osiris, god of resurrection | Hades |
| Horus the Elder, lord of the sky | Zeus |
| Set, god of chaos and storms | Typhon |
| Isis, goddess of magic | Demeter |
| Nephthys, lady of mourning | Hecate |

The tale survives in Plutarch's *On Isis and Osiris*, which names Hermes and Selene directly, identifying them with Thoth and the Egyptian moon — it's the same myth either way, just carried by different names. Now **you take the messenger's place.** Can you outplay the moon and secure the Five Days once more?

---

## HOW TO PLAY

**Lunar Myth Draughts** is American draughts (checkers) with a roguelike twist:

- **Select a difficulty** at the start menu — it's locked for the whole run
- **Win 5 consecutive games** against the moon to complete your run and conquer the Duat
- **Lose even once — or stalemate — and your run ends.** Return to the menu with your streak reset to 0

### Checkers Rules

**Moving**
- Blue pieces move one dark square diagonally forward onto an empty square
- Men never move backward

**Capturing**
- Jump diagonally over an enemy piece into the empty square behind it, and remove it
- **Capturing is mandatory** — if you can jump, you must
- Multi-jumps are forced — if the same piece can jump again, it must keep going

**Kings**
- A man reaching the far row is crowned and stacks a second disc
- Kings move and capture one square at a time, forward or backward
- A man crowned mid-capture ends its turn there

**Winning**
- Capture every enemy piece, or leave your opponent with no legal move
- **Forty moves with no capture or promotion is a stalemate — and it counts as a loss.** A live countdown above the board tracks it, turning red once it's running low

### Who Moves First

Within a single Duat Run, first move alternates by round: **rounds 1, 3, and 5 you move first; rounds 2 and 4, the moon does.**

### The Moon

The crescent gauge shows how much light your opponent still holds. Every capture shifts the balance.

### Roguelike Mechanics

- **Duat Run counter** — shows your current win streak, 0 to 5
- **Difficulty lock** — once picked, it stays locked for the entire run
- **One loss or stalemate ends the run** — the counter resets and you return to the menu
- **Five wins = victory** — conquer 5 consecutive games at your chosen difficulty to free the Five Days

---

## SETTINGS

All under the **Game** menu:

- **New Game** — start over (confirms first if a game's in progress), returns to the title screen
- **Board Colors** — pick a square color scheme: Desert (default), Black & White, Red & Black, or Green & White
- **Change Theme** — confirms, then returns you to the title screen to pick Kemetic or Hellenic again
- **Piece Movement** — toggle between **Sliding** (animated) and **Snappy** (instant, no transition)
- **Sound** — on/off

Board color and piece movement preferences persist across sessions. Theme does not — it's a fresh choice every time you return to the title screen, by design.

---

## ACHIEVEMENTS

Four tiers, tracked in their own tab, shared across both themes and every difficulty:

| Tier | Achievement | Condition |
|---|---|---|
| 🏆 Human | Range | Capture twice in a single move |
| 👑 King | Promotion | Promote a piece to a king |
| 🌙 Demi-God | Winner | Beat the game (5 wins) on any difficulty |
| ⚡ God | Thrice Great | Beat the game on all three difficulties |

Winner and Thrice Great show live progress bars — Winner tracks your all-time best round reached (never regresses on a loss), and Thrice Great tracks how many difficulty tiers you've fully beaten.

---

## CONTROLS

**Mouse / Touch** — click a piece to select it, click a destination to move, click buttons for menus and navigation.

**Keyboard**
- `F2` — New Game (confirms first if a game's in progress)
- `Esc` — close menus

**Move Log** — a running list of every move in algebraic notation (a1–h8), captures marked and color-coded by side.

---

## DIFFICULTY LEVELS

Same underlying AI depths and behavior in both themes — only the names change.

| Tier | Kemetic | Hellenic | Behavior |
|---|---|---|---|
| Easy | Scribe | Grammateus | Plays conservatively, blunders often. Good for learning. |
| Medium | Vizier | Archon | Plays tactically, sets up captures and kings. A fair fight. |
| Hard | Pharaoh | Basileus | Plays aggressively, rarely blunders. A real test. |

---

## TECHNICAL

A single self-contained HTML5 file — no build step, no dependencies, no external assets. Open it in a browser and it runs.

- Vanilla JavaScript, no frameworks
- Canvas-based pixel art for every character portrait, piece icon, and background scene — all drawn procedurally, nothing is a raster image
- Web Audio API for procedurally generated sound effects — no audio files
- `localStorage` for achievements, best-run tracking, and preferences, with a startup probe that warns you plainly if storage isn't actually persisting in your browser/environment
- Responsive layout with dedicated handling for short landscape viewports (mobile/tablet)
- Windows XP–inspired retro UI throughout

### Browser Support
Any modern browser with Canvas and Web Audio API support: Chrome/Chromium 88+, Firefox 85+, Safari 14+, Edge 88+.

---

## ANCIENT SOURCES

The myth of a wisdom god's gamble with the moon, winning back five days for a cursed sky goddess, is recorded in Egyptian tradition and referenced in the Book of Thoth. The Five Days (Epagomenal Days) were celebrated as sacred and outside the normal 360-day calendar. Plutarch's *On Isis and Osiris* preserves the Greek telling, naming Hermes and Selene directly and identifying them with the Egyptian pair — which is exactly why this game can tell the same story both ways.

The draughts rules follow **American Checkers** (English Draughts): mandatory captures, forced multi-jumps, backward-moving kings.

---

## CREDITS & SUPPORT

**Lunar Myth Draughts** is created by **Uthman Ken** (known magically as **Mufti Khrollo**), an independent author, occultist, and digital creator exploring the intersection of Islamic esotericism and Western Hermetic magic.

This game is part of a broader mission: digitizing medieval Islamic and Hermetic knowledge — talismanic squares, angelic correspondences, gematria systems, and divination frameworks — into interactive digital instruments for contemporary practitioners.

- **YouTube**: [@TBOG786](https://www.youtube.com/@TBOG786)
- **Substack**: [mufti963khrollo](https://mufti963khrollo.substack.com)
- **TikTok**: [@thegnosticmuslim](https://www.tiktok.com/@thegnosticmuslim)
- **Instagram**: [@khrollo963](https://www.instagram.com/khrollo963)
- **GitHub**: [khrollo963](https://github.com/khrollo963)
- **Amazon**: [Uthman Ken](https://www.amazon.com/s?k=Uthman+Ken)
- **Support via PayPal**: [@everythingken](https://www.paypal.com/donate/?hosted_button_id=everythingken)

---

## PLAY NOW

Pick your pantheon. Wager with the moon. Win back the Five Days.

**Good luck. The moon is waiting.**

☾ ☥ ☾
