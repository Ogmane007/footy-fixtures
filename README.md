# ⚽ Footy Fixtures & Picks

A clean, fast football fixtures and prediction app built for **clarity, transparency, and experimentation**.

This project combines **real match data**, **statistical models**, and **modern UI** to help explore football fixtures, probabilities, and pick performance — without pretending to be a betting oracle.

---

## ✨ What this app does

* 📅 Browse **fixtures by competition and date**
* 📊 Generate **statistical match probabilities** (Poisson-based)
* 🏆 See **Top 3 picks** per match with confidence levels
* 💾 **Save picks locally** (no accounts, no backend)
* 📈 Track **pick accuracy over time** (wins / losses / win rate)
* 💰 Compare **model probability vs odds** (mocked but realistic)
* 🧠 "Explain the pick" — see *why* the model leans a certain way
* ⏱ Live kickoff countdowns + team logos

Everything runs **client-side**, fast, and transparently.

---

## 🧠 How predictions work (in plain English)

This app **does not use AI predictions**.

Instead, it uses:

* Recent team form (last N finished matches)
* Goals for / against averages
* Home vs away adjustments
* A **Poisson goal model** to estimate score probabilities

From that, it derives:

* Home / Draw / Away
* Over 2.5 goals
* Both Teams To Score (BTTS)

Odds are currently **mocked**, then compared to the model to show:

* Implied probability
* Value edge (model − market)

> ⚠️ No injuries, lineups, tactics, or live odds movement are included (yet).

---

## 🖥 Tech stack

* **Next.js (App Router)**
* **TypeScript**
* **Tailwind CSS**
* Football-Data.org API (fixtures, teams, results)
* LocalStorage for saved picks & history

No database. No auth. No server-side state.

---

## 📂 Key features & pages

* `/` — Fixtures browser
* `/match/[id]` — Match picks, odds comparison, explanations
* `/saved` — Saved picks with filters & delete

---

## 🧪 Experimental by design

This project is intentionally:

* Opinionated
* Transparent
* Easy to extend

Planned / future ideas:

* Elo-style team ratings
* Head-to-head weighting
* Home/away performance splits
* Real odds APIs + caching
* Odds movement tracking

---

## ⚠️ Disclaimer

This app is **for educational and analytical purposes only**.

It is **not betting advice**.
Use responsibly.

---

## 🚀 Running locally

```bash
npm install
npm run dev
```

Add your Football-Data API key to `.env.local`:

```env
FOOTBALL_DATA_API_KEY=your_key_here
```

---

## 🙌 Why this exists

This project was built to:

* Practice clean data modeling
* Explore football analytics
* Design a professional sports UX
* Stay honest about what models can and *can’t* do

If you like football, data, or building thoughtful tools — you’ll feel at home here.

---

