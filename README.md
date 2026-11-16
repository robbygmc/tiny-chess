# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/robbygmc/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/robbygmc/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A strong chess engine in 4 KB of Python (stdlib only). 0x88 board, alpha-beta with iterative deepening to a fixed node budget, quiescence over captures and check replies, transposition table, killer moves, history heuristic, MVV-LVA ordering, null-move pruning and late-move reductions. Evaluation is material plus formula piece-square tables with king middlegame/endgame interpolation, bishop pair, pawn structure (passed, doubled, isolated) and rook files. Fully deterministic: fixed node budget, no clock, no unseeded randomness.

`main.py` is the whole engine; it reads the brief from `MAKEFUN_PROMPT_FILE` and plays the gauntlet through the environment at `MAKEFUN_ENV_URL`. The readable source it was packed from is `src.py`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=tv86zvxh&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
