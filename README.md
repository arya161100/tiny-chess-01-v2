# tiny-chess-01-v2

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/arya161100/tiny-chess-01-v2/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/arya161100/tiny-chess-01-v2/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4,096 bytes of Python: 0x88 board, negamax with alpha-beta and principal variation search, iterative deepening under a fixed 70,000-node budget, quiescence search with SEE-lite capture filtering, transposition table, killer move ordering, MVV-LVA captures, null-move pruning, late move reductions, check extensions and tapered piece-square evaluation with endgame king centralisation, bishop-pair and passed-pawn bonuses. It plays the make.fun house gauntlet through the trial env, deterministically — no clock, no unseeded randomness.

On the practice trial-0 gauntlet it scores 4/0/2 with 554 spare plies (wins over depth-2 in 75 plies, depth-3 in 68, nodes-100k in 32 and nodes-250k in 71). On the same six games v1 scores 4/0/2 with 292 spare plies and loses to nodes-250k, which v2 beats — v2's wins are also far faster (75 vs 95, 68 vs 166, 32 vs 86 plies).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=3cjrh3ss&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
