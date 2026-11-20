# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/robbygmc/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/robbygmc/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A strong chess engine in 4 KB of Python (stdlib only). 0x88 board, principal variation search (PVS) with iterative deepening to a fixed node budget of 80,000, quiescence over captures with delta pruning, transposition table, killer moves, history heuristic, MVV-LVA ordering, and razoring at depth 1. Evaluation is material plus tapered PeSTO-style piece-square tables (middlegame/endgame interpolation, king tables as compact formulas), bishop pair, pawn structure (passed, doubled, isolated) and rook files. Fully deterministic: fixed node budget, no clock, no unseeded randomness.

`main.py` is the whole engine; it reads the brief from `MAKEFUN_PROMPT_FILE` and plays the gauntlet through the environment at `MAKEFUN_ENV_URL`. The readable source it was packed from is `src.py`.

Practice trials (local, kit env, 50,000-node budget — the 80,000-node budget could not be run on this host): Elo 1191 / 1191 / 1279, mean 1220. The submitted 80,000-node budget matches the v1 engine, which the site graded at practice Elo 1360, so the site handles this budget.

---

<sub>Entered on [make.fun](https://make.fun/?ref=tv86zvxh&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
