# ⚡ FootballGPT | محرك التوقعات

> AI-powered football prediction engine built by a team of ML engineers and data scientists.
> The model is fully open source — no black box, no hidden logic. Read the code. Run it yourself. We have nothing to hide.
> **Telegram: [@FootballGPT_AR](https://t.me/FootballGPT_AR) | Contact: [@nuamansp](https://t.me/nuamansp)**
---

## 🤖 What is FootballGPT?

FootballGPT is a machine learning system designed to predict football match outcomes with statistical precision.

We are not tipsters. We are engineers who got tired of fake predictions and built our own system from scratch.

The model analyzes hundreds of variables per match — things the human eye cannot process — and outputs a probability score for every game it evaluates.

We only share picks when the model finds a **real edge**. No edge = no post. That is discipline, not laziness.

---

## ⚙️ The Stack

| Component | Technology |
|---|---|
| Primary Model | XGBoost + LSTM Neural Network |
| Training Data | 500,000+ match events |
| Coverage | 11 seasons × 8 major leagues |
| Odds Reference | Pinnacle (sharpest market in the world) |
| Feature Models | xG, PPDA, set pieces, fatigue, form decay |
| Language | Python 3.10+ |
| Key Libraries | scikit-learn, xgboost, pytorch, pandas, numpy |

---

## 🧠 How The Model Works

```
RAW DATA INGESTION
└── Historical match data (11 seasons)
└── Real-time odds movement (Pinnacle)
└── Player availability & injury reports
└── Team form, home/away splits, fixture congestion

FEATURE ENGINEERING
└── Rolling averages with form decay weights
└── ELO ratings adjusted by xG
└── Squad depth scoring
└── Set piece threat index
└── Defensive pressure metrics (PPDA)

MODEL LAYER (Ensemble)
├── XGBoost → classifies win/draw/loss probabilities
├── LSTM Neural Network → detects sequential patterns
└── Bayesian updater → calibrates against live odds

OUTPUT
└── P(Home Win) / P(Draw) / P(Away Win)
└── Model confidence score (1-10)
└── Edge calculation vs bookmaker implied probability
└── Value bet flag (edge > 6% only)

BANKROLL MANAGEMENT
└── Kelly Criterion staking
└── Maximum 2-3% of bankroll per bet
└── High selectivity — few picks per week
```

---

## 🏆 Leagues Covered

- 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Premier League
- 🌍 UEFA Champions League
- 🇪🇸 La Liga
- 🇩🇪 Bundesliga
- 🇮🇹 Serie A
- 🇫🇷 Ligue 1
- 🇳🇱 Eredivisie
- 🌍 AFCON / African Cup of Nations

---

## 📈 Model Performance

> Full public tracker updated every week. We show wins AND losses. Always.

| Season | Picks | Win Rate | ROI |
|---|---|---|---|
| 2023/24 | 187 | 58.3% | +11.2% |
| 2024/25 | 214 | 61.2% | +14.7% |
| 2025/26 | Ongoing | Updating... | Updating... |

> ⚠️ Past performance does not guarantee future results.
> Betting always carries risk. Never bet more than you can afford to lose.

---

## 🆓 Free Forever

Everything we publish is completely free.

- ✅ No VIP groups
- ✅ No paid subscriptions
- ✅ No hidden tiers
- ✅ No charges of any kind

The model is the product — not the monetization.

---

## 📱 Follow The Channel

All daily predictions, analysis and weekly reports are published on our Telegram channel.

👉 **[Join FootballGPT on Telegram](https://t.me/FootballGPT_AR)**

For questions about the model or the system:

👤 **[@nuamansp](https://t.me/nuamansp)**

---

## 🚀 Run It Yourself

```bash
# Clone the repository
git clone https://github.com/FootballGPT/football-model

# Create virtual environment
python -m venv footballgpt
source footballgpt/bin/activate  # Windows: footballgpt\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run predictions for upcoming fixtures
python predict.py --league PremierLeague --gameweek next
```

---

## 📁 Repository Structure

```
FootballGPT/
├── data/
│   ├── raw/              # Historical match data
│   ├── processed/        # Cleaned & engineered features
│   └── fixtures/         # Upcoming match data
├── models/
│   ├── xgboost_model.py  # XGBoost classifier
│   ├── lstm_model.py     # Neural network sequence model
│   └── ensemble.py       # Combined model output
├── features/
│   ├── xg_model.py       # Expected goals calculation
│   ├── ppda_model.py     # Defensive pressure metrics
│   ├── elo.py            # ELO rating system
│   └── form_decay.py     # Weighted form calculation
├── betting/
│   ├── value_bet.py      # Edge detection vs bookmaker
│   └── kelly.py          # Kelly criterion staking
├── tracker/
│   └── results.csv       # Full public pick history
├── predict.py            # Main prediction script
├── requirements.txt
└── README.md
```

---

## 🔬 The Value Betting Principle

We don't just predict winners. We find **mispriced odds.**

```
Example:
Our model says  → Man City win probability = 65%
Bookmaker implies → 57% (odds 1.75)

Edge = 65% - 57% = +8% ✅ Value Bet

Over hundreds of bets, positive edge = long term profit
even with a win rate below 60%
```

This is the core principle. Math over emotion. Always.

---

## ⚠️ Disclaimer

This project is for **educational and research purposes only.**
FootballGPT does not encourage irresponsible gambling.
Always bet within your means. If gambling affects your life, please seek help.

---

## 📜 License

MIT License — open source, free to use, free to modify.

---

> ⚽ **Football is not luck — it is mathematics.**
> الكورة مشي حظ — هي رياضيات

**Built with ❤️ by the FootballGPT Team**
**Telegram: [@FootballGPT_AR](https://t.me/FootballGPT_AR) | Contact: [@nuamansp](https://t.me/nuamansp)**
