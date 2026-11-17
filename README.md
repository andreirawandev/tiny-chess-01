# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/andreirawandev/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/andreirawandev/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact 0x88 chess engine in under 4 KB of Python: alpha-beta search with quiescence, a transposition table and MVV-LVA move ordering. Deterministic, standard library only, no model calls.

## Engine

0x88 board, alpha-beta search with quiescence (captures only), a transposition table, MVV-LVA move ordering with killer moves and a history heuristic, late move reductions, aspiration windows around the previous iteration's score, and iterative deepening to an 85,000-node cap (~3–4 s per move, under the 10 s limit). Evaluation: material, centrality, pawn advancement, passed-pawn bonus, rook on an open file, bishop pair, and king pawn-shield. Deterministic, Python 3.13 standard library only, no model calls.

Practice gauntlet (kit, 3 trials × 6 games): mean Elo 1432 (1191 / 1451 / 1654), above the 1,154 practice floor.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=hf4m3ky4&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
